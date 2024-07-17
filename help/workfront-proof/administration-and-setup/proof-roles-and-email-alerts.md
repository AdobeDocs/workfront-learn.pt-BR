---
title: Funções de prova e alertas por email
description: Aprenda a habilitar funções de prova e alertas por email adequados para que os destinatários das provas tenham acesso a elas e possam ver o trabalho que está sendo realizado no [!DNL  Workfront].
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
ht-degree: 100%

---

# Funções de prova e alertas por email

As funções de prova e os alertas por email ajudam a impulsionar o fluxo de trabalho de prova, garantindo que os destinatários possam acessar as provas e ver o trabalho que está sendo realizado.

Vamos revisar algumas terminologias básicas de prova:

* **Função na prova -** Define o que um usuário pode fazer com uma prova (por exemplo, comentar, marcar, aprovar etc.).
* **Alerta por email -** Emails enviados para pessoas no fluxo de trabalho de prova quando uma atividade é realizada.

![Uma imagem da janela [!UICONTROL Nova prova] com as colunas [!UICONTROL Função na prova] e [!UICONTROL Alertas por email] realçadas.](assets/proof-roles-and-email-alerts.png)

O(a) admin do sistema de prova pode definir configurações padrão de função de prova e alertas por email para os usuários de prova da sua organização. Além disso, essas informações podem ser inseridas em modelos de fluxo de trabalho de prova (também conhecidos como modelos de fluxo de trabalho automatizados).

No entanto, pode haver momentos em que você precise definir essas informações manualmente ao fazer o upload de uma prova.

O [!DNL Workfront] oferece estas recomendações gerais ao atribuir funções de prova aos destinatários da prova:

* **Revisor e Aprovador -** Esses usuários podem fazer comentários e tomar uma decisão sobre uma prova (como aprovar ou rejeitar). Use esta função de prova para as principais partes interessadas (sejam internas ou externas) no processo de revisão.
* **Revisor -** Algumas pessoas do fluxo de trabalho de prova só precisam fazer comentários; essa função é ideal para elas. A função de revisor também pode ser atribuída a usuários do [!DNL Workfront] que apenas fazem upload de provas ou atuam como proprietários das provas, mas que não fazem parte do processo de revisão.
* **Somente leitura -** Ideal para destinatários que precisam apenas ver a prova. A função [!UICONTROL Somente leitura] concede acesso de visualização e não permite fazer comentários.

O [!DNL Workfront] oferece estas recomendações gerais ao atribuir alertas por email aos destinatários da prova:

* **Decisão final -** Isso envia um email quando a última pessoa toma uma decisão sobre a prova. Atribua isso à pessoa que monitora o fluxo de trabalho de prova. Esta pessoa pode ser: gerente de provas, proprietário de provas, criador de provas, gerente de projeto ou outro usuário do [!DNL Workfront]. O [!DNL Workfront] recomenda utilizar esse alerta em um fluxo de trabalho básico, para que a pessoa que monitora a prova saiba que todas as decisões foram tomadas.
* **Decisões -** Isso envia alertas à medida que cada parte interessada no fluxo de trabalho de prova toma uma decisão sobre a prova. Esta opção é recomendada ao utilizar um fluxo de trabalho automatizado, com diversas decisões. Atribua essa opção à pessoa que monitora o fluxo de trabalho de prova. Esta pessoa pode ser: gerente de provas, proprietário de provas, criador de provas, gerente de projeto ou outro usuário do [!DNL Workfront].
* **Desabilitado -** Use isto para usuários de prova convidados a fim de limitar o número de emails que recebem sobre a prova. Os destinatários ainda são notificados sobre novas provas, novas versões e provas atrasadas; além disso, os usuários do [!DNL Workfront] são notificados sobre mensagens diretas feitas em um comentário de prova utilizando @nomedeusuário, e o mesmo ocorre para destinatários convidados com @endereçodeemail.

## Sua vez

1. Faça logon no Workfront e crie usuários de provas que você não criou anteriormente. Defina o perfil de permissões de prova nas configurações do usuário, de acordo com a função que a pessoa desempenhará nos fluxos de trabalho de prova.
1. Para usuários já criados, edite as configurações para se ajustar ao perfil de permissões de prova, se necessário.
1. Acesse a área de configurações de prova e vá até a guia Usuários. Verifique as configurações pessoais dos usuários: idioma, fuso horário, formato de data, função de prova padrão e alerta de email padrão. Isto é importante caso os usuários tenham sido criados antes de se estabelecer os padrões globais do sistema.

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
