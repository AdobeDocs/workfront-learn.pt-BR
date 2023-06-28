---
title: Funções de prova e alertas de email
description: Saiba como ativar funções de prova e alertas de email adequados para que os recipients de prova tenham acesso a provas e visibilidade do trabalho que está sendo feito no [!DNL  Workfront].
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Beginner
thumbnail: proof-roles-and-email-alerts.png
jira: KT-10177
exl-id: 15bfb18a-5392-4a91-a6a2-223f7ac30dc5
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

# Funções de prova e alertas de email

Funções de prova e alertas de email ajudam a direcionar o fluxo de trabalho de prova, garantindo que os recipients tenham o acesso correto às provas e visibilidade do trabalho que está sendo feito.

Vamos analisar alguns termos básicos de prova:

* **Função de prova —** Define o que um usuário pode fazer com uma prova (por exemplo, comentário, marcação, aprovação etc.).
* **Alerta por email —** Emails enviados para pessoas no fluxo de trabalho de prova quando há atividade na prova.

![Uma imagem do [!UICONTROL Nova prova] janela com o [!UICONTROL Função de prova] e [!UICONTROL Alertas de email] colunas realçadas.](assets/proof-roles-and-email-alerts.png)

O administrador do sistema de prova pode definir funções de prova padrão e alertas de email para os usuários de prova da sua organização. Além disso, essas informações podem ser inseridas em modelos de fluxo de trabalho de prova (também conhecidos como modelos de fluxo de trabalho automatizados).

No entanto, pode haver momentos em que você precise definir essas informações manualmente ao carregar uma prova.

[!DNL Workfront] O oferece estas recomendações gerais ao atribuir funções de prova a recipients de prova:

* **Revisor e Aprovador —** Esses usuários podem fazer comentários sobre provas e tomar uma decisão (como aprovada ou rejeitada) sobre uma prova. Use essa função de prova para os principais participantes internos e externos no processo de revisão.
* **Revisor —** Algumas pessoas no fluxo de trabalho de prova precisam apenas fazer comentários, essa função é ideal para elas. A função de revisor também pode ser atribuída a [!DNL Workfront] usuários que fazem upload de provas principalmente ou servem como proprietários de prova, mas não fazem parte do processo de prova.
* **Somente Leitura —** Ideal para recipients que só precisam ver a prova. [!UICONTROL Somente leitura] concede acesso à visualização e não permite comentários.

[!DNL Workfront] O oferece estas recomendações gerais ao atribuir alertas de email a destinatários de prova:

* **Decisão final —** Isso envia um email quando a última pessoa toma uma decisão sobre a prova. Atribua isso à pessoa que monitora o fluxo de trabalho de prova. Pode ser um gerente de prova, proprietário de prova, criador de prova, gerente de projeto ou outro [!DNL Workfront] usuário. [!DNL Workfront] O recomenda esse alerta ao usar um fluxo de trabalho básico, para que a pessoa que monitora a prova saiba que todas as decisões foram tomadas.
* **Decisões —** Isso envia alertas conforme cada parte interessada do fluxo de trabalho de prova toma uma decisão sobre a prova. Essa opção é melhor ao usar um fluxo de trabalho automatizado, com várias decisões. Atribua à pessoa que monitora o fluxo de trabalho de prova. Pode ser um gerente de prova, proprietário de prova, criador de prova, gerente de projeto ou outro [!DNL Workfront] usuário.
* **Desativado —** Use isso para usuários de prova convidados para limitar o número de emails que eles recebem sobre a prova. Os recipients ainda são notificados sobre novas provas, novas versões e provas atrasadas, além de [!DNL Workfront] os usuários recebem mensagens diretas feitas em um comentário de prova usando @username e recipients convidados com @emailaddress.

## Sua vez

1. Faça logon no Workfront e crie usuários que usarão provas de que você não criou anteriormente. Defina o perfil de permissões de prova nas configurações do usuário de acordo com a função que a pessoa terá nos fluxos de trabalho de prova.
1. Para usuários que já foram criados, edite as configurações para ajustar a seleção de perfil de permissões de prova, se necessário.
1. Acesse a área Configurações de prova e vá para a guia Usuários. Verifique as configurações pessoais dos usuários (idioma, fuso horário, formato de data, função de prova padrão e alerta de email padrão). Isso é importante se esses usuários tiverem sido criados antes de os padrões do sistema global serem estabelecidos.

<!--
Download the proof role and email alert guides to have on hand as you start uploading proofs and assigning proof recipients.
-->

<!--
## Learn more
* Notifications for proof comments and decisions
-->

<!--
## Guides
* Proof roles
* Email alerts
-->
