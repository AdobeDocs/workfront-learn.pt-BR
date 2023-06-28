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
jira: KT-8861
exl-id: e893d94a-e808-4bc1-bc6e-f46a5582b55d
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# Criar um relatório de matriz

Neste vídeo, você aprenderá:

* Quando um relatório de matriz pode ser útil
* E como criar um relatório de matriz

>[!VIDEO](https://video.tv.adobe.com/v/335156/?quality=12&learn=on)

## Atividade: criar um relatório de matriz

Crie um relatório de matriz que mostre quantas solicitações há em cada status, classificadas por fila de solicitações. Isso oferece uma visão rápida da quantidade de trabalho que está chegando e do quão bem você está acompanhando.

Você deseja que as filas de solicitações apareçam nos agrupamentos de linhas. Status aparece como os agrupamentos de coluna. Nomeie seu relatório como &quot;Solicitações por status e por fila de solicitações&quot;.

## Resposta

1. Selecionar **[!UICONTROL Relatórios]** do **[!UICONTROL Menu principal]**.
1. Clique em **[!UICONTROL Novo Relatório]** e selecione **[!UICONTROL Problema]**.
1. Vá para a **[!UICONTROL Agrupamentos]** e clique em **[!UICONTROL Alternar para agrupamento de matriz]**.
1. Para [!UICONTROL Agrupamentos de linhas], selecione **[!UICONTROL Projeto]** > **[!UICONTROL Nome]**.
1. Para [!UICONTROL Agrupamento de colunas], selecione **[!UICONTROL Problema]** > **[!UICONTROL Status]**.

   ![Uma imagem da tela para criar um novo agrupamento de relatório de problemas](assets/matrix-report-groupings.png)

1. Vá para a **[!UICONTROL Filtros]** guia.
1. Para garantir que você veja somente solicitações em filas de solicitações ativas, adicione as seguintes regras de filtro:

   * [!UICONTROL Projeto] > [!UICONTROL Status igual a] > [!UICONTROL Igual] > [!UICONTROL Atual]
   * [!UICONTROL Definição da fila] > [!UICONTROL É público] > [!UICONTROL Não Igual] > [!UICONTROL Nenhum] (é assim que sabemos que um projeto é, na verdade, uma fila de solicitações, pela Definição de fila sendo atribuída a uma das opções públicas.)

1. Clique em **[!UICONTROL Salvar + Fechar]**. Quando solicitado a fornecer um nome de relatório, digite &quot;Solicitações por status e Fila de solicitações&quot;.

   ![Uma imagem da tela para criar um novo filtro de relatório de problemas](assets/matrix-report-filters.png)
