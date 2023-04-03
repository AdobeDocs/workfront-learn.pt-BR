---
title: Entender grupos e usuários em [!UICONTROL Workfront DAM]
description: Saiba como criar pastas, grupos e usuários no [!UICONTROL Workfront DAM]. Entenda os tipos de função do usuário e conceda permissões a pastas.
activity: use
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
team: Technical Marketing
kt: 8967
exl-id: 4ebf675c-b72d-447e-b131-a89acb449e15
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Configuração do sistema: grupos e usuários

Neste vídeo, você aprenderá a:

* Entenda como as configurações de grupo afetam o acesso aos ativos
* Criar pastas, grupos e usuários em uma ordem específica
* Entender os tipos de função do usuário
* Conceder permissões a pastas
* Criar e editar grupos
* Adicionar e editar usuários

>[!VIDEO](https://video.tv.adobe.com/v/335230/?quality=12&learn=on)

## Grupos e usuários revisam

Ao configurar seu [!UICONTROL Workfront DAM] , é importante considerar as funções que usuários e grupos desempenham no cenário geral.

Grupos controlam o acesso às pastas de ativos em [!UICONTROL Workfront DAM]. As configurações de grupo também controlam o que os usuários podem fazer com os ativos (exibir, baixar, editar, etc.) eles têm permissão de acesso.

Ao criar grupos, é vital ter em mente quais pastas de ativos os membros desse grupo precisarão acessar no [!UICONTROL Workfront DAM].

Os usuários são indivíduos que têm logon no [!UICONTROL Workfront DAM]. Um usuário não pode acessar nada em [!UICONTROL Workfront DAM] a menos que sejam atribuídos a um grupo. Os usuários podem pertencer a mais de um grupo, dependendo de suas necessidades.

## Grupos padrão

Há dois grupos padrão que vêm com [!UICONTROL Workfront DAM]. Todos os usuários pertencem a esses grupos automaticamente, com base no fato de terem ou não [!UICONTROL Workfront DAM] credenciais de logon. Não é possível adicionar ou remover usuários desses grupos:

* **Grupo de convidados**—Usado para controlar o acesso de um usuário anônimo. Pode ser alguém sem credenciais de logon ou um usuário que não está conectado no momento.
* **Registrado** Grupo -In - Todos os usuários conectados pertencem a esse grupo.

O grupo Administrador e suas configurações também existem por padrão. Você pode adicionar usuários a esse grupo, mas não pode ajustar as configurações.

## Tipos de função

À medida que grupos são criados, um tipo de função é atribuída a eles. O tipo de função determina qual parte do [!UICONTROL Workfront DAM] os usuários do sistema obtêm quando fazem login — [!UICONTROL Workfront DAM] por si só ou [!UICONTROL Conexão de marca].

Há três tipos de função disponíveis com [!UICONTROL Workfront DAM] licenças:

* **[!UICONTROL Brand Portal]**—Esses usuários têm acesso somente a [!UICONTROL Conexão de marca], que é o local onde eles podem visualizar e baixar ativos aprovados.
* **[!UICONTROL Colaborador]**—Esses usuários podem acessar [!UICONTROL Workfront DAM] e [!UICONTROL Conexão de marca]. Eles têm direitos de acesso total a ativos e pastas — exibir, baixar, carregar, editar, mover e excluir.
* **[!UICONTROL Administrador]**—Os administradores de sistema têm acesso a tudo em [!UICONTROL Conexão de marca] e [!UICONTROL Workfront DAM], além da capacidade de estabelecer as configurações globais do sistema para cada um. Eles também podem acessar ativos que expiraram ou que foram definidos como inativos.

<!-- 
Learn more graphic & documentation article link, below
* Understanding the difference between Workfront licenses and Workfront DAM role types
* -->
