---
title: Entender o modo de texto básico para filtros
description: Saiba qual é o modo de texto, qual é o caso de camel e algum modo de texto "plug and play" básico que você pode usar nos filtros de relatório em [!DNL  Workfront].
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
source-git-commit: 59ac9907b116f8abadf5e15f8de351c02a7a2909
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# Entender o modo de texto básico para filtros

>[!IMPORTANT]
>
>Pré-requisitos:
>
>* Entender os elementos de relatório
>* Entender os componentes de relatório
>* Criar um filtro básico


Neste vídeo, você aprenderá:

* O modo de texto é
* Qual é o caso do camelo?
* Algum modo de texto &quot;plug and play&quot; básico que você pode usar nos filtros de relatório

>[!VIDEO](https://video.tv.adobe.com/v/336820/?quality=12)

O modo de texto a seguir excluirá tarefas em que um usuário marcou &quot;Concluído com a minha parte&quot;. Tudo o que você precisa fazer é criar um filtro de tarefa, adicionar as regras de filtro desejadas, alternar para o modo de texto e colar o código abaixo após qualquer modo de texto que você ver no filtro.

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

## Filtros adicionais do modo de texto de plug-in e play

### Tarefa - Mostrar todas as tarefas que aguardam a minha aprovação

```
approvalProcessID_Mod=notblank
currentUserApproversMM:ID=$$USER.ID
currentUserApproversMM:ID_Mod=in
currentUserApproversMM_Join=allowingnull
```

### Tarefa - Mostrar todas as tarefas que aprovei

Crie um relatório de tarefa com os filtros desejados, vá para a guia Filter e clique em Switch to Text Mode. Adicione este código ao que já estiver lá:

```
approvalProcessID_Mod=notblank
approverStatuses:approvedByID=$$USER.ID
approverStatuses:approvedByID_Mod=in
```

### Tarefa - Mostre-me todas as tarefas que tenham pelo menos um antecessor entre projetos

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

### Tarefa - Mostrar todas as tarefas que atribuí a outros

Crie um relatório de tarefa com os filtros desejados, vá para a guia Filter e clique em Switch to Text Mode. Adicione este código ao que já estiver lá:

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

Isso mostrará todas as tarefas em que o usuário conectado atribuiu pelo menos um dos destinatários atuais. Se os destinatários tiverem sido atribuídos por várias pessoas, somente o nome da primeira pessoa que atribuiu alguém será exibido como &quot;Solicitado por&quot; na página de aterrissagem da tarefa.

## Atividade: Perguntas sobre o modo de texto

1. Como você escreveria o caso de camelo para o campo intitulado &quot;Inserido por ID&quot;?
1. Em um relatório de Ocorrência , crie um filtro para mostrar os problemas que foram marcados como fechados, mas que estão pendentes de aprovação.

### Respostas

1. O caso de camelo para o campo &quot;Inserido por ID&quot; deve ser escrito da seguinte maneira — enteredByID
1. O modo de texto deve ter esta aparência no filtro de relatório de problemas:

   ![Uma imagem da tela para criar um novo filtro no modo de texto](assets/btm-answer.png)
