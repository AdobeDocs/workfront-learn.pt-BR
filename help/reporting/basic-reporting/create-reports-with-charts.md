---
title: Criar relatórios com gráficos
description: Os gráficos aprimoram a visualização de dados organizando insights de dados por meio de filtros, agrupamentos e formatos de coluna empilhados personalizáveis, tornando a análise mais clara e acionável.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335153.png
jira: KT-8860
last-substantial-update: 2025-05-06T00:00:00Z
exl-id: ea3b360b-1fbd-4d1a-b505-b75759d24e41
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '596'
ht-degree: 39%

---

# Criar relatórios com gráficos

O vídeo explica como usar gráficos para visualizar dados de maneira eficaz, especialmente para rastrear tarefas do projeto. &#x200B; Ela demonstra a criação de dois tipos de relatórios no Workfront:

**Relatório de Tarefas Atrasadas por Projeto:**

* Comece com um relatório de lista e aplique filtros para mostrar somente tarefas atrasadas e incompletas nos projetos atuais. &#x200B;
* Agrupe tarefas por nome de projeto e crie um gráfico de pizza para visualizar a distribuição de tarefas atrasadas entre projetos. &#x200B;
* Defina o gráfico como a guia padrão para facilitar o acesso. &#x200B;

**Relatório de tarefas por projeto e status do progresso:**

* Copie o primeiro relatório e adicione outro agrupamento para o status de progresso da tarefa.
* Remova os filtros para incluir todas as tarefas, mostrando seu progresso durante a execução do projeto.
* Use um gráfico de colunas empilhadas para exibir o número total de tarefas por projeto, com pilhas representando diferentes status de progresso.
* Personalize as cores, se necessário, e salve o relatório.

O vídeo destaca como gráficos de pizza e de colunas empilhadas podem fornecer insights sobre a distribuição de tarefas e o desempenho do projeto, ajudando os usuários a comparar projetos e entender visualmente o progresso da tarefa. &#x200B;

>[!VIDEO]&#x200B;(https://video.tv.adobe.com/v/335155/?quality=12&learn=on&enablevpops=0)

## Principais conclusões

* **Gráficos para Melhorar a Clareza dos Dados**: a visualização de dados com gráficos, como gráficos de pizza ou de coluna, facilita a compreensão da distribuição de tarefas e do progresso do projeto em comparação aos relatórios de lista. &#x200B;
* **Filtragem para Insights Específicos**: a aplicação de filtros (por exemplo, tarefas incompletas e atrasadas em projetos atuais) ajuda a se concentrar em dados relevantes para análise direcionada. &#x200B;
* **Agrupamento para melhor organização**: o agrupamento de tarefas por nome de projeto ou status de progresso organiza os dados de maneira eficaz, permitindo comparações significativas entre projetos. &#x200B;
* **Opções de Personalização de Gráfico**: os usuários podem selecionar tipos de gráfico (por exemplo, pizza, coluna, barra) e personalizar cores para alinhá-las com preferências ou marcas. &#x200B;
* **Gráficos de colunas empilhadas para Insights Detalhados**: os gráficos de colunas empilhadas fornecem uma visão abrangente do progresso das tarefas nos projetos, mostrando o total de tarefas e seus status em uma única visualização.


## Atividades “Criar relatórios com gráficos”

### Atividade 1: adicionar um gráfico a um relatório

O final do trimestre está se aproximando e você talvez queira ver como os projetos concluídos recentemente cumpriram seus orçamentos. Crie um relatório que mostre o custo planejado em relação ao custo efetivo dos projetos. Consulte apenas os projetos que foram concluídos no último trimestre. Adicione um gráfico de colunas de combinação usando cores personalizadas.

### Resposta 1

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
   * [!UICONTROL Projeto] > [!UICONTROL &#x200B; Data efetiva de conclusão] > [!UICONTROL Último trimestre]

   ![Uma imagem da tela que permite adicionar filtros a um relatório](assets/chart-report-filters.png)

1. Na guia **[!UICONTROL Gráfico]**, escolha **[!UICONTROL Coluna]** como o tipo de gráfico.
1. Para o [!UICONTROL Eixo esquerdo (Y)], escolha [!UICONTROL Custo Planejado].
1. Para o [!UICONTROL Eixo Inferior (X)], escolha [!UICONTROL Nome].
1. Clique no botão **[!UICONTROL Gráfico de Combinação]** e selecione [!UICONTROL Custo Real] no campo **[!UICONTROL Valor]**.
1. No campo **[!UICONTROL Tipo de Gráfico]**, selecione Linha.
1. Clique na caixa de cores para alterar a cor [!UICONTROL Custo Efetivo]. Selecione uma cor.
1. Clique em **[!UICONTROL Salvar + Fechar]**. Quando for solicitado um nome de relatório, insira “Custo planejado comparado ao custo efetivo de projetos concluídos no último trimestre”.

   ![Uma imagem da tela que permite adicionar um gráfico a um relatório](assets/chart-report-chart.png)
