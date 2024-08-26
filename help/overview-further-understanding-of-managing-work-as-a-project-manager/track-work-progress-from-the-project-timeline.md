---
title: Acompanhe o progresso da linha do tempo do projeto
description: Saiba como acompanhar o progresso do trabalho na linha do tempo do projeto no [!DNL  Workfront] usando Percentual concluído, Status, Atribuições ou Restrições.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: track-work-progress-from-the-project-timeline.jpeg
type: Tutorial
role: User
last-substantial-update: 2023-08-16T00:00:00Z
level: Beginner
jira: KT-10150
hide: true
source-git-commit: 2351b6ff9977fd8a81289ab2fad28e21322d347e
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Acompanhe o progresso da linha do tempo do projeto

Certifique-se de que as tarefas estejam progredindo da maneira esperada para atender aos prazos do projeto. À medida que você examina a lista de [!UICONTROL Tarefa], existem vários recursos no [!DNL  Workfront] que ajudam você a monitorar o progresso e o status do trabalho.

## Percentual completo

Às vezes, o percentual concluído em cada tarefa de trabalho é usado para avaliar o progresso do trabalho. É importante observar que este campo deve ser ajustado manualmente, pois é a estimativa do cessionário quanto ao progresso alcançado.

>[!TIP]
>
>Embora o pecentual concluído em tarefas de trabalho precise ser atualizado manualmente, no caso da tarefa principal ele é calculado pelo Workfront com base no percentual concluído e na duração ou nas horas planejadas de cada tarefa derivada. Isso significa que você obterá melhor precisão do percentual concluído se dividir tarefas grandes em subtarefas menores.


![Lista de tarefas do projeto mostrando a coluna [!UICONTROL Percentual concluído] ](assets/planner-fund-task-percent-complete.png)

Há três momentos em que o percentual concluído muda automaticamente

* Quando o [!UICONTROL Status] da tarefa estiver definido como Concluído, o percentual concluído será alterado para 100.
* Se o [!UICONTROL Status] da tarefa voltar para Novo, o percentual concluído é redefinido para 0.
* Em uma tarefa principal, quando o percentual concluído de uma tarefa derivada é alterada.

## Status

Inclua a coluna [!UICONTROL Status] em uma [!UICONTROL Visualização] para ver rapidamente quais tarefas foram iniciadas, quais estão em andamento e quais estão concluídas. Você pode até configurar a formatação condicional em uma [!UICONTROL Visualização] para codificar cada status com cores, tornando as informações mais fáceis de decifrar.

## Atribuições de tarefas

Ao revisar o projeto, revise as atribuições de tarefas. Talvez o trabalho tenha atrasado porque ninguém foi atribuído à tarefa. Ou talvez a pessoa atribuída não tivesse as habilidades certas para concluir o trabalho. Adicione mais pessoas a uma tarefa ou reatribua tarefas para garantir que o trabalho seja concluído.

## Restrição da tarefa

Às vezes, as restrições das tarefas mudam e você não percebe. As restrições podem afetar o comportamento da sua linha do tempo, portanto, certifique-se de que elas estejam definidas como você deseja.

![Lista de tarefas do projeto mostrando a coluna Restrição da tarefa](assets/planner-fund-task-constraint.png)

Crie uma Exibição personalizada que inclua a coluna [!UICONTROL Restrição da tarefa] para ver essas informações em sua lista de tarefas. Se você planejou o projeto a partir de uma data de início, você deseja que suas tarefas tenham a restrição [!UICONTROL O mais breve possível] ([!UICONTROL ASAP]).

Para obter mais detalhes sobre restrições de tarefas, consulte [Compreenda e gerencie tipos de duração e restrições de tarefas](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/intermediate-projects/understand-and-manage-duration-types-and-task-constraints.html?lang=pt-BR).
