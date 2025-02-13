---
title: Criar relatórios com atividades de gráficos
description: Pratique a criação de relatórios com gráficos, com instruções passo a passo.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335153.png
jira: KT-8860
hidefromtoc: true
source-git-commit: 915b28bbbf138fa84dce6d1915387fbe22c63362
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 81%

---

# Criar relatórios com atividades de gráficos

Pratique a criação de relatórios com gráficos, com instruções passo a passo.

## Atividade 1: adicionar um gráfico a um relatório

O final do trimestre está se aproximando e você talvez queira ver como os projetos concluídos recentemente cumpriram seus orçamentos. Crie um relatório que mostre o custo planejado em relação ao custo efetivo dos projetos. Consulte apenas os projetos que foram concluídos no último trimestre. Adicione um gráfico de colunas de combinação usando cores personalizadas.

## Resposta 1

1. Selecione **[!UICONTROL Relatórios]** no **[!UICONTROL Menu principal]**.
1. Clique no menu **[!UICONTROL Novo relatório]** e selecione **[!UICONTROL Projeto]**.
1. Na guia **[!UICONTROL Colunas (visualização)]**, clique em **[!UICONTROL Adicionar coluna]**.
1. Selecione [!UICONTROL Projeto] > [!UICONTROL Custo planejado] e resuma esta coluna pela **[!UICONTROL Soma]**.
1. Clique em **[!UICONTROL Adicionar coluna]** novamente.
1. Selecione [!UICONTROL Projeto] > [!UICONTROL Custo efetivo] e resuma esta coluna pela **[!UICONTROL Soma]**.

   ![Uma imagem da tela que permite adicionar colunas a um relatório](assets/chart-report-columns.png)

1. Na guia **[!UICONTROL Agrupamentos]**, agrupe o relatório por [!UICONTROL Projeto] > [!UICONTROL Nome].

   ![Uma imagem da tela que permite adicionar agrupamentos a um relatório](assets/chart-report-groupings.png)

1. Na guia **[!UICONTROL Filtros]**, adicione duas regras de filtro:

   * [!UICONTROL Projeto] > [!UICONTROL Status igual a] > [!UICONTROL Concluído]
   * [!UICONTROL Projeto] > [!UICONTROL  Data efetiva de conclusão] > [!UICONTROL Último trimestre]

   ![Uma imagem da tela que permite adicionar filtros a um relatório](assets/chart-report-filters.png)

1. Na guia **[!UICONTROL Gráfico]**, escolha **[!UICONTROL Coluna]** como o tipo de gráfico.
1. Para o [!UICONTROL Eixo esquerdo (Y)], escolha [!UICONTROL Projeto] > [!UICONTROL Custo planejado].
1. Para o [!UICONTROL Eixo inferior (X)], escolha [!UICONTROL Projeto] > [!UICONTROL Nome].
1. Clique no botão **[!UICONTROL Gráfico de combinação]** e selecione [!UICONTROL Projeto] > [!UICONTROL Custo efetivo] no campo **[!UICONTROL Valor]**.
1. Clique na seta ao lado da caixa de cores para alterar a cor do [!UICONTROL Custo efetivo]. Selecione uma das cores que aparece ou clique na caixa no canto inferior direito para abrir a paleta de cores.
1. Clique em **[!UICONTROL Salvar + Fechar]**. Quando solicitado a fornecer um nome de relatório, chame-o de &quot;Custo Planejado vs. Custo Efetivo por Projeto Concluído no Último Trimestre&quot;.

   ![Uma imagem da tela que permite adicionar um gráfico a um relatório](assets/chart-report-chart.png)
