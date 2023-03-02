---
title: Criar relatórios com gráficos
description: Saiba como os gráficos podem melhorar a visualização de dados e como usar as ferramentas de gráfico no Workfront.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335153.png
kt: 8860
exl-id: ea3b360b-1fbd-4d1a-b505-b75759d24e41
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# Criar relatórios com gráficos

Neste vídeo, você aprenderá:

* Como os gráficos podem melhorar a visualização de dados
* Como usar as ferramentas de gráfico da Workfront

>[!VIDEO](https://video.tv.adobe.com/v/335155/?quality=12)

## Atividade: adicionar um gráfico a um relatório

O final do trimestre está se aproximando, e você quer ver como os projetos concluídos recentemente estão presos aos seus orçamentos. Crie um relatório que mostre o custo planejado versus o custo real dos projetos. Você deseja ver apenas os projetos que foram concluídos no último trimestre. Adicione um gráfico de colunas de combinação usando cores personalizadas.

## Resposta

1. Selecionar **[!UICONTROL Relatórios]** do **[!UICONTROL Menu principal]**.
1. Clique em **[!UICONTROL Novo Relatório]** e selecione **[!UICONTROL Projeto]**.
1. No **[!UICONTROL Colunas (Exibir)]** clique em **[!UICONTROL Adicionar coluna]**.
1. Selecionar [!UICONTROL Projeto] > [!UICONTROL Custo Planejado] e resumir essa coluna por **[!UICONTROL Sum]**.
1. Clique em **[!UICONTROL Adicionar coluna]** novamente.
1. Selecionar [!UICONTROL Projeto] > [!UICONTROL Custo Efetivo] e resumir essa coluna por **[!UICONTROL Sum]**.

   ![Uma imagem da tela para adicionar colunas a um relatório](assets/chart-report-columns.png)

1. No **[!UICONTROL Agrupamentos]** defina o relatório como agrupar por [!UICONTROL Projeto] > [!UICONTROL Nome].

   ![Uma imagem da tela para adicionar agrupamentos a um relatório](assets/chart-report-groupings.png)

1. No **[!UICONTROL Filtros]** adicione duas regras de filtro:

   * [!UICONTROL Projeto] > [!UICONTROL Status igual a] > [!UICONTROL Concluído]
   * [!UICONTROL Projeto] >[!UICONTROL  Data de término efetivo] > [!UICONTROL Trimestre passado]

   ![Uma imagem da tela para adicionar filtros a um relatório](assets/chart-report-filters.png)

1. No **[!UICONTROL Gráfico]** escolha **[!UICONTROL Coluna]** para o tipo de gráfico.
1. Para o [!UICONTROL Eixo esquerdo (Y)], escolha [!UICONTROL Projeto] > [!UICONTROL Custo Planejado].
1. Para o [!UICONTROL Eixo inferior (X)], escolha [!UICONTROL Projeto] > [!UICONTROL Nome].
1. Clique em **[!UICONTROL Gráfico Combinado]** e selecione [!UICONTROL Projeto] > [!UICONTROL Custo Efetivo] no **[!UICONTROL Valor]** campo.
1. Clique na seta ao lado da caixa de cores para alterar a [!UICONTROL Custo Efetivo] cor. Selecione uma das cores exibidas ou clique na caixa no canto inferior direito para exibir a paleta de cores.
1. Clique em **[!UICONTROL Salvar + Fechar]**. Quando solicitado a fornecer um nome de relatório, chame-o de &quot;Custo Planejado vs. Custo Efetivo por Projeto Concluído no Último Trimestre&quot;.

   ![Uma imagem da tela para adicionar um gráfico a um relatório](assets/chart-report-chart.png)
