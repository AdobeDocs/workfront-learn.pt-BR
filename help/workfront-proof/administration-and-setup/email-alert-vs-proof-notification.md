---
title: Entender alertas de email e notificações de prova
description: Entenda a diferença entre alertas de email e notificações de prova no [!DNL  Workfront].
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: email-alert-vs-proof-notifications.png
jira: KT-10174
last-substantial-update: 2024-01-23T00:00:00Z
exl-id: 51423110-960c-46ed-8b4e-6e73c67c42e0
source-git-commit: 731005176bc02e3a4d26d00373931fa7444afeea
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---

# Entender alertas de email e notificações de prova

Os alertas de email são diferentes dos emails de notificação de prova. Você receberá um email de notificação de prova quando receber uma nova prova para revisão, quando uma prova estiver atrasada ou quando houver uma nova versão da prova para você examinar.

![Uma imagem de um email de notificação de prova indicando que há uma nova prova a ser revisada.](assets/email-alert-1.png)

Se você desativar a opção de notificação ao carregar uma prova, ninguém receberá qualquer comunicação do [!DNL Workfront] sobre a existência de uma nova prova a ser revisada.

Os alertas de email são definidos por revisor/aprovador, com mais frequência conforme o upload da prova é feito. Um tipo de alerta de email padrão pode ser atribuído aos recipients de prova para que você não precise configurá-lo sempre que fizer upload de uma prova. Fale com o administrador do sistema sobre como definir esses padrões.

![Imagem de um alerta por email indicando que foi tomada uma decisão sobre a prova e que há um comentário a ser revisado.](assets/email-alert-2.png)

Mesmo se os alertas de email estiverem definidos como [!UICONTROL Desabilitado], os recipients de prova ainda serão notificados sobre uma nova prova ou versão.

## Práticas recomendadas

| Prática recomendada | Aqui está o porquê |
|---|---|
| Desative a configuração &quot;Enviar emails do Workfront quando um comentário for feito em uma prova&quot; nas configurações do Workfront | Quando essa configuração estiver ativada (que é por padrão), os usuários têm o potencial de obter várias notificações por email para cada comentário em uma prova, uma da funcionalidade de prova e outra do próprio Workfront. Essas notificações duplicadas causam confusão e interrupção de notificações por email, bem como uma caixa de entrada de email completa, que pode resultar no ignoramento de notificações de prova recebidas pelos usuários. O que, por sua vez, poderia significar o não cumprimento de prazos. <br> <br>Observação: essa configuração é encontrada no Menu principal do Workfront > Configuração > Email > Revisão e aprovação. |


