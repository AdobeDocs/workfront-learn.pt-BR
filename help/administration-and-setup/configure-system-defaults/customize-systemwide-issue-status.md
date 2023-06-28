---
title: Personalizar status de problemas em todo o sistema
description: Saiba como alterar nomes de status de problemas, controlar os tipos de problemas para os quais um status é usado e bloquear/desbloquear status para personalização em nível de grupo.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10030
exl-id: c8f5677f-8d9d-4d1a-a1e3-d1a438878213
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# Personalizar os status de todo o sistema

[!DNL Workfront] O fornece uma variedade de status padrão para acomodar os workflows de gerenciamento de problemas de sua organização. Esses status podem ser renomeados para corresponder à terminologia da sua organização. Os status e podem ser atribuídos a tipos de ocorrências específicos.

Status adicionais podem ser criados, se necessário. Somente administradores do sistema podem criar status de todo o sistema. Além disso, os administradores de sistema controlam quais status podem ser editados por administradores de grupo.

![[!UICONTROL Problemas] guia em [!UICONTROL Estátuas] página em [!UICONTROL Configuração]](assets/admin-fund-all-issue-statuses.png)

## Modificar status existentes

[!DNL Workfront] A recomenda um número mínimo de status. Isso facilita a escolha do status certo para os usuários e resulta em uma lista mais curta de status a serem mantidos.

É possível editar um status existente para alterar o nome, a que tipos de problemas ele está atribuído, a cor relacionada etc.

![Lista de status de problema com [!UICONTROL Editar] opção realçada](assets/admin-fund-edit-issue-status.png)

1. Clique em **[!UICONTROL Configuração]** no **[!UICONTROL Menu principal]**.
1. Expanda a **[!UICONTROL Preferências do projeto]** no painel do menu esquerdo.
1. Selecionar **[!UICONTROL Status]**.
1. Selecione o **[!UICONTROL Problemas]** e verifique se [!UICONTROL Status do sistema] é exibido no canto superior direito.
1. Selecionar **[!UICONTROL Lista principal]** para ver os status de todos os tipos de ocorrências. É aqui que você cria ou modifica um status de problema.
1. Passe o mouse sobre o lado direito do status que deseja renomear e clique em **[!UICONTROL Editar]**.
1. Dê um novo nome ao status ou altere qualquer outra informação, conforme desejado.
1. Bloqueie o status se estas configurações forem aplicáveis a todos os usuários em seu [!DNL Workfront] instância.
1. Desbloqueie o status para permitir que administradores de grupos editem o status somente para seus grupos.
1. Marque as caixas para o tipo de problema ao qual o status deve se aplicar.
1. Clique em **[!UICONTROL Salvar]**.

![Janela para criar um novo status](assets/admin-fund-edit-issue-status-2.png)

### Atribuições de status

Nem todos os status podem ser atribuídos a todos os tipos de problemas. A variável [!UICONTROL Status] A página tem colunas que mostram para qual tipo de problema cada status pode ser usado.

![Pedido de alteração destacado na guia Problemas da página Status](assets/admin-fund-issue-type-statuses.png)


Para ver apenas os status atribuídos a um tipo de ocorrência específico, clique no nome do tipo de ocorrência na parte superior da janela.

![[!UICONTROL Problema] guia de [!UICONTROL Status] página com colunas realçadas](assets/admin-fund-statuses-issue-type.png)

Aqui, você pode arrastar e soltar os problemas na ordem em que deseja que eles apareçam no [!UICONTROL Status] menu suspenso.

Para editar os status, será necessário voltar para a página [!UICONTROL Lista principal].
