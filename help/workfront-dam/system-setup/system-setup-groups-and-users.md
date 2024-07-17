---
title: Configurar grupos e usuários
description: Aprenda como criar pastas, grupos e usuários no [!UICONTROL Workfront DAM]. Entenda os tipos de funções do usuário e conceda permissões às pastas.
activity: use
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
team: Technical Marketing
jira: KT-8967
exl-id: 4ebf675c-b72d-447e-b131-a89acb449e15
doc-type: video
source-git-commit: 6c31f8d2e98ad8cd1880cd03ec0b0e6c0fd9ec09
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 100%

---

# Configurar grupos e usuários

Neste vídeo, você aprenderá a:

* Entenda como as configurações de grupo afetam o acesso a ativos
* Crie pastas, grupos e usuários em uma ordem específica
* Entenda os tipos de função de usuário
* Conceda permissões a pastas
* Crie e edite grupos
* Adicione e edite usuários

>[!VIDEO](https://video.tv.adobe.com/v/335230/?quality=12&learn=on)

## Revisão de grupos e usuários

À medida que você configura seu sistema do [!UICONTROL DAM do Workfront], é importante considerar as funções que os usuários e grupos desempenham no quadro geral.

Os grupos controlam o acesso às pastas de ativos no [!UICONTROL Workfront DAM]. As configurações de grupo também controlam o que os usuários podem fazer com os ativos (visualizar, baixar, editar etc.) que eles têm permissão para acessar.

Ao criar grupos, é vital ter em mente quais pastas de ativos os membros desse grupo precisarão acessar no [!UICONTROL DAM do Workfront].

Usuários são os indivíduos com logons para o [!UICONTROL Workfront DAM]. Eles não podem acessar nada no [!UICONTROL Workfront DAM] a menos que sejam atribuídos a um grupo. Os usuários podem pertencer a mais de um grupo, dependendo das necessidades.

## Grupos padrão

Existem dois grupos padrão que vêm com o [!UICONTROL Workfront DAM]. Todos os usuários pertencem a esses grupos automaticamente, com base no fato de terem as credenciais de logon do [!UICONTROL Workfront DAM]. Não é possível adicionar ou remover usuários destes grupos:

* **Grupo de convidados**: usado para controlar o acesso de um usuário anônimo. Pode ser alguém sem credenciais de logon ou usuários que não estejam conectados no momento.
* Grupo com **logon**: todos os usuários que estão logados pertencem a este grupo.

O grupo Administrador e suas configurações também existem por padrão. Você pode adicionar usuários a este grupo, mas não pode ajustar as configurações.

## Tipos de função

À medida que os grupos são criados, um tipo de função é atribuído a eles. O tipo de função determina qual parte do [!UICONTROL Workfront DAM] os usuários do sistema obtêm quando fazem logon – se é o próprio [!UICONTROL Workfront DAM] ou o [!UICONTROL Brand Connect].

Existem três tipos de função disponíveis com as licenças do [!UICONTROL Workfront DAM]:

* **[!UICONTROL Brand Portal]**: esses usuários têm acesso apenas ao [!UICONTROL Brand Connect], onde eles podem visualizar e fazer download dos ativos aprovados.
* **[!UICONTROL Colaborador]**: esses usuários podem acessar o [!UICONTROL Workfront DAM] e o [!UICONTROL Brand Connect]. Eles têm direito ao acesso total a ativos e pastas: visualizar, baixar, fazer upload, editar, mover e excluir.
* **[!UICONTROL Administradores]**: os administradores do sistema têm acesso a tudo, tanto no [!UICONTROL Brand Connect] quanto no [!UICONTROL Workfront DAM], além da capacidade de estabelecer as configurações globais do sistema para cada um. Eles também podem acessar ativos que expiraram ou foram definidos como inativos.

<!-- 
Learn more graphic & documentation article link, below
* Understanding the difference between Workfront licenses and Workfront DAM role types
* -->
