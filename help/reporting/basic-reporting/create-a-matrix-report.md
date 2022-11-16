---
title: Criar um relatório de matriz
description: Saiba quando um relatório de matriz pode ser útil e como criar um relatório de matriz no Workfront.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335156.png
kt: 8861
exl-id: e893d94a-e808-4bc1-bc6e-f46a5582b55d
source-git-commit: 252ba3ba44f22519a35899fcda9c6bca597a6c2c
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# Criar um relatório de matriz

Neste vídeo, você aprenderá:

* Quando um relatório de matriz pode ser útil
* E como criar um relatório de matriz

>[!VIDEO](https://video.tv.adobe.com/v/335156/?quality=12)

## Atividade: Criar um relatório de matriz

Crie um relatório de matriz que mostre quantas solicitações há em cada status, classificadas por fila de solicitações. Isso oferece um instantâneo rápido da quantidade de trabalho que está chegando e como você está acompanhando isso.

Você deseja que as filas de solicitação apareçam nos agrupamentos de linha. O status é exibido como os agrupamentos de colunas. Nomeie seu relatório como &quot;Solicitações por Status e Fila de Solicitações&quot;.

## Resposta

1. Selecionar **[!UICONTROL Relatórios]** do **[!UICONTROL Menu principal]**.
1. Clique no botão **[!UICONTROL Novo relatório]** e selecione **[!UICONTROL Problema]**.
1. Vá para o **[!UICONTROL Agrupamentos]** e clique em **[!UICONTROL Alternar para Agrupamento de Matriz]**.
1. Para [!UICONTROL Agrupamentos de linhas], selecione **[!UICONTROL Projeto]** > **[!UICONTROL Nome]**.
1. Para [!UICONTROL Agrupamento de colunas], selecione **[!UICONTROL Problema]** > **[!UICONTROL Status]**.

   ![Uma imagem da tela para criar um novo agrupamento de relatório de edição](assets/matrix-report-groupings.png)

1. Vá para o **[!UICONTROL Filtros]** guia .
1. Para garantir que você veja somente as solicitações nas filas de solicitação ativas, adicione as seguintes regras de filtro:

   * [!UICONTROL Projeto] > [!UICONTROL Status equivale a] > [!UICONTROL Igual] > [!UICONTROL Atual]
   * [!UICONTROL Definição de Fila] > [!UICONTROL É Público] > [!UICONTROL Diferente de] > [!UICONTROL Nenhum] (é assim que sabemos que um projeto é na verdade uma fila de solicitações, pelo fato de a Definição de fila estar atribuída a uma das opções públicas.)

1. Clique em **[!UICONTROL Salvar + Fechar]**. Quando solicitado para um nome de relatório, digite &quot;Solicitações por Status e Fila de Solicitações&quot;.

   ![Uma imagem da tela para criar um novo filtro de relatório de ocorrência](assets/matrix-report-filters.png)
