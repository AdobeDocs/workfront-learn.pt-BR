---
title: Criar atividades de relatório de matriz
description: Pratique a criação de relatórios de matriz, com instruções passo a passo.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335156.png
jira: KT-8861
hidefromtoc: true
source-git-commit: 915b28bbbf138fa84dce6d1915387fbe22c63362
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 66%

---

# Criar atividades de relatório de matriz

Pratique a criação de relatórios de matriz, com instruções passo a passo.

## Atividade 1: criar um relatório de matriz

Crie um relatório matriz que mostre quantas solicitações existem em cada status, classificadas pela fila de solicitações. Isso lhe dá uma ideia rápida da quantidade de trabalho que está chegando e como você está se mantendo atualizado.

As filas de solicitações devem aparecer nos agrupamentos de linhas. O status aparece nos agrupamentos de colunas. Nomeie seu relatório como &quot;Solicitações por status e por fila de solicitações&quot;.

## Resposta 1

1. Selecione **[!UICONTROL Relatórios]** no **[!UICONTROL Menu principal]**.
1. Clique na opção **[!UICONTROL Novo relatório]** e selecione **[!UICONTROL Problema]**.
1. Acesse a guia **[!UICONTROL Agrupamentos]** e clique em **[!UICONTROL Alternar para o agrupamento matriz]**.
1. Em [!UICONTROL Agrupamentos de linhas], selecione **[!UICONTROL Projeto]** > **[!UICONTROL Nome]**.
1. Em [!UICONTROL Agrupamento de colunas], selecione **[!UICONTROL Problema]** > **[!UICONTROL Status]**.

   ![Uma imagem da tela de criação de um novo agrupamento de relatórios de problemas](assets/matrix-report-groupings.png)

1. Acesse a guia **[!UICONTROL Filtros]**.
1. Para garantir que sejam exibidas somente solicitações em filas ativas, adicione as seguintes regras de filtro:

   * [!UICONTROL Projeto] > [!UICONTROL Status igual a] > [!UICONTROL Igual] > [!UICONTROL Atual]
   * [!UICONTROL Definição da fila] > [!UICONTROL É público] > [!UICONTROL Não é igual] > [!UICONTROL Nenhum] (é assim que sabemos que um projeto é, na verdade, uma fila de solicitações, quando a Definição de fila é atribuída a uma das opções públicas.)

1. Clique em **[!UICONTROL Salvar e Fechar]**. Quando solicitado a fornecer um nome de relatório, digite &quot;Solicitações por status e Fila de solicitações&quot;.

   ![Uma imagem da tela de criação de um novo filtro de relatórios de problemas](assets/matrix-report-filters.png)
