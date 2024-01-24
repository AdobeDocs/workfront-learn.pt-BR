---
title: Criar um modelo de fluxo de trabalho automatizado
description: Saiba como criar um modelo de fluxo de trabalho automatizado atribuindo recipients de prova e definindo prazos de prova. Em seguida, compartilhe o template com outros usuários.
activity: use
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
team: Technical Marketing
thumbnail: 335130.png
jira: KT-8830
last-substantial-update: 2024-01-23T00:00:00Z
exl-id: eac89e40-d3ea-4376-82a2-16bec550d131
doc-type: video
source-git-commit: 731005176bc02e3a4d26d00373931fa7444afeea
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---

# Criar um modelo de fluxo de trabalho automatizado

Neste vídeo, você aprenderá a:

* Criar um modelo de fluxo de trabalho automatizado para [!DNL  Workfront] prova
* Atribuir recipients de prova
* Definir um prazo do processo de revisão e aprovação
* Compartilhar o modelo de fluxo de trabalho automatizado com outras pessoas

>[!VIDEO](https://video.tv.adobe.com/v/335130/?quality=12&learn=on)

## Opções adicionais de ativação de estágio

Duas opções para determinar quando um estágio do fluxo de trabalho de prova deve ser iniciado raramente são usadas, se houver: a variável [!UICONTROL Data e hora] e a opção &quot;[!UICONTROL Quando o prazo final do estágio anterior passar]&quot;.

A segunda opção realmente só funciona em cenários nos quais há um grande grupo de pessoas revisando e nas quais você não quer esperar por todas elas. É um tipo de opção &quot;Eu vou lhe dar um certo tempo para completar sua revisão e então você perde sua chance&quot;. Mas mesmo isso pode retardar um processo de revisão.

Se você usar &quot;[!UICONTROL quando o prazo final do estágio anterior passar],&quot; é importante lembrar que você pode ativar manualmente um estágio a qualquer momento se não quiser esperar o término de um prazo.

## Práticas recomendadas

| Prática recomendada | Aqui está o porquê |
|---|---|
| Defina a função de prova do criador da prova como Revisor. | A função de prova Revisor garante que o criador da prova possa fazer comentários e acessar comentários deixados por outros. Na maioria das vezes, o criador da prova não é obrigado a tomar uma decisão sobre uma prova que carregou. As funções de prova Aprovador, Revisor e Aprovador, Autor ou Moderador exigem que seja tomada uma decisão. Se o criador da prova receber uma dessas funções de prova, mas nunca tomar uma decisão, isso poderá afetar negativamente os prazos de prova. |
| Evite usar a função de prova Aprovador. | A função de Aprovador de prova não permite que o usuário faça comentários nesta prova. Isso pode levar um usuário a rejeitar a prova, sem qualquer explicação, porque não pode fazer comentários. Em vez disso, use a função de prova Revisor e Aprovador para que o usuário possa fornecer feedback. |
| Evite a opção de alerta por email de prova de Todas as atividades. | Essa opção envia uma notificação por email de prova sempre que algo acontece com uma prova: um comentário é feito, uma resposta é postada, uma decisão é tomada, etc. O recipient está essencialmente vendo a atividade de prova à medida que ela acontece.<br><br>Para proprietários e criadores de provas, o alerta por email de Decisões funciona melhor para fluxos de trabalho de prova de vários estágios e a Decisão final funciona melhor para fluxos de trabalho de estágio único. Geralmente, todos os outros podem ser definidos como Desativado, a menos que queiram ser notificados sobre outras pessoas que estejam fazendo comentários ou tomando decisões (nesse caso, uma das opções de resumo de email pode funcionar melhor). |
