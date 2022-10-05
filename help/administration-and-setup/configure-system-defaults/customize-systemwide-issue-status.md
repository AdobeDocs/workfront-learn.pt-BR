---
title: Personalizar status de problemas do sistema
description: Saiba como alterar nomes de status de problemas, controlar os tipos de problemas para os quais um status é usado e bloquear/desbloquear status para personalização em nível de grupo.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
kt: 10030
exl-id: c8f5677f-8d9d-4d1a-a1e3-d1a438878213
source-git-commit: 02bc5a09a838be6d98c9b746bff731236ee4116f
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# Personalizar status de todo o sistema

[!DNL Workfront] O fornece uma variedade de estatutos padrão para acomodar os workflows de gerenciamento de problemas de sua organização. Esses status podem ser renomeados para corresponder à terminologia de sua organização. E os status podem ser atribuídos a tipos de problema específicos.

Status adicionais podem ser criados, se necessário. Somente administradores de sistema podem criar status do sistema. Além disso, os administradores de sistema controlam quais status podem ser editados pelos administradores de grupo.

![[!UICONTROL Problemas] guia em [!UICONTROL Estatutos] em [!UICONTROL Configuração]](assets/admin-fund-all-issue-statuses.png)

## Modificar os status existentes

[!DNL Workfront] A recomenda um número mínimo de status. Isso facilita a escolha do status certo para os usuários e resulta em uma lista mais curta de status a serem mantidos.

É possível editar um status existente para alterar o nome, os tipos de problema aos quais ele é atribuído, a cor relacionada etc.

![Lista de status da ocorrência com [!UICONTROL Editar] opção realçada](assets/admin-fund-edit-issue-status.png)

1. Clique em **[!UICONTROL Configuração]** no **[!UICONTROL Menu principal]**.
1. Expanda o **[!UICONTROL Preferências do projeto]** no painel do menu esquerdo.
1. Selecionar **[!UICONTROL Status]**.
1. Selecione o **[!UICONTROL Problemas]** e certifique-se de [!UICONTROL Status do sistema] é exibido no canto superior direito.
1. Selecionar **[!UICONTROL Lista principal]** para ver os status de todos os tipos de problema. É aqui que você cria ou modifica um status de ocorrência.
1. Passe o mouse sobre o lado direito do status que deseja renomear e clique em **[!UICONTROL Editar]**.
1. Dê um novo nome ao status ou altere qualquer outra informação, conforme desejado.
1. Bloquear o status se essas configurações se aplicarem a todos os usuários em seu [!DNL Workfront] instância.
1. Desbloqueie o status para permitir que os administradores de grupo editem o status somente para seus grupos.
1. Marque as caixas do tipo de problema ao qual o status deve ser aplicado.
1. Clique em **[!UICONTROL Salvar]**.

![Janela para criar um novo status](assets/admin-fund-edit-issue-status-2.png)

### Atribuições de status

Nem todos os status podem ser atribuídos a todos os tipos de emissão. O [!UICONTROL Status] tem colunas mostrando para qual tipo de problema cada status pode ser usado.

![Alterar ordem realçada na guia Problemas da página Status](assets/admin-fund-issue-type-statuses.png)


Para ver apenas os status atribuídos a um tipo de problema específico, clique no nome do tipo de problema na parte superior da janela.

![[!UICONTROL Problema] guia de [!UICONTROL Status] página com colunas realçadas](assets/admin-fund-statuses-issue-type.png)

Aqui, você pode arrastar e soltar os problemas na ordem em que deseja que eles apareçam na [!UICONTROL Status] menu suspenso.

Para editar os status, você precisará voltar para o [!UICONTROL Lista principal].
