---
title: Entender os filtros EXISTENTES
description: Saiba o que é um filtro EXISTE, o que ele pode fazer por você e como criá-lo do zero. Além disso, veja vários exemplos úteis de filtros EXISTE.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
type: Tutorial
role: User
level: Intermediate
jira: KT-1880
last-substantial-update: 2025-08-25T00:00:00Z
doc-type: video
exl-id: f518a919-0c44-4122-873a-e2f10e3162d5
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '682'
ht-degree: 4%

---

# Entender os filtros EXISTENTES

Os filtros EXISTS são avançados, filtros de modo de texto, que nos permitem contornar a limitação de salto de 2 tabelas/campos em um Report Builder padrão. Ou podem ser usados para identificar objetos no sistema que não têm uma condição de relação específica por meio de NOTEXISTS.

Neste vídeo, você aprenderá a criar um filtro EXISTE para ver &quot;Aprovações de prova em projetos atuais&quot; em um relatório de aprovações de prova.

Para obter uma apresentação mais detalhada sobre como o EXISTS funciona, consulte [Criar filtros complexos do modo de texto usando instruções EXISTS](https://experienceleague.adobe.com/pt-br/docs/workfront/using/reporting/reports/text-mode/create-complex-text-mode-filters-using-exists-statements).

>[!VIDEO](https://video.tv.adobe.com/v/3471181/?quality=12&learn=on&enablevpops=1)

## Exemplos de filtro EXISTE

### O relatório do projeto JÁ EXISTE

Isso usa a tarefa como o objeto de vinculação, comparando a projectID encontrada no nível da tarefa e correspondendo-a ao campo de ID do nível do projeto. Isso nos permite comparar os usuários de atribuição na tarefa com um curinga $$USER.ID. Isso resulta na devolução somente de projetos nos quais o usuário de visualização está atribuído a um
tarefa, independentemente de ser o principal responsável ou não.

```
EXISTS:A:$$OBJCODE=TASK
EXISTS:A:assignmentsUsersMM:ID=$$USER.ID
EXISTS:A:assignmentsUsersMM:ID_Mod=in
EXISTS:A:projectID=FIELD:ID
```


Isso usa o problema (optask) como o objeto de vinculação, também comparando a projectID encontrada no nível de problema (optask) e correspondendo isso ao campo de ID do nível de projeto. Em seguida, verifica se algum desses problemas (optasks) tem uma data de entrada dentro do intervalo especificado. Nesse caso, retornaria qualquer projeto que tenha
não teve um problema (optask) registrado em um acumulado nos últimos 30 dias, devido ao NOTEXISTS.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=OPTASK
EXISTS:A:entryDate=$$TODAY
EXISTS:A:entryDate_Mod=between
EXISTS:A:entryDate_Range=$$TODAY-30d
EXISTS:A:projectID=FIELD:ID
```

### O relatório de modelo EXISTE

Este filtro mostrará todos os modelos que não foram usados para criar um projeto ou que foram anexados a um projeto no ano passado. Uma advertência é que para descobrir se um modelo foi usado ou não como um anexo, ele depende de esse modelo ter tarefas nele.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=TASK
EXISTS:A:entryDate=$$TODAY-1y
EXISTS:A:entryDate_Mod=gte
EXISTS:A:templateTask:templateID=FIELD:ID
EXISTS:B:$$EXISTSMOD=NOTEXISTS
EXISTS:B:$$OBJCODE=PROJ
EXISTS:B:entryDate=$$TODAY-1y
EXISTS:B:entryDate_Mod=gte
EXISTS:B:templateID=FIELD:ID
```

### O relatório da tarefa JÁ EXISTE

Isso usa a tabela Usuário como o objeto de vinculação, conectando pela taskID de atribuições e pela ID de tarefas. Em seguida, verifica a coleção de IDs das equipes para as IDs de equipe do usuário, retornando a tarefa se qualquer um dos atribuídos estiver na mesma equipe que o usuário que está visualizando.

```
EXISTS:1:$$OBJCODE=USER
EXISTS:1:teams:ID=$$USER.teamIDs
EXISTS:1:userAssignments:taskID=FIELD:ID
```

### EXISTE UM RELATÓRIO DE USUÁRIO

Isso retornará todos os usuários que não postaram uma atualização nas últimas 3 semanas. Isso usa o objeto da nota para preencher a lacuna e compara a ID do proprietário a uma ID do usuário. Em seguida, retorna esse usuário se nenhuma nota de sua propriedade tiver uma data de entrada superior a 3 semanas atrás.

```
EXISTS:A:$$OBJCODE=NOTE
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:ownerID=FIELD:ID
EXISTS:A:entryDate=$$TODAY-3w
EXISTS:A:entryDate_Mod=gt
```

Isso retornará todos os usuários que não registraram horas na última semana. Isso usa um método extremamente semelhante ao exemplo acima, mas usa as informações do proprietário da hora e a data de entrada da hora para basear quais usuários ela retorna.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=HOUR
EXISTS:A:entryDate=$$TODAY-1w
EXISTS:A:entryDate_Mod=gte
EXISTS:A:ownerID=FIELD:ID
```

Em um relatório de usuário, mostrar uma lista de usuários que corresponde à guia Pessoas de um projeto.

```
EXISTS:1:$$OBJCODE=PRTU
EXISTS:1:projectID=<projectID>
EXISTS:1:userID=FIELD:ID
```

### Relatório de Categoria (Formulário Personalizado) EXISTE

Este texto lhe fornecerá uma lista de todos os formulários de projeto que nunca foram usados em um projeto. Isso deve ser usado junto com a especificação do tipo de objeto do formulário em que estamos focados. Nesse caso, o foco é PROJ, portanto, devemos incluir as chamadas nas linhas objTypes. Isso poderia ser usado
para outros tipos de objeto alterando as partes relacionadas ao código do objeto. Isso verifica a coleção de projetos anexados aos formulários listados e retorna se não houver correspondência.

```
EXISTS:A:$$OBJCODE=PROJ
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:objectCategories:categoryID=FIELD:ID
objTypes=PROJ
objTypes_Mod=in
```

### Relatório de Parâmetro (campo personalizado) EXISTE

Isso retorna qualquer campo personalizado que não esteja atualmente anexado a um formulário personalizado no sistema.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```

### O relatório JÁ EXISTE

Isso retornará qualquer relatório que use um valor específico em seus filtros.

```
EXISTS:1:$$OBJCODE=UIFT
EXISTS:1:ID=FIELD:filterID
EXISTS:1:preference:value=<value here>
EXISTS:1:preference:value_Mod=cicontains
```

Isso retornará qualquer relatório anexado a qualquer painel.

```
EXISTS:A:$$OBJCODE=PRTBSC
EXISTS:A:internalSectionID=FIELD:ID
EXISTS:A:portalTab:ID_Mod=notblank
```

### EXISTE relatório de aprovação de prova

Isso retornaria aprovações de prova somente em projetos com o status Atual. Isso usa o objeto Document para preencher a lacuna da aprovação de prova para o projeto, verificando o currentVersionID para o documentVersionID. A partir daí, vamos para o status dos projetos.

```
EXISTS:1:$$OBJCODE=DOCU
EXISTS:1:currentVersionID=FIELD:documentVersionID
EXISTS:1:project:status=CUR
EXISTS:1:project:status_Mod=in
```
