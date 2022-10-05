---
title: Introdução a funções de prova e alertas de email
description: Saiba como habilitar funções de prova adequadas e alertas de email para que os recipients de prova tenham acesso a provas e visibilidade do trabalho que está sendo feito em [!DNL  Workfront].
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Beginner
thumbnail: proof-roles-and-email-alerts.png
kt: 10177
exl-id: 15bfb18a-5392-4a91-a6a2-223f7ac30dc5
source-git-commit: c06dcc985c3b63781911e3c8cb1ac0f1a888ac7d
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 0%

---

# Funções de prova e alertas de email

As funções de prova e alertas de email ajudam a direcionar o fluxo de trabalho de prova, garantindo que os recipients tenham o acesso correto às provas e tenham visibilidade do trabalho que está sendo feito.

Vamos analisar a terminologia básica da prova:

* **Função de prova —** Define o que um usuário pode fazer com uma prova (por exemplo, comentário, marcação, aprovar, etc.).
* **Alerta por email —** Emails enviados às pessoas no workflow de prova quando há atividade na prova.

![Uma imagem da [!UICONTROL Nova prova] com a [!UICONTROL Função de prova] e [!UICONTROL Alertas por email] colunas realçadas.](assets/proof-roles-and-email-alerts.png)

O administrador do sistema de prova pode definir funções de prova padrão e alertas de email para os usuários de prova da organização. Além disso, essas informações podem ser incorporadas a templates de workflow de prova (também conhecidos como templates de workflow automatizados).

No entanto, pode haver momentos em que você precise definir essas informações manualmente ao fazer upload de uma prova.

[!DNL Workfront] O oferece essas recomendações gerais ao atribuir funções de prova aos recipients de prova:

* **Revisor e Aprovador —** Esses usuários podem fazer comentários em provas e tomar uma decisão (como aprovada ou rejeitada) em uma prova. Use esta função de prova para as principais partes interessadas internas e externas no processo de revisão.
* **Revisor —** Algumas pessoas no fluxo de trabalho de prova precisam apenas fazer comentários. Essa função é ideal para elas. A função de revisor também pode ser atribuída ao [!DNL Workfront] os usuários que carregam principalmente provas ou servem como proprietário de prova, mas que de outra forma não fazem parte do processo de revisão de texto.
* **Somente leitura —** Ideal para recipients que precisam apenas ver a prova. [!UICONTROL Somente leitura] O fornece acesso à visualização e não permite comentários.

[!DNL Workfront] O oferece essas recomendações gerais ao atribuir alertas de email a recipients de prova:

* **Decisão final —** Isso envia um email quando a última pessoa toma uma decisão na prova. Atribua isso à pessoa que está monitorando o workflow de prova. Pode ser um gerente de prova, proprietário de prova, criador de prova, gerente de projeto ou outro [!DNL Workfront] usuário. [!DNL Workfront] O recomenda esse alerta ao usar um workflow básico, para que a pessoa que está monitorando a prova saiba que todas as decisões foram tomadas.
* **Decisões —** Isso envia alertas quando cada parte interessada no fluxo de trabalho de prova toma uma decisão sobre a prova. Essa opção é melhor ao usar um fluxo de trabalho automatizado, com várias decisões. Atribua à pessoa que está monitorando o workflow de prova. Pode ser um gerente de prova, proprietário de prova, criador de prova, gerente de projeto ou outro [!DNL Workfront] usuário.
* **Desabilitado —** Use para usuários de prova de convidado para limitar o número de emails recebidos sobre a prova. Os recipients ainda são notificados sobre novas provas, novas versões e provas atrasadas, além de [!DNL Workfront] os usuários recebem mensagens diretas feitas em um comentário de prova usando @username e recipients convidados com @emailaddress.

## Sua vez

1. Faça logon no Workfront e crie usuários que usarão provas que você não criou anteriormente. Defina o perfil de permissões de prova nas configurações do usuário de acordo com a função que a pessoa reproduzirá nos workflows de prova.
1. Para usuários que já foram criados, edite as configurações para ajustar a seleção de perfil de permissões de prova e , se necessário.
1. Acesse a área Configuração de prova e vá para a guia Usuários . Verifique as configurações pessoais dos usuários - idioma, fuso horário, formato de data, função de prova padrão e alerta por email padrão. Isso é importante se esses usuários tiverem sido criados antes que os padrões globais do sistema fossem estabelecidos (essas configurações são discutidas na Seção 1 deste caminho de aprendizagem).

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
