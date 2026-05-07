---
title: Entenda os processos de aprovação específicos do grupo
description: Saiba como admins de grupo podem criar ou editar processos de aprovação dos grupos que gerenciam.
feature: Approvals
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate
jira: KT-10017
hide: true
exl-id: 9986469c-b02f-48ac-b71e-055473a2855b
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-05T19:17:51.764Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 214
ht-degree: 100%

---

# Entenda os processos de aprovação específicos do grupo

Admins de sistema e de grupo podem criar processos de aprovação no [!DNL Workfront]. Admins de sistema podem criar processos para usar em todo o sistema do [!DNL Workfront] ou apenas para um grupo específico. Enquanto isso, admins de grupo podem criar ou editar processos somente para o grupo que gerenciam.

Para ter um processo de aprovação que possa ser usado por todos no [!DNL Workfront], verifique se o campo [!UICONTROL “Este processo de aprovação pode ser usado por”] está definido como [!UICONTROL Todos os grupos].

A janela ![[!UICONTROL Editar processo de aprovação] com o campo de grupo realçado](assets/admin-fund-approval-processes-1.png)

Os status disponíveis no menu [!UICONTROL “Iniciar processo de aprovação quando o status estiver definido como”] depende da opção selecionada no campo “usado por”. Se a opção [!UICONTROL Todos os grupos] estiver selecionada, somente os status bloqueados em todo o sistema estarão disponíveis.

Para limitar um processo de aprovação para um grupo específico, selecione o nome desse grupo na lista do campo [!UICONTROL “Este processo de aprovação pode ser usado por”].

A janela ![[!UICONTROL Editar processo de aprovação] com o campo de grupo expandido](assets/admin-fund-approval-processes-2.png)

A opção [!UICONTROL Todos os grupos] não está disponível para admins de grupo.

Quando um grupo específico é selecionado, somente os status disponíveis para esse grupo são exibidos no menu [!UICONTROL “Iniciar processo de aprovação quando o status estiver definido como”].

A janela ![[!UICONTROL Editar processo de aprovação] com o campo de status realçado](assets/admin-fund-approval-processes-3.png)
