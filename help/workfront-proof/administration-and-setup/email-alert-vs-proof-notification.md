---
title: Entenda sobre alertas de email e notificações de prova
description: Entenda a diferença entre alertas de email e notificações de prova no  [!DNL  Workfront].
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: email-alert-vs-proof-notifications.png
jira: KT-10174
last-substantial-update: '2024-01-24T00:00:00.000Z'
exl-id: 51423110-960c-46ed-8b4e-6e73c67c42e0
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: b18b693b-6d59-4359-95fd-a386b7a615fe
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-05T20:07:01.396Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 307
ht-degree: 100%

---

# Entenda sobre alertas de email e notificações de prova

Os alertas por email são diferentes dos emails de notificação de prova. Você receberá um email de notificação de prova quando receber uma nova prova para revisar, quando uma prova estiver atrasada ou quando houver uma nova versão para análise.

![Uma imagem de um email de notificação de prova indicando que há uma nova prova a ser revisada.](assets/email-alert-1.png)

Se você desativar a opção de notificação ao enviar uma prova, ninguém receberá mensagens do [!DNL Workfront] informando que há uma nova prova para ser revisada.

Os alertas por email são definidos por revisor ou aprovador, geralmente, assim que a prova é carregada. Um tipo de alerta de email padrão pode ser atribuído aos destinatários, para que você não precise defini-lo sempre que fizer upload de uma prova. Converse com o(a) admin de sistema sobre como definir esses padrões.

![Uma imagem de um alerta por email indicando que uma decisão foi tomada na prova e que há um comentário para revisão.](assets/email-alert-2.png)

Mesmo que os alertas por email estejam configurados como [!UICONTROL Desabilitado], os destinatários da prova ainda serão notificados sobre uma nova prova ou versão.

## Práticas recomendadas

| Prática recomendada | Saiba por quê |
|---|---|
| Desabilite a configuração “Enviar emails do Workfront quando um comentário for feito em uma prova” nas configurações do Workfront | Quando essa configuração está habilitada (por padrão), os usuários têm a possibilidade de receber diversas notificações por email para cada comentário em uma revisão, uma da funcionalidade de revisão e outra do próprio Workfront. Essas notificações duplicadas levam à interrupção e confusão das notificações por email, bem como a uma caixa de entrada de email cheia, o que pode fazer com que os usuários ignorem as notificações de revisão recebidas. Isso, por sua vez, pode resultar em prazos perdidos. <br> <br>Observação: esta configuração do Workfront é encontrada em Menu principal > Configuração > Email > Revisão e aprovação. |


