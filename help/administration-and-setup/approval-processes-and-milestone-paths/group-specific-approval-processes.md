---
title: Entender os processos de aprovação específicos de grupo
description: Saiba como os administradores de grupo podem criar ou editar processos de aprovação para os grupos que gerenciam.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate
jira: KT-10017
exl-id: 138989b2-32d7-43e5-9660-d7b4172f232a
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 0%

---

# Entender os processos de aprovação específicos de grupo

Os administradores de sistema e de grupo podem criar processos de aprovação no [!DNL Workfront]. Os administradores do sistema podem criar processos para uso em todo o [!DNL Workfront] sistema ou apenas para um grupo específico. Os administradores de grupo podem criar ou editar processos somente para o grupo que gerenciam.

Para um processo de aprovação que pode ser usado por todos no [!DNL Workfront], verifique se [!UICONTROL &quot;Este processo de aprovação pode ser usado por&quot;] o campo está definido como [!UICONTROL Todos os grupos].

![[!UICONTROL Editar processo de aprovação] janela com o campo de grupo realçado](assets/admin-fund-approval-processes-1.png)

Os status disponíveis na variável [!UICONTROL &quot;Iniciar processo de aprovação quando o status estiver definido como&quot;] depende da seleção no campo &quot;usado por&quot;. Com [!UICONTROL Todos os grupos] selecionada, somente os status bloqueados em todo o sistema estarão disponíveis.

Para limitar um processo de aprovação para um grupo específico, selecione o nome desse grupo na lista da [!UICONTROL &quot;Este processo de aprovação pode ser usado por&quot;] campo.

![[!UICONTROL Editar processo de aprovação] janela com campo de grupo expandido](assets/admin-fund-approval-processes-2.png)

A variável [!UICONTROL Todos os grupos] opção não está disponível para administradores de grupo.

Quando um grupo específico é selecionado, somente os status disponíveis para esse grupo são exibidos no [!UICONTROL &quot;Iniciar processo de aprovação quando o status estiver definido como&quot;] menu.

![[!UICONTROL Editar processo de aprovação] janela com o campo de status realçado](assets/admin-fund-approval-processes-3.png)

