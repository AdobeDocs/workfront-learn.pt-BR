---
title: Criar instruções OU em filtros
description: Saiba como usar uma instrução OU para informar ao Workfront que você deseja ver isto OU aquilo em seu relatório.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
thumbnail: create-or-statements-in-filters.png
type: Tutorial
role: User
level: Intermediate
jira: KT-9987
exl-id: 1a56f2f6-12df-43a5-943c-986a85661efa
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '915'
ht-degree: 100%

---

# Criar instruções OU em filtros

Ao criar um filtro com diversas linhas de critérios, por padrão, o Workfront coloca um E entre cada linha. Isso garante que, ao usar esse filtro, cada resultado na lista atenda a todas as regras de filtro.

Neste exemplo, temos três critérios (ou regras) para um filtro de projeto:

1. O projeto deve ter uma data de conclusão planejada que ocorra no mês atual.
1. O projeto deverá estar no portfólio de Marketing de eventos.
1. Ele deve ser um projeto ativo, ou seja, deve ter o status Atual.

![Uma imagem da criação de um filtro com instruções E no [!DNL Workfront]](assets/or-statement-1.png)

Os projetos na lista de resultados atendem a todos esses três critérios, ajudando você a restringir os resultados da pesquisa para ver as informações exatas de que precisa.

![Uma imagem de uma lista filtrada no [!DNL Workfront]](assets/or-statement-2.png)

No entanto, pode haver momentos em que você deseja que os resultados do filtro atendam a vários critérios, e é nesse momento que as instruções OU podem ajudar. Com uma instrução OU, você informa ao filtro que deseja ver coisas que correspondam a QUALQUER uma de suas instruções OU, em oposição a TODAS as suas instruções E.

## Usar instruções OU

As instruções OU expandem ou aumentam a quantidade de informações que o filtro encontra, visto que para aparecer na lista de resultados, um item precisa atender a apenas uma das regras de filtro e não a todas.

Vejamos uma instrução OU simples: projetos nos quais você atua como gerente (proprietário) de projetos OU projetos que foram criados por você.

![Uma imagem da criação de um filtro com instruções OU no [!DNL Workfront]](assets/or-statement-3.png)

Depois de configurar ambas as regras de filtro, clique no E entre elas e mude para OU.

![Uma imagem da criação de um filtro com instruções OU no [!DNL Workfront]](assets/or-statement-4.png)

O OU entre as duas regras de filtro expande seus critérios de pesquisa, solicitando que o Workfront encontre projetos que atendam a uma ou outra dessas opções: projetos que possuem seu nome no campo de proprietário ou projetos que você criou.

## Várias regras de filtro com instruções OU

Agora vamos examinar uma instrução OU que contém diversas regras de filtro em cada lado da instrução. Este caso utiliza as mesmas duas regras de antes, mas adiciona outra: os projetos também devem ter um status Atual.

![Uma imagem da criação de um filtro com instruções OU no [!DNL Workfront]](assets/or-statement-5.png)

Observe que o Workfront “agrupou” as regras de filtro em cada lado da instrução OU (há uma caixa cinza ao redor delas). Isso instrui o Workfront a executar as regras em cada lado da instrução OU ao mesmo tempo, encontrando projetos que atendam a ambos os critérios, visto que estão unidos por uma instrução E.

Neste exemplo, o Workfront procura:

* Projetos que tenham seu nome no campo de proprietário e que também possuam o status Atual.
* **MAIS (OU)**
* Projetos criados por você que também possuam o status Atual.

Inserir a regra “Projetos com o status Atual” em cada lado da instrução OU garante que a regra funcione em conjunto com cada uma das outras regras. Essa regra comum às vezes é chamada de “constante”.

>[!NOTE]
>
>É possível utilizar mais de uma regra de filtro repetida em cada lado da instrução OU, dependendo de suas necessidades. No entanto, o Workfront recomenda usar o mínimo de regras repetidas possível, a fim de garantir que o filtro forneça os resultados desejados.

## O que acontece se a regra de filtro comum não for utilizada?

Sem as regras de filtro comum, não é possível obter os resultados de pesquisa esperados.

Por exemplo, se você inserir a regra “Projetos com o status Atual” apenas em um lado da instrução OU, ela funcionará somente com as regras de filtro dessa seção. Na imagem abaixo, é possível ver que a regra “Projetos com o status Atual” está apenas na seção superior.

![Uma imagem da criação de um filtro com instruções OU no [!DNL Workfront]](assets/or-statement-6.png)

Isso significa que o Workfront procurará:

* Projetos que têm seu nome no campo de proprietário e possuem o status Atual.
* **MAIS (OU)**
* Todos os projetos que você criou.

Como pode ver, esta configuração de filtro fornece resultados ligeiramente diferentes dos obtidos com a regra de filtro repetida. Por isso é importante se certificar de que o filtro esteja configurado corretamente para garantir os resultados desejados e necessários.

Pode ser que você não utilize instruções OU com frequência ao criar filtros. Porém, utilizar esse recurso pode ajudar a reduzir o número de filtros que você precisa criar. Apenas certifique-se de que seus filtros não retornem muitos resultados, já que uma lista longa pode dificultar que os usuários encontrem as informações exatas necessárias.

## Atividade de filtro OU

Você deseja encontrar tarefas incompletas atribuídas a você ou que não foram atribuídas a ninguém. Você configurou um filtro semelhante ao abaixo. Este filtro fornecerá os resultados desejados? Por que ou por que não?

![Uma imagem de uma instrução OU criada incorretamente no [!DNL Workfront]](assets/or-statement-your-turn-1.png)

### Respostas

Não, este filtro não fornecerá os resultados esperados (tarefas que não foram concluídas e que foram atribuídas a você ou não foram atribuídas a ninguém), porque a regra de filtro para o status da tarefa está apenas em um lado da instrução OU.

Em vez disso, esse filtro gerará uma lista que mostra:

* Tarefas atribuídas a você que possuem o status Em andamento ou Novo.
* **MAIS (OU)**
* Todas as tarefas não atribuídas, independentemente do status.

O filtro deve ser semelhante ao mostrado abaixo. Observe que este filtro possui a regra de filtragem para o status da tarefa em ambos os lados da instrução OU.

![Uma imagem de uma instrução OU criada corretamente no [!DNL Workfront]](assets/or-statement-your-turn-2.png)
