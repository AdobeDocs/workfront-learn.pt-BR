---
title: Criar um modelo de fluxo de trabalho automatizado
description: Aprenda como criar um modelo de fluxo de trabalho automatizado, atribuindo destinatários de provas e definindo prazos para provas. Em seguida, compartilhe o modelo com outros usuários.
activity: use
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
team: Technical Marketing
thumbnail: 335130.png
jira: KT-8830
last-substantial-update: 2024-01-24T00:00:00Z
exl-id: eac89e40-d3ea-4376-82a2-16bec550d131
doc-type: video
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: ht
source-wordcount: '432'
ht-degree: 100%

---

# Criar um modelo de fluxo de trabalho automatizado

Neste vídeo, você aprenderá a:

* Criar um modelo de fluxo de trabalho automatizado de prova no [!DNL  Workfront] 
* Atribuir destinatários de prova
* Definir um prazo para o processo de revisão e aprovação
* Compartilhar o modelo de fluxo de trabalho automatizado com outras pessoas

>[!VIDEO](https://video.tv.adobe.com/v/3454256/?quality=12&learn=on&enablevpops&captions=por_br)

## Opções adicionais de ativação de estágio

Há duas opções que raramente (ou nunca) são usadas para determinar quando um estágio do fluxo de trabalho de revisão deve começar: as opções [!UICONTROL Data e hora] e “[!UICONTROL Quando o prazo da etapa anterior expirar]”.

Realisticamente, a segunda opção só funciona em cenários onde você tem um grande grupo de pessoas revisando e não quer esperar por todas elas. Seria como dizer: “Vou dar um tempo para você concluir sua revisão, mas se não o fizer, perderá sua chance”. Mas isso pode até mesmo retardar o processo de revisão.

Se você usar a opção “[!UICONTROL Quando o prazo do estágio anterior expirar]”, é importante lembrar que é possível ativar manualmente um estágio a qualquer momento se não quiser esperar o prazo expirar.

## Práticas recomendadas

| Prática recomendada | Saiba por quê |
|---|---|
| Defina a função de prova do(a) criador(a) da revisão como “Revisor”. | A função de prova “Revisor” garante que o criador da prova possa fazer comentários e acessar comentários feitos por outras pessoas. Na maioria das vezes, o(a) criador(a) da revisão não tem a obrigação de tomar uma decisão sobre a revisão que carregou. As funções de prova “Aprovador”, “Revisor e Aprovador”, “Autor” ou “Moderador” exigem a tomada de uma decisão. Se o criador da prova receber uma dessas funções, mas não tomar nenhum decisão, isso poderá afetar negativamente os prazos das provas. |
| Evite usar a função de revisão “Aprovador”. | A função “Aprovador” não permite que o usuário faça comentários nesta prova. Isso poderia levar uma pessoa a rejeitar a revisão, sem qualquer explicação, pois não seria possível fazer comentários. Utilize a função de prova “Revisor e Aprovador” para que o usuário possa fornecer feedback. |
| Evite a opção de alerta por email de revisão “Todas as atividades”. | Esta opção envia uma notificação por email sobre a prova sempre que algo acontece, como quando um comentário é feito, uma resposta é postada, uma decisão é tomada etc. O recipient essencialmente vê a atividade da prova conforme ela acontece.<br><br>Para proprietários e criadores de revisões, o alerta de “Decisões” por email funciona melhor em fluxos de trabalho de revisão de vários estágios e a “Decisão final” funciona melhor para fluxos de trabalho de estágio único. Geralmente, todos os outros usuários podem ser definidos como Desabilitados, a menos que queiram ser notificados sobre comentários ou decisões de outras pessoas (nesse caso, uma das opções de resumo por email pode funcionar melhor). |
