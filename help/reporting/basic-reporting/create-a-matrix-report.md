---
title: Criar um relatório matriz
description: Saiba quando um relatório matriz pode ser útil e como criá-lo no Workfront.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335156.png
jira: KT-8861
exl-id: e893d94a-e808-4bc1-bc6e-f46a5582b55d
doc-type: video
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 100%

---

# Criar um relatório matriz

Neste vídeo, você aprenderá:

* Quando um relatório matriz pode ser útil
* E como criar um relatório matriz

>[!VIDEO](https://video.tv.adobe.com/v/335156/?quality=12&learn=on&enablevpops)

## Atividade: criar um relatório matriz

Crie um relatório matriz que mostre quantas solicitações existem em cada status, classificadas pela fila de solicitações. Isso oferece uma visão rápida da quantidade de trabalho que está chegando e de como você está lidando com ele.

As filas de solicitações devem aparecer nos agrupamentos de linhas. O status aparece nos agrupamentos de colunas. Nomeie seu relatório como “Solicitações por status e por fila de solicitações”.

## Responder

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

1. Clique em **[!UICONTROL Salvar e Fechar]**. Quando solicitado a fornecer um nome de relatório, digite “Solicitações por status e fila de solicitações”.

   ![Uma imagem da tela de criação de um novo filtro de relatórios de problemas](assets/matrix-report-filters.png)
