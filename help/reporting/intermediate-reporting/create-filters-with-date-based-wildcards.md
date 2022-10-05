---
title: Criar filtros com caracteres curingas com base em data
description: Saiba como e quando usar curingas com base em data e criar um filtro com um curinga com base em data em [!DNL  Workfront].
activity: use
feature: Reports and Dashboards
thumbnail: 336812.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9082
exl-id: 0f7db4eb-a062-4eb3-99ca-c40d8e266943
source-git-commit: 83c7379a5398c78cea31a4571b34fd5b64bce027
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

---

# Criar filtros com caracteres curingas com base em data

Neste vídeo, você aprenderá a:

* Saiba quando usar curingas com base em data
* Entenda a diferença entre os dois curingas com base em data do Workfront
* Adicionar um curinga com base em data a um filtro
* Criar uma data personalizada usando curingas, atributos, operadores e modificadores
* Criar um intervalo de datas personalizado usando curingas

>[!VIDEO](https://video.tv.adobe.com/v/336812/?quality=12)

## Perguntas sobre a atividade

1. Como você criaria a regra de filtro se quisesse problemas que tivessem uma data de vencimento de ontem ou hoje?
1. Como você criaria a regra de filtro para encontrar projetos que estavam previstos na semana passada?
1. As seguintes regras de filtro fazem parte de um relatório de tarefa que você usa regularmente. Que tipo de resultados obteria com este relatório?

![Uma imagem da tela para criar um filtro de tarefa com um curinga baseado em data](assets/date-wildcard-answer-1.png)

## Respostas

1. Filtrar a data de conclusão planejada da emissão entre [!UICONTROL $$TODAY-1d] e [!UICONTROL $$TODAY].
1. Filtrar a data de conclusão planejada do projeto entre [!UICONTROL $$TODAYb-1w] e [!UICONTROL $$TODAYe-1w].
1. Este relatório encontra tarefas atribuídas a você que ainda não foram concluídas (em outras palavras, têm uma porcentagem de conclusão menor que 100) e que estão vencidas ou vencidas hoje. A regra de filtro para a data de conclusão planejada das tarefas diz para examinar as tarefas que têm uma data de vencimento igual ou anterior à data de hoje.
