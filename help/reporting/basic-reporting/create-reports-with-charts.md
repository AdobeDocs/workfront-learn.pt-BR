---
title: Criar relatórios com gráficos
description: Saiba como os gráficos podem melhorar a visualização dos dados e como usar as ferramentas de gráfico no Workfront.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335153.png
kt: 8860
exl-id: ea3b360b-1fbd-4d1a-b505-b75759d24e41
source-git-commit: 252ba3ba44f22519a35899fcda9c6bca597a6c2c
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# Criar relatórios com gráficos

Neste vídeo, você aprenderá:

* Como os gráficos podem melhorar a visualização dos dados
* Como usar ferramentas de gráfico do Workfront

>[!VIDEO](https://video.tv.adobe.com/v/335155/?quality=12)

## Atividade: Adicionar um gráfico a um relatório

O final do trimestre está se aproximando e você quer ver como projetos concluídos recentemente ficaram presos aos seus orçamentos. Crie um relatório que mostre o custo planejado vs. o custo real dos projetos. Você deseja ver apenas os projetos que foram concluídos no último trimestre. Adicione um gráfico de colunas de combinação usando cores personalizadas.

## Resposta

1. Selecionar **[!UICONTROL Relatórios]** do **[!UICONTROL Menu principal]**.
1. Clique no botão **[!UICONTROL Novo relatório]** e selecione **[!UICONTROL Projeto]**.
1. No **[!UICONTROL Colunas (Exibir)]** clique em **[!UICONTROL Adicionar coluna]**.
1. Selecionar [!UICONTROL Projeto] > [!UICONTROL Custo Planejado] e resumir esta coluna por **[!UICONTROL Soma]**.
1. Clique em **[!UICONTROL Adicionar coluna]** novamente.
1. Selecionar [!UICONTROL Projeto] > [!UICONTROL Custo real] e resumir esta coluna por **[!UICONTROL Soma]**.

   ![Uma imagem da tela para adicionar colunas a um relatório](assets/chart-report-columns.png)

1. No **[!UICONTROL Agrupamentos]** , defina o relatório como agrupar por [!UICONTROL Projeto] > [!UICONTROL Nome].

   ![Uma imagem da tela para adicionar agrupamentos a um relatório](assets/chart-report-groupings.png)

1. No **[!UICONTROL Filtros]** adicione duas regras de filtro:

   * [!UICONTROL Projeto] > [!UICONTROL Status equivale a] > [!UICONTROL Concluído]
   * [!UICONTROL Projeto] >[!UICONTROL  Data de conclusão real] > [!UICONTROL Último trimestre]

   ![Uma imagem da tela para adicionar filtros a um relatório](assets/chart-report-filters.png)

1. No **[!UICONTROL Gráfico]** guia , escolha **[!UICONTROL Coluna]** para o tipo de gráfico.
1. Para o [!UICONTROL Eixo Esquerdo (Y)], escolha [!UICONTROL Projeto] > [!UICONTROL Custo Planejado].
1. Para o [!UICONTROL Eixo Inferior (X)], escolha [!UICONTROL Projeto] > [!UICONTROL Nome].
1. Clique no botão **[!UICONTROL Gráfico de Combinação]** e selecione [!UICONTROL Projeto] > [!UICONTROL Custo real] no **[!UICONTROL Valor]** campo.
1. Clique na seta ao lado da caixa de cor para alterar a [!UICONTROL Custo real] cor. Selecione uma das cores exibidas ou clique na caixa no canto inferior direito para exibir a paleta de cores.
1. Clique em **[!UICONTROL Salvar + Fechar]**. Quando solicitado a fornecer um nome de relatório, chame-o de &quot;Custo Planejado vs Custo Real por Projeto Concluído no Último Trimestre&quot;.

   ![Uma imagem da tela para adicionar um gráfico a um relatório](assets/chart-report-chart.png)
