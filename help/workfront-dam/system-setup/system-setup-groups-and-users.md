---
title: Entender grupos e usuários no [!UICONTROL DAM DO WORKFRONT]
description: Saiba como criar pastas, grupos e usuários no [!UICONTROL DAM DO WORKFRONT]. Entenda os tipos de função de usuário e conceda permissões para pastas.
activity: use
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
team: Technical Marketing
jira: KT-8967
exl-id: 4ebf675c-b72d-447e-b131-a89acb449e15
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Configuração do sistema: grupos e usuários

Neste vídeo, você aprenderá a:

* Entender como as configurações de grupo afetam o acesso a ativos
* Criar pastas, grupos e usuários em uma ordem específica
* Entender os tipos de função de usuário
* Conceder permissões a pastas
* Criar e editar grupos
* Adicionar e editar usuários

>[!VIDEO](https://video.tv.adobe.com/v/335230/?quality=12&learn=on)

## Revisão de grupos e usuários

À medida que você configura o [!UICONTROL DAM DO WORKFRONT] sistema, é importante considerar as funções que os usuários e grupos desempenham na visão geral.

Os grupos controlam o acesso às pastas de ativos no [!UICONTROL DAM DO WORKFRONT]. As configurações de grupo também controlam o que os usuários podem fazer com os ativos (exibir, baixar, editar etc.) eles têm permissão para acessar.

Ao criar grupos, é vital ter em mente quais pastas de ativos os membros desse grupo precisarão acessar no [!UICONTROL DAM DO WORKFRONT].

Os usuários são os indivíduos que têm logons no [!UICONTROL DAM DO WORKFRONT]. Um usuário não pode acessar nada no [!UICONTROL DAM DO WORKFRONT] a menos que estejam atribuídos a um grupo. Os usuários podem pertencer a mais de um grupo, dependendo de suas necessidades.

## Grupos padrão

Há dois grupos padrão que vêm com o [!UICONTROL DAM DO WORKFRONT]. Todos os usuários pertencem a esses grupos automaticamente, com base no fato de terem ou não [!UICONTROL DAM DO WORKFRONT] credenciais de logon. Não é possível adicionar ou remover usuários destes grupos:

* **Grupo convidado**—Usado para controlar o acesso de um usuário anônimo. Pode ser alguém sem credenciais de logon ou um usuário que não esteja conectado no momento.
* **Registrado**-No grupo — Todos os usuários conectados pertencem a este grupo.

O grupo Admin e suas configurações também existem por padrão. Você pode adicionar usuários a este grupo, mas não pode ajustar as configurações.

## Tipos de função

À medida que grupos são criados, eles recebem um tipo de função. O tipo de função determina qual parte da função [!UICONTROL DAM DO WORKFRONT] os usuários do sistema recebem quando fazem logon — [!UICONTROL DAM DO WORKFRONT] ele mesmo ou [!UICONTROL Conectar marca].

Há três tipos de função disponíveis com o [!UICONTROL DAM DO WORKFRONT] licenças:

* **[!UICONTROL Brand Portal]**— Esses usuários têm acesso somente a [!UICONTROL Conectar marca], que é onde eles podem visualizar e baixar os ativos aprovados.
* **[!UICONTROL Colaborador]**— Esses usuários podem acessar [!UICONTROL DAM DO WORKFRONT] e [!UICONTROL Conectar marca]. Eles têm direitos de acesso total a ativos e pastas — visualizar, baixar, fazer upload, editar, mover e excluir.
* **[!UICONTROL Administrador]**—Administradores do sistema têm acesso a tudo em [!UICONTROL Conectar marca] e [!UICONTROL DAM DO WORKFRONT], além da capacidade de estabelecer as configurações globais do sistema para cada um. Eles também podem acessar ativos que expiraram ou foram definidos como inativos.

<!-- 
Learn more graphic & documentation article link, below
* Understanding the difference between Workfront licenses and Workfront DAM role types
* -->
