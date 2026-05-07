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
last-substantial-update: '2025-06-27T00:00:00.000Z'
jira: KT-9082
exl-id: 0f7db4eb-a062-4eb3-99ca-c40d8e266943
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: c6dd2ac5-f5bd-4e59-9101-25b156918623
subfeature_v2:
  - id: ceb4d94a-32ed-4fea-9724-1339d684b0bc
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-06T13:57:08.996Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 246
ht-degree: 100%

---

# Criar filtros com curingas baseados em data

Neste vídeo, você aprenderá a:

* Saiba quando usar curingas baseados em data
* Entenda a diferença entre os dois curingas baseados em data do Workfront
* Adicionar um curinga baseado em data a um filtro
* Criar uma data personalizada usando curingas, atributos, operadores e modificadores
* Criar um intervalo de datas personalizado usando curingas

>[!VIDEO](https://video.tv.adobe.com/v/336812/?quality=12&learn=on&enablevpops=0)


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
