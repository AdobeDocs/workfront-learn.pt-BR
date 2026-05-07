---
title: Atividade - Criar um relatório de calendário
description: Instruções passo a passo sobre como criar um calendário do cliente mostrando suas tarefas incompletas e problemas.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
last-substantial-update: '2025-06-23T00:00:00.000Z'
thumbnail: your-turn-to-create-a-calendar.png
jira: KT-10026
exl-id: 74d57f1a-c6c5-49e0-9529-2e2deb2f273e
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: c6dd2ac5-f5bd-4e59-9101-25b156918623
subfeature_v2: id: c6584858-4838-4ce3-ab7f-7292f37179f4
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T14:16:18.343Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 362
ht-degree: 81%

---

# Atividade - Criar um relatório de calendário

Crie um calendário de cliente chamado de “Meu trabalho pendente”.

Inclua um grupo de calendários chamado “Tarefas pendentes”, mostrando todas as tarefas pendentes atribuídas a você nos projetos atuais.

Selecione a cor vermelho para esses itens.

Inclua outro grupo de calendário chamado “Problemas pendentes”, mostrando todos os problemas pendentes atribuídos a você nos projetos atuais. Selecione a cor azul para esses itens.

## Responder

1. Navegue até a área “Calendários” do menu principal.
1. Clique no botão “Novo calendário” e nomeie o calendário como “Meu trabalho pendente”.
1. Clique no botão Adicionar ao calendário e Adicionar itens avançados.
1. Na janela “Adicionar itens ao calendário”, nomeie o grupo como “Tarefas pendentes”.
1. Selecione a cor vermelho.
1. Altere o campo “Data” para “Datas planejadas”.
1. Defina o campo “No calendário, mostrar” como “Somente data final”.
1. Defina o campo “Alternar para as datas reais quando disponíveis” como “Não”.
1. Na seção “O que você gostaria de adicionar ao calendário?”, selecione Tarefas. Em seguida, clique no botão Adicionar tarefas.
1. Adicione três regras de filtro:

   * Projeto > Status igual a > Igual > Atual
   * Usuários atribuídos > ID > Igual > $$USER.ID
   * Tarefa > Está concluída > Igual > Falso

1. Clique em Salvar.

   ![Uma imagem da tela de adição de itens a um calendário](assets/calendar-activity-1.png)

1. Crie um segundo agrupamento clicando em Adicionar ao calendário e Adicionar itens avançados.
1. Na janela “Adicionar itens ao calendário”, nomeie o grupo como “Problemas pendentes”.
1. Selecione a cor azul.
1. Altere o campo “Data” para “Datas planejadas”.
1. Defina o campo “No calendário, mostrar” como “Somente data final”.
1. Defina o campo “Alternar para as datas reais quando disponíveis” como “Não”.
1. Na seção “O que você gostaria de adicionar ao calendário?”, selecione Problemas. Em seguida, clique no botão Add Issues (Adicionar problemas).
1. Adicione as três regras de filtro a seguir:

   * Projeto > Status igual a > Igual > Atual
   * Usuários atribuídos > ID > Igual > $$USER.ID
   * Problema > Está completo > Igual > Falso

1. Clique em Salvar.

   ![Uma imagem da tela de adição de itens a um calendário](assets/calendar-activity-2.png)

Como você usou $$USER.ID nos filtros, poderá compartilhar este calendário com outras pessoas para que vejam suas próprias tarefas e problemas pendentes.
