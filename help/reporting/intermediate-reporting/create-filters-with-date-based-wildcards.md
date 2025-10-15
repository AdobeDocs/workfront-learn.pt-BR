---
title: Criar filtros com curingas baseados em data
description: Aprenda como e quando usar curingas baseados em data e como criar um filtro com base na data atual.
activity: use
feature: Reports and Dashboards
thumbnail: 336812.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: 2025-06-27T00:00:00Z
jira: KT-9082
exl-id: 0f7db4eb-a062-4eb3-99ca-c40d8e266943
doc-type: video
source-git-commit: cc423944628d01e16d390842ecb25696505f923c
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Criar filtros com curingas baseados em data

Neste vídeo, você aprenderá a:

* Saiba quando usar curingas baseados em data
* Entenda a diferença entre os dois curingas baseados em data do Workfront
* Adicionar um curinga baseado em data a um filtro
* Criar uma data personalizada usando curingas, atributos, operadores e modificadores
* Criar um intervalo de datas personalizado usando curingas

>[!VIDEO](https://video.tv.adobe.com/v/3413828/?captions=por_br&quality=12&learn=on&enablevpops=0)


## Atividades “Criar filtros com curingas baseados em data”


### Perguntas sobre a atividade

1. Como você criaria a regra de filtro se estivesse procurando por problemas com uma data de vencimento para o dia de ontem ou hoje?
1. Como você criaria a regra de filtro para encontrar projetos com uma data de vencimento para a semana passada?
1. As regras de filtro a seguir fazem parte de um relatório de tarefas que você usa regularmente. Que tipos de resultado você obteria com esse relatório?

![Uma imagem da tela de criação de filtros de tarefa com um curinga baseado em data](assets/date-wildcard-answer-1.png)

### Respostas

1. Filtrar problemas com uma data de conclusão planejada entre [!UICONTROL $$TODAY-1d] e [!UICONTROL $$TODAY].
1. Filtrar projetos com uma data de conclusão planejada entre [!UICONTROL $$TODAYb-1w] e [!UICONTROL $$TODAYe-1w].
1. Este relatório encontrou tarefas atribuídas a você que ainda não foram concluídas (ou seja, têm uma porcentagem de conclusão menor que 100) e que estão atrasadas ou vencem hoje. A regra de filtro para a data de conclusão planejada das tarefas orienta a analisar tarefas que tenham uma data de vencimento igual ou anterior à data de hoje.
