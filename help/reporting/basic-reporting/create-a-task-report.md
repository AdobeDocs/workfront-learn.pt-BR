---
title: Criar um relatório de tarefas
description: Saiba como criar um relatório de tarefas com um filtro complexo e encontrar os relatórios que você cria no Workfront. Atividade - crie um relatório de observações com prompts.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335154.png
jira: KT-8859
exl-id: 90bad2e8-9cd2-4ae7-973b-eeab9d615bef
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 11%

---

# Criar um relatório de tarefas

Neste vídeo, você aprenderá:

* Como criar um relatório de tarefas com um filtro complexo
* Como localizar os relatórios que você cria

>[!VIDEO](https://video.tv.adobe.com/v/335154/?quality=12&learn=on)

## Atividade: criar um relatório de observações com prompts

Crie um relatório de Notas que pode ser usado para procurar notas do usuário (ou seja, comentários ou atualizações) ou notas do sistema com base no conteúdo da nota, no autor, na data de entrada, no nome do projeto ou no tipo de auditoria. Nomeie o relatório como &quot;Pesquisa de notas&quot;.

Ao usar o prompt de Texto de observação, este relatório pesquisará em threads de atualização para extrair rapidamente qualquer item que atenda aos critérios especificados nos prompts. Ao executar o relatório, não é necessário preencher todos os prompts, apenas aqueles com os quais você se importa. Os em branco são automaticamente ignorados.

A exibição deve incluir colunas para:

* Texto da Nota
* Texto de Auditoria
* Data de Entrada
* Proprietário: Nome
* Tipo de Auditoria
* Nome da tarefa
* Nome do Problema

Deixe a guia do filtro em branco.

Agrupar no Nome do Projeto.

Incluir prompts para o seguinte:

* Texto de Auditoria
* Texto da Nota
* Nome do proprietário
* Data de Entrada
* Nome do Projeto
* Tipo de Auditoria

## Resposta

1. Selecionar **[!UICONTROL Relatórios]** do **[!UICONTROL Menu principal]**.
1. Clique em **[!UICONTROL Novo Relatório]** e selecione **[!UICONTROL Nota]**.
1. Entrada **[!UICONTROL Colunas (Exibir)]** configure suas colunas para incluir:

   ![Uma imagem da tela para criar colunas de relatório de anotações](assets/note-report-columns.png)

   * [!UICONTROL Nota] > [!UICONTROL Texto da Nota]
   * [!UICONTROL Nota] > [!UICONTROL Texto de auditoria]
   * [!UICONTROL Nota] > [!UICONTROL Data de entrada]
   * [!UICONTROL Proprietário] > [!UICONTROL Nome]
   * [!UICONTROL Nota] > [!UICONTROL Tipo de Auditoria]
   * [!UICONTROL Tarefa] > [!UICONTROL Nome]
   * [!UICONTROL Problema] > [!UICONTROL Nome]

1. Selecione o **[!UICONTROL Data de entrada]** e altere a variável **[!UICONTROL Classificar em ordem decrescente]**.
1. No **[!UICONTROL Agrupamentos]** defina o relatório como agrupar por [!UICONTROL Projeto] > [!UICONTROL Nome].

   ![Uma imagem da tela para criar agrupamentos de relatórios de anotações](assets/note-report-groupings.png)

1. Sair [!UICONTROL Filtros] em branco.
1. Abertura **[!UICONTROL Configurações do relatório]** e nomeie o relatório como &quot;Pesquisa de Notas&quot;.
1. No [!UICONTROL Descrição] , coloque algo como, &quot;Procure por notas do sistema ou do usuário com base no Tipo de auditoria selecionado e em outros prompts. As notas do sistema são exibidas na coluna Texto de auditoria e as notas do usuário são exibidas na coluna Texto de nota.&quot;

   ![Uma imagem da tela para criar configurações de relatório de anotações](assets/note-report-report-options.png)

1. Selecionar **[!UICONTROL Guia Detalhes]** para que seja exibido quando o relatório for carregado.
1. Defina o relatório para mostrar 200 itens quando ele for incluído em um painel.
1. Clique em **[!UICONTROL Prompts do relatório]** e adicione:

   ![Uma imagem da tela para criar avisos de relatórios](assets/note-report-report-prompts.png)

   * [!UICONTROL Nota] > [!UICONTROL Texto de auditoria]
   * [!UICONTROL Nota] > [!UICONTROL Texto da Nota]
   * [!UICONTROL Proprietário] > [!UICONTROL Nome]
   * [!UICONTROL Nota] > [!UICONTROL Data de entrada]
   * [!UICONTROL Projeto] > [!UICONTROL Nome]
   * [!UICONTROL Nota] > [!UICONTROL Tipo de Auditoria]

1. Marque a caixa para **[!UICONTROL Mostrar solicitações nos painéis]**.
1. Salve e feche o relatório.
