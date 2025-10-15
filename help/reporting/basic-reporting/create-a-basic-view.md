---
title: Criar uma visualização básica
description: Aprenda o que é uma visualização e como criá-la e compartilhá-la com outros usuários no Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 335148.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
last-substantial-update: 2025-06-06T00:00:00Z
jira: KT-8854
exl-id: ba3c0e10-dcf1-4a7b-bf11-ccfed9040e6d
doc-type: video
source-git-commit: cc423944628d01e16d390842ecb25696505f923c
workflow-type: tm+mt
source-wordcount: '976'
ht-degree: 75%

---

# Criar uma visualização básica

O vídeo explica como criar e personalizar exibições no Workfront para exibir informações específicas sobre itens em uma lista, como projetos, tarefas, problemas e documentos. &#x200B; As exibições permitem que os usuários vejam detalhes como nome, descrição, status e outros campos relevantes para os itens. &#x200B;

O vídeo enfatiza a flexibilidade das visualizações no Workfront e fornece instruções passo a passo para criá-las, personalizá-las e gerenciá-las.

>[!VIDEO](https://video.tv.adobe.com/v/3450243/?captions=por_br&quality=12&learn=on&enablevpops=0)

## Principais conclusões

* **Personalizando Exibições**: os usuários podem editar exibições existentes ou criar novas adicionando, removendo ou reorganizando colunas para exibir informações específicas, como status ou orçamento do projeto.
* **Edição em linha**: alguns campos em uma exibição de lista podem ser atualizados diretamente sem abrir itens individuais, tornando mais rápido fazer alterações. &#x200B;
* **Criando Exibições do Zero**: os usuários podem criar exibições para atender a necessidades específicas, como rastrear a integridade do projeto, adicionando colunas relevantes como orçamento, custo real e status de progresso. &#x200B;
* **Compartilhamento e Gerenciamento de Exibições**: as exibições personalizadas podem ser compartilhadas com membros da equipe para colaboração ou removidas quando não forem mais necessárias.

## Atividades “Criar uma exibição básica”


### Atividade 1: criar uma visualização do status da tarefa

Como gerente de projeto, líder de equipe ou gerente de recursos, você deseja acompanhar o andamento das tarefas que estão sendo realizadas. Com essa visualização, você pode observar vários indicadores de status de uma tarefa em uma linha da lista ou do relatório.

Crie uma visualização de tarefas chamada “Visualização de status da tarefa” com as seguintes colunas:

* [!UICONTROL Nome da tarefa]
* [!UICONTROL Atribuições]
* [!UICONTROL Duração]
* [!UICONTROL Percentual concluído]
* [!UICONTROL Status]
* [!UICONTROL Status do Progresso]
* [!UICONTROL Ícones de Status]

### Resposta 1

![Uma imagem da tela de criação de uma visualização do status da tarefa](assets/view-exercise.png)

1. Em um relatório de lista de tarefas, acesse o menu suspenso **[!UICONTROL Visualização]** e selecione **[!UICONTROL Nova visualização]**.
1. Nomeie sua visualização como “Visualização do status da tarefa”.
1. Remova estas colunas: [!UICONTROL Horas planejadas], [!UICONTROL Predecessores], [!UICONTROL Data de início] e [!UICONTROL Data de expiração]. 
1. Clique em **[!UICONTROL Adicionar coluna]**.
1. No campo [!UICONTROL Exibir nesta coluna], digite “status” e selecione a opção “Status” na origem do campo [!UICONTROL Tarefa].
1. Clique em **[!UICONTROL Adicionar coluna]** novamente.
1. No campo [!UICONTROL Exibir nesta coluna], digite “status” e selecione a opção “Status do progresso” na origem do campo [!UICONTROL Tarefa].
1. Clique em **[!UICONTROL Adicionar coluna]** novamente.
1. No campo [!UICONTROL Exibir nesta coluna], digite “status” e selecione “Ícones de status” na origem do campo Tarefa.
1. Clique em **[!UICONTROL Salvar]**.

Passe o mouse sobre cada um dos ícones na coluna [!UICONTROL Ícones de status] para ver o que eles representam. Se estiverem esmaecidos, significa que a tarefa não tem notas, documentos, processos de aprovação etc. Se um ícone aparecer em cores, há pelo menos um desse item associado à tarefa. Você pode clicar nos ícones da nota ou do documento para acessá-los.

### Atividade 2: criar uma visualização de marcos

Se você usa marcos, essa exibição é a maneira mais fácil de ver marcos por nome na lista de tarefas e adicioná-los ou removê-los de uma tarefa usando a edição em linha.

Crie uma visualização de tarefas chamada “Visualização de marcos” com as seguintes colunas:

* [!UICONTROL Nome da tarefa]
* [!UICONTROL Atribuições]
* [!UICONTROL Duração]
* [!UICONTROL Horas planejadas]
* [!UICONTROL Marco: nome]
* [!UICONTROL Início em]
* [!UICONTROL Concluir em]
* [!UICONTROL Percentual concluído]


### Resposta 2

![Uma imagem da tela de criação de uma visualização de marco](assets/view-milestone-exercise-1.png)

1. Em uma lista de tarefas do projeto, acesse o menu suspenso **[!UICONTROL Visualização]** e selecione **[!UICONTROL Nova visualização]**.
1. Nomeie sua visualização como “Visualização de marco”.
1. Clique na coluna [!UICONTROL Predecessores] para selecioná-la.
1. No campo [!UICONTROL Mostrar nesta coluna], clique no ícone &quot;menos&quot; no campo [!UICONTROL Tarefa >> Predecessoras], digite &quot;[!UICONTROL nome da etapa]&quot; e clique no &quot;[!UICONTROL Nome]&quot; na lista.
1. Clique em **[!UICONTROL Salvar]**.

![Uma imagem de uma lista de tarefas usando uma visualização de marcos](assets/view-milestone-exercise-2.png)

### Atividade 3: criar uma visualização de tipos de duração e restrições de tarefas

Essa visualização permitirá examinar e editar todos os tipos de duração e restrições de tarefa no projeto.

Crie uma visualização de tarefas chamada “Visualização de tipos de duração e restrições de tarefas” com as seguintes colunas:

* [!UICONTROL Nome da tarefa]
* [!UICONTROL Atribuições]
* [!UICONTROL Duração]
* [!UICONTROL Duração Planejada]
* [!UICONTROL Horas planejadas]
* [!UICONTROL Predecessoras]
* [!UICONTROL Início em]
* [!UICONTROL Concluir em]
* [!UICONTROL Tipo de Duração]
* [!UICONTROL Restrição de Tarefa]
* [!UICONTROL Data de Restrição]

Mude o [!UICONTROL Formato do campo] nas colunas [!UICONTROL Data de início] e [!UICONTROL Data de expiração] para exibir a data e a hora.

### Resposta 3

![Uma imagem da tela mostrando a visualização dos tipos de duração e as restrições da tarefa](assets/view-activity-3.png)

1. Em uma lista de tarefas do projeto, acesse o menu suspenso **[!UICONTROL Visualização]** e selecione **[!UICONTROL Nova visualização]**.
1. Nomeie sua visualização como “Visualização de tipos de duração e restrições de tarefa”.
1. Remova a coluna [!UICONTROL % concluído].
1. Clique em **[!UICONTROL Adicionar coluna]**.
1. No campo [!UICONTROL Exibir nesta coluna], digite [!UICONTROL “duração”] e selecione [!UICONTROL “Duração planejada”] na origem do campo [!UICONTROL Tarefa].
1. Mova esta coluna entre as colunas [!UICONTROL Duração] e [!UICONTROL Horas planejadas].
1. Clique em **[!UICONTROL Adicionar coluna]** novamente.
1. No campo [!UICONTROL Exibir nesta coluna], digite [!UICONTROL “tipo de duração”] e selecione [!UICONTROL “Tipo de duração”] na origem do campo [!UICONTROL Tarefa].
1. Clique em **[!UICONTROL Adicionar coluna]** novamente.
1. No campo [!UICONTROL Exibir nesta coluna], digite [!UICONTROL “restrição”] e selecione [!UICONTROL “Restrição de tarefa”] na origem do campo Tarefa.
1. Clique em **[!UICONTROL Adicionar coluna]** novamente.
1. No campo [!UICONTROL Exibir nesta coluna], digite [!UICONTROL “restrição”] e selecione [!UICONTROL “Data da restrição”] na origem do campo Tarefa.
1. Selecione a coluna [!UICONTROL Data de início] e clique em [!UICONTROL Opções avançadas].
1. Na lista suspensa [!UICONTROL Formato do Campo], selecione [!UICONTROL &quot;10/17/60 3:00 AM&quot;].
1. Selecione a coluna [!UICONTROL Data de expiração] e clique em [!UICONTROL Opções avançadas].
1. Na lista suspensa [!UICONTROL Formato do Campo], selecione [!UICONTROL &quot;10/17/60 3:00 AM&quot;].
1. Clique em **[!UICONTROL Salvar]**.

### Atividade 4: criar uma exibição do status ativo do modelo de projeto

Qualquer pessoa que gerencia modelos de projeto aprecia a possibilidade de ver o status ativo (verdadeiro ou falso) de cada modelo em uma lista. E algo ainda melhor é poder editar os campos em linha.

Crie uma exibição de modelo de projeto chamada “Padrão + status ativo” com as seguintes colunas:

* [!UICONTROL Nome]
* [!UICONTROL Proprietário]
* [!UICONTROL Duração]
* [!UICONTROL Horas planejadas]
* [!UICONTROL Custo planejado]
* [!UICONTROL Sinalizadores]
* [!UICONTROL Nome do grupo]
* [!UICONTROL Está ativo]


### Resposta 4

![Uma imagem da tela que mostra o status ativo de um modelo de projeto](assets/view-activity-4.png)

1. Em uma lista de modelos de projeto, acesse o menu suspenso **[!UICONTROL Visualização]** e selecione **[!UICONTROL Nova visualização]**.
1. Nomeie sua visualização como “Padrão + status ativo”.
1. Clique em **[!UICONTROL Adicionar coluna]**.
1. No campo [!UICONTROL Exibir nesta coluna], digite “está” e selecione “Está ativo” na origem do campo [!UICONTROL Modelo].
1. Clique em **[!UICONTROL Salvar visualização]**.
