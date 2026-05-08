---
title: Personalize os status de problemas em todo o sistema
description: Saiba como alterar os nomes dos status de problemas, controlar os tipos de problema para os quais um status é usado e bloquear/desbloquear status para personalização na camada dos grupos.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10030
exl-id: c8f5677f-8d9d-4d1a-a1e3-d1a438878213
TQID: https://experienceleague.adobe.com/Wo7ObQJmkrsaYDXxaPMYQvDFfQx8wtC8qYi3Nvc6DkY
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 392
ht-degree: 100%

---

# Personalize os status de todo o sistema

O [!DNL Workfront] fornece uma variedade de status padrão para acomodar os fluxos de trabalho de gerenciamento de problemas da sua organização. Esses status podem ser renomeados de acordo com a terminologia da sua organização. E os status podem ser atribuídos a tipos de problema específicos.

Status adicionais podem ser criados, se necessário. Somente os administradores do sistema podem criar status para todo o sistema. Além disso, os administradores do sistema controlam quais status podem ser editados pelos administradores de grupos.

Guia ![[!UICONTROL Problemas] na página [!UICONTROL Status], em [!UICONTROL Configuração]](assets/admin-fund-all-issue-statuses.png)

## Modificar status existentes

O [!DNL Workfront] recomenda uma quantidade mínima de status. Isso facilita a escolha do status certo para os usuários e resulta em uma lista mais curta de status a serem mantidos.

É possível editar um status existente para alterar o nome, a que tipos de problema ele está atribuído, a cor relacionada etc.

![Lista de status de problemas com a opção [!UICONTROL Editar] realçada](assets/admin-fund-edit-issue-status.png)

1. Clique em **[!UICONTROL Configuração]** no **[!UICONTROL Menu principal]**.
1. Expanda a seção **[!UICONTROL Preferências do projeto]** no painel do menu esquerdo.
1. Selecione **[!UICONTROL Status]**.
1. Selecione a guia **[!UICONTROL Problemas]** e verifique se [!UICONTROL Status do sistema] aparece no canto superior direito.
1. Selecione **[!UICONTROL Lista principal]** para ver os status de todos os tipos de problema. É aqui que você cria ou modifica um status de problema.
1. Passe o mouse sobre o lado direito do status que deseja renomear e clique em **[!UICONTROL Editar]**.
1. Dê um novo nome ao status ou altere qualquer outra informação, conforme desejado.
1. Bloqueie o status, se essas configurações se aplicarem a todos os usuários da sua instância do [!DNL Workfront].
1. Desbloqueie o status, para permitir que os administradores de grupos editem o status somente para seus grupos.
1. Marque as caixas para o tipo de problema ao qual o status deve se aplicar.
1. Clique em **[!UICONTROL Salvar]**.

![Janela de criação de um novo status](assets/admin-fund-edit-issue-status-2.png)

### Atribuições de status

Nem todos os status podem ser atribuídos a todos os tipos de problema. A página [!UICONTROL Status] possui colunas que mostram para qual tipo de problema cada status pode ser usado.

![Pedido de alteração realçado na guia “Problemas” da página “Status”](assets/admin-fund-issue-type-statuses.png)


Para ver apenas os status atribuídos a um tipo de problema específico, basta clicar no nome do tipo de problema, na parte superior da janela.

Guia ![[!UICONTROL Problema] na página [!UICONTROL Status] com colunas realçadas](assets/admin-fund-statuses-issue-type.png)

Aqui, você pode arrastar e soltar os problemas na ordem em que deseja que apareçam no menu suspenso [!UICONTROL Status].

Para editar os status, você precisará voltar à [!UICONTROL Lista principal].
