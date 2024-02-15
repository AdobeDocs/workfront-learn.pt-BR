---
title: Definir funções de prova padrão
description: Saiba como definir a função de prova padrão que é atribuída quando novos usuários são criados ou alguém abre uma prova.
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: set-default-proof-roles.png
jira: KT-10235
last-substantial-update: 2024-01-24T00:00:00Z
exl-id: 77dfb9f1-3242-47ca-a0ce-203b535af156
source-git-commit: 30748311c14fb8aa6b10c03a74e83f46bdb5dfbf
workflow-type: ht
source-wordcount: '359'
ht-degree: 100%

---

# Definir funções de prova padrão



A primeira configuração padrão a ser concluída é determinar uma função de prova padrão que será atribuída quando novos usuários forem criados ou as pessoas abrirem uma prova.

As funções de prova determinam o que um usuário é capaz de fazer com uma prova: somente leitura, fazer comentários, aprová-la, etc. O [!DNL Workfront] recomenda que os padrões de função de prova sejam definidos para todos os usuários, para facilitar e agilizar a adição de destinatários às provas e a configuração de fluxos de trabalho.

![Funções de prova podem ser selecionadas ao fazer upload de uma prova](assets/proof-system-setups-proof-role-example.png)

No entanto, essa função de prova padrão pode ser alterada quando for feito o upload de provas individuais, garantindo que todos possam cumprir a função exigida no processo de revisão e aprovação.


## Definir funções de prova padrão

1. Selecione **Configurar** no [!UICONTROL Menu principal].
1. Selecione **Revisão e aprovação** no menu esquerdo.
1. Clique no botão ao lado da função de prova padrão desejada para tanto para novos usuários do [!DNL Workfront] como para usuários de prova convidados, no caso dos“destinatários designados” — qualquer pessoa que seja adicionada ao fluxo de trabalho de prova, manualmente ou por meio de um modelo de fluxo de trabalho.
1. Clique no botão ao lado da função de prova padrão desejada tanto para novos usuários do [!DNL Workfront] como para usuários de prova convidados, no caso dos usuários “não destinatários”. Estes são geralmente usuários do [!DNL Workfront] que têm acesso a uma prova, mas não são uma das pessoas com atribuição no fluxo de trabalho.
1. Salve as alterações.

![Configurações de revisão e aprovação no Workfront](assets/proof-system-setups-workfront-defaults.png)

Pense no que a maioria dos seus usuários e convidados devem fazer quando forem adicionados a um fluxo de trabalho de revisão. Esse deve ser o seu padrão.

## Práticas recomendadas

| Prática recomendada | Saiba por quê |
|---|---|
| Use Somente leitura ou Revisor para a configuração “Funções para não destinatários que abrirem uma prova de documento” no Workfront. | Todas as outras opções dessa configuração exigem que seja tomada uma decisão da prova, o que pode atrapalhar seu fluxo de trabalho de revisão. Geralmente, as pessoas que não são adicionadas ao fluxo de trabalho da revisão só precisam visualizar a prova ou fazer comentários, não precisam aprovar a prova; portanto, as opções “Somente leitura” ou “Revisor” são a sua melhor escolha.<br> <br>Observação: essa configuração fica no Menu principal do Workfront > Configuração > Revisão e Aprovação. |
