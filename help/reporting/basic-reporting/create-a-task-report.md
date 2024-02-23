---
title: Crie um relatório de tarefas
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
source-git-commit: 5fa3bbf2fb4763e63beeb7ac640cc93ccf54fed5
workflow-type: ht
source-wordcount: '922'
ht-degree: 100%

---

# Crie um relatório de tarefas

Neste vídeo, você aprenderá:

* Como criar um relatório de tarefas com um filtro complexo
* Como localizar os relatórios que você cria

>[!VIDEO](https://video.tv.adobe.com/v/335154/?quality=12&learn=on)



>[!TIP]
>
>Pegue suas espátulas e tigelas e prepare-se para experimentar as “receitas” em nosso [Livro de receitas de relatórios do cliente do Adobe Workfront](/help/assets/workfront-customer-reporting-cookbook.pdf). Lá dentro, você encontrará instruções passo a passo para 10 relatórios, prontos para você preparar em seu ambiente hoje mesmo.
>Reunimos os relatórios favoritos dos clientes e os compilamos em um livro de receitas rápidas e de fácil digestão, para você levá-las e testá-las em sua própria cozinha do Workfront.
>Esses 10 relatórios vêm de clientes que são exatamente como você. Espalhados por setores, departamentos, equipes, posições e todos em diferentes empresas, devemos um enorme agradecimento aos incríveis clientes que compartilharam um de seus relatórios favoritos. Alguns relatórios são simples (mas incrivelmente úteis), e outros são mais complexos para elevar o nível dos seus relatórios.



## Atividade 1: criar um relatório de notas com solicitações

Crie um relatório de notas que você pode usar para pesquisar notas do usuário (ou seja, comentários ou atualizações) ou notas do sistema com base no conteúdo da nota, no autor, na data de entrada, no nome do projeto ou no tipo de auditoria. Nomeie o relatório como “Pesquisa de notas”.

Ao usar o prompt de texto da nota, este relatório pesquisará nas threads de atualização para extrair rapidamente qualquer um que atenda aos critérios especificados nos prompts. Ao executar o relatório, você não precisa preencher todas as solicitações, apenas as de seu interesse. Os que estão branco são automaticamente ignorados.

A visualização deve incluir colunas para:

* Texto da Nota
* Texto de Auditoria
* Data de Entrada
* Proprietário: nome
* Tipo de Auditoria
* Nome da tarefa
* Nome do Problema

Deixe a guia do filtro em branco.

Grupo no nome do projeto.

Inclua prompts para o seguinte:

* Texto de Auditoria
* Texto da Nota
* Nome do proprietário
* Data de Entrada
* Nome do Projeto
* Tipo de Auditoria

## Resposta da atividade 1

1. Selecione **[!UICONTROL Relatórios]** no **[!UICONTROL Menu principal]**.
1. Clique no menu **[!UICONTROL Novo relatório]** e selecione **[!UICONTROL Nota]**.
1. Em **[!UICONTROL Colunas (Visualização)]** configure as colunas para incluir:

   ![Uma imagem da tela para criar colunas de relatório de notas](assets/note-report-columns.png)

   * [!UICONTROL Nota] > [!UICONTROL Texto da Nota]
   * [!UICONTROL Nota] > [!UICONTROL Texto de auditoria]
   * [!UICONTROL Nota] > [!UICONTROL Data de entrada]
   * [!UICONTROL Proprietário] > [!UICONTROL Nome]
   * [!UICONTROL Nota] > [!UICONTROL  Tipo de auditoria]
   * [!UICONTROL Tarefa] > [!UICONTROL Nome]
   * [!UICONTROL Problema] > [!UICONTROL Nome]

1. Selecione a coluna **[!UICONTROL Data de entrada]** e altere **[!UICONTROL Classificar para decrescente]**.
1. Na guia **[!UICONTROL Agrupamentos]**, configure o relatório para agrupar por [!UICONTROL Projeto] > [!UICONTROL Nome].

   ![Uma imagem da tela para criar agrupamentos de relatórios de notas](assets/note-report-groupings.png)

1. Deixe [!UICONTROL Filtros] em branco.
1. Abra as **[!UICONTROL Configurações de relatório]** e nomeie o relatório como “Pesquisa de notas”.
1. No campo [!UICONTROL Descrição], coloque algo como “Pesquisar notas do sistema ou do usuário com base no tipo de auditoria selecionado e outras solicitações. As notas do sistema são exibidas na coluna Texto da auditoria e as do usuário na coluna Texto da nota.”

   ![Uma imagem da tela para criar configurações de relatório de notas](assets/note-report-report-options.png)

1. Selecione a **[!UICONTROL Guia Detalhes]** para exibição quando o relatório for carregado.
1. Defina o relatório para mostrar 200 itens quando ele for incluído em um painel.
1. Clique em **[!UICONTROL Prompts do relatório]** e adicione:

   ![Uma imagem da tela para criar prompts de relatório de notas](assets/note-report-report-prompts.png)

   * [!UICONTROL Nota] > [!UICONTROL Texto de auditoria]
   * [!UICONTROL Nota] > [!UICONTROL Texto da Nota]
   * [!UICONTROL Proprietário] > [!UICONTROL Nome]
   * [!UICONTROL Nota] > [!UICONTROL Data de entrada]
   * [!UICONTROL Projeto] > [!UICONTROL Nome]
   * [!UICONTROL Nota] > [!UICONTROL  Tipo de auditoria]

1. Marque a caixa para **[!UICONTROL Mostrar prompts em painéis]**.
1. Salve e feche o relatório.

## Atividade 2: criar um relatório de feedback de equipe administrativa

Este é um relatório que mostra todos os problemas de uma fila de solicitações de feedback criada para admins de sistema. Você pode ver como criar essa fila de solicitações no tutorial [Criar uma fila de solicitações de feedback para admins de sistema](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/create-a-system-admin-feedback-request-queue.html?lang=pt-BR).

Esse relatório também usa um formulário personalizado. Para saber como criar um formulário personalizado, consulte o tutorial [Criar e compartilhar um formulário personalizado](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/custom-data/custom-forms/custom-forms-creating-and-sharing-a-custom-form.html?lang=pt-BR).

Esse formulário personalizado deve ser criado da seguinte maneira:

Nome: feedback do processo administrativo

1. Tipo de processo (campo suspenso)
   * níveis de acesso
   * processo de aprovação (somente global)
   * notificações de email
   * modelo de Layout
   * caminho de marcos
   * modelo de projeto
   * notificações de lembrete
   * fila de solicitações
1. Nome do processo (campo de texto de linha única)
1. Grau do processo (campo suspenso)
   * 1 - totalmente inútil
   * 2 - não muito útil
   * 3 - bom, mas poderia ser melhor
   * 4 - excelente
1. Problema ou boas notícias (campo de texto de parágrafo)

Crie um relatório de problemas chamado **Relatório de feedback da equipe administrativa**.

A visualização deve ter as seguintes colunas:

* Problema: nome
* Contato principal: nome
* Problema: tipo de processo
* Problema: nome do processo
* Problema: grau do processo
* Problema: problema ou boas notícias
* Problema: data de entrada
* Problema: idade
* Problema: atribuições
* Problema: status

Tipo de grupo do processo.

Filtre a ID do projeto da fila de solicitações que contém os problemas de feedback.


![Uma captura de tela do relatório de feedback da equipe administrativa](assets/create-a-system-admin-feedback-request-queue.png)



## Resposta da atividade 2

1. Selecione **[!UICONTROL Relatórios]** no **[!UICONTROL Menu principal]**.
1. Clique no menu **[!UICONTROL Novo relatório]** e selecione **[!UICONTROL Problema]**.
1. Em **[!UICONTROL Colunas (Visualização)]** configure as colunas para incluir:

   ![Uma imagem da tela de criação de colunas de relatórios de problemas](assets/task-report-activity-2-1.png)

   * [!UICONTROL Problema] > [!UICONTROL Nome]
   * [!UICONTROL Contato principal] > [!UICONTROL Nome]
      * Observação: “Owner:Name” é exibido como o rótulo da coluna. Você pode alterar isso para “Relatado por” clicando em Opções avançadas e digitando “Relatado por” no campo **Rótulo de coluna personalizado**.
   * [!UICONTROL Problema] > [!UICONTROL Tipo de processo]
   * [!UICONTROL Problema] > [!UICONTROL Nome do processo]
   * [!UICONTROL Problema] > [!UICONTROL Grau do processo]
   * [!UICONTROL Problema] > [!UICONTROL Problema ou boas notícias]
   * [!UICONTROL Problema] > [!UICONTROL Data de entrada]
   * [!UICONTROL Problema] > [!UICONTROL Idade]
   * [!UICONTROL Problema] > [!UICONTROL Atribuições]
   * [!UICONTROL Problema] > [!UICONTROL Status]

1. Selecione a coluna **[!UICONTROL Data de entrada]** e altere **[!UICONTROL Classificar para decrescente]**.
1. Na guia **[!UICONTROL Agrupamentos]**, defina o agrupamento do relatório como **[!UICONTROL Problema] > [!UICONTROL Tipo de processo]**.

   ![Uma imagem da tela de criação de agrupamentos de relatórios de problemas](assets/task-report-activity-2-2.png)

1. Na guia **[!UICONTROL Filtros]**, adicione um filtro de **[!UICONTROL Problema] > [!UICONTROL ID do projeto]** igual ao do projeto da fila de solicitações que contém os problemas de feedback.

   ![Uma imagem da tela de criação de filtros de relatório de problemas](assets/task-report-activity-2-3.png)

1. Salve e feche o relatório.
