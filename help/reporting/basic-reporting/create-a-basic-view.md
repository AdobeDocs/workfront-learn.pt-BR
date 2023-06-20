---
title: Criar uma exibição básica
description: Saiba o que é uma visualização, como criá-la e como compartilhá-la com outros usuários no Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 335148.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
last-substantial-update: 2023-06-20T00:00:00Z
kt: 8854
exl-id: ba3c0e10-dcf1-4a7b-bf11-ccfed9040e6d
doc-type: video
source-git-commit: f7e6fa6a728699c307fbba926d1bdaa697ba4894
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 6%

---

# Criar uma exibição básica

Neste vídeo, você aprenderá:

* O que é uma visualização no Workfront
* Como criar e modificar uma visualização
* Como compartilhar uma visualização com outros usuários do Workfront

>[!VIDEO](https://video.tv.adobe.com/v/335148/?quality=12&learn=on)

## Atividade 1: criar uma exibição de status de tarefa

Como gerente de projeto, líder de equipe ou gerente de recursos, você deseja acompanhar o andamento do trabalho da tarefa. Com essa visualização, você obtém vários indicadores de status de uma tarefa em uma linha da lista ou do relatório.

Crie uma exibição de tarefa chamada &quot;Exibição do status da tarefa&quot; com as seguintes colunas:

* [!UICONTROL Nome da tarefa]
* [!UICONTROL Atribuições]
* [!UICONTROL Duração]
* [!UICONTROL Percentual concluído]
* [!UICONTROL Status]
* [!UICONTROL Progresso - Status de Progresso]
* [!UICONTROL Ícones de Status]

## Resposta da Atividade 1

![Uma imagem da tela para criar uma exibição de status de tarefa](assets/view-exercise.png)

1. Em um relatório de lista de tarefas, vá para a **[!UICONTROL Exibir]** e selecione **[!UICONTROL Nova visualização]**.
1. Nomeie sua exibição como &quot;Exibição do status da tarefa&quot;.
1. Remover estas colunas: [!UICONTROL Horas planejadas], [!UICONTROL Predecessores], [!UICONTROL Início em], e [!UICONTROL Prazo final].
1. Clique em **[!UICONTROL Adicionar coluna]**.
1. No [!UICONTROL Mostrar nesta coluna] digite &quot;status&quot; e selecione &quot;Status&quot; na caixa suspensa [!UICONTROL Tarefa] origem do campo.
1. Clique em **[!UICONTROL Adicionar coluna]** novamente.
1. No [!UICONTROL Mostrar nesta coluna] digite &quot;status&quot; e selecione &quot;Status do progresso&quot; na caixa [!UICONTROL Tarefa] origem do campo.
1. Clique em **[!UICONTROL Adicionar coluna]** novamente.
1. No [!UICONTROL Mostrar nesta coluna] digite &quot;status&quot; e depois selecione &quot;Ícones de Status&quot; na origem do campo Tarefa.
1. Clique em **[!UICONTROL Salvar]**.

Passe o mouse sobre cada um dos ícones no [!UICONTROL Ícones de Status] para ver o que eles representam. Se estiverem esmaecidos, significa que a tarefa não tem notas, documentos, processos de aprovação etc. Se um ícone for exibido em cores, há pelo menos um desse item associado à tarefa. Você pode clicar nos ícones de nota ou documento para ir para esse item.

## Atividade 2: criar uma visualização de etapa

Se você usa marcos, essa exibição é a maneira mais fácil de ver marcos por nome e adicioná-los ou editá-los usando a edição em linha.

Crie uma visualização de tarefa chamada &quot;Visualização de marco&quot; com as seguintes colunas:

* [!UICONTROL Nome da tarefa]
* [!UICONTROL Atribuições]
* [!UICONTROL Duração]
* [!UICONTROL Horas planejadas]
* [!UICONTROL Etapa: Nome]
* [!UICONTROL Início em]
* [!UICONTROL Concluir em]
* [!UICONTROL Percentual concluído]


## Resposta da Atividade 2

![Uma imagem da tela para criar uma visualização de marco](assets/view-milestone-exercise-1.png)

1. Em uma lista de tarefas de projeto, vá para a **[!UICONTROL Exibir]** e selecione **[!UICONTROL Nova visualização]**.
1. Nomeie sua visualização como &quot;Visualização de marco&quot;.
1. Clique no link [!UICONTROL Predecessores] para selecioná-la.
1. No [!UICONTROL Mostrar nesta coluna] clique no ícone X na caixa [!UICONTROL Tarefa >> Predecessoras] e digite &quot;[!UICONTROL nome da etapa]&quot; e clique em &quot;[!UICONTROL Nome]&quot; na lista.
1. Clique em **[!UICONTROL Salvar]**.

![Imagem de uma lista de tarefas usando uma exibição de marco](assets/view-milestone-exercise-2.png)
