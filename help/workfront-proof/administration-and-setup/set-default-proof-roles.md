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
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 52%

---

# Definir funções de prova padrão



A primeira configuração padrão a ser concluída é determinar uma função de prova padrão que será atribuída quando novos usuários forem criados ou as pessoas abrirem uma prova.

As funções de prova determinam o que um usuário é capaz de fazer com uma prova: somente leitura, fazer comentários, aprová-la, etc. O [!DNL Workfront] recomenda que os padrões de função de prova sejam definidos para todos os usuários, para facilitar e agilizar a adição de destinatários às provas e a configuração de fluxos de trabalho.

![Funções de prova podem ser selecionadas ao fazer upload de uma prova](assets/proof-system-setups-proof-role-example.png)

No entanto, essa função de prova padrão pode ser alterada quando for feito o upload de provas individuais, garantindo que todos possam cumprir a função exigida no processo de revisão e aprovação.


## Definir funções de prova padrão

1. Selecione **Configurar** no [!UICONTROL Menu principal].
1. Selecione **Revisão e aprovação** no menu esquerdo.
1. Clique no botão ao lado da função de prova padrão desejada para novos [!DNL Workfront] usuários e usuários convidados de prova para &quot;recipients designados&quot; — qualquer pessoa adicionada ao fluxo de trabalho de prova, manualmente ou por meio de um template de fluxo de trabalho.
1. Clique no botão ao lado da função de prova padrão desejada para novos [!DNL Workfront] usuários e usuários de prova de convidado para usuários &quot;não destinatários&quot;. Em geral, [!DNL Workfront] usuários que têm acesso a uma prova, mas não são uma das pessoas atribuídas ao fluxo de trabalho.
1. Salve as alterações.

![Configurações de revisão e aprovação no Workfront](assets/proof-system-setups-workfront-defaults.png)

Pense no que a maioria dos seus usuários e convidados devem fazer quando forem adicionados a um fluxo de trabalho de revisão. Esse deve ser o seu padrão.

## Práticas recomendadas

| Prática recomendada | Aqui está o porquê |
|---|---|
| Use somente leitura ou Revisor para a configuração &quot;Funções para não destinatários que abrem uma prova de documento&quot; no Workfront. | As outras opções dessa configuração exigem que seja tomada uma decisão de prova, o que pode prejudicar seu fluxo de trabalho de prova. Geralmente, as pessoas que não são adicionadas ao fluxo de trabalho de prova precisam apenas visualizar a prova ou fazer comentários, não aprovar realmente a prova, portanto, as opções Somente leitura ou Revisor são a melhor opção. <br> <br>Observação: essa configuração é encontrada no Menu principal do Workfront > Configuração > Revisão e Aprovação. |
