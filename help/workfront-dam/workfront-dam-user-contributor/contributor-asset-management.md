---
title: Saiba como gerenciar ativos no [!UICONTROL Workfront DAM]
description: Saiba como gerenciar ativos no [!UICONTROL Workfront DAM] para melhorar o fluxo de trabalho.
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8996
exl-id: a09d0b0e-2631-414e-87e6-385ddbeb5cd2
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# Colaborador: gerenciamento de ativos

Neste vídeo, você aprenderá a:

* Usar o menu Editar em um ativo
* Definir uma data de expiração
* Exibir notificações
* Estabelecer configurações de notificação individual
* Fazer upload de uma versão de ativo
* Criar uma nova pasta
* Aplicar um modelo de metadados a uma pasta
* Estabelecer permissões de pasta

>[!VIDEO](https://video.tv.adobe.com/v/335256/?quality=12)

## Como as versões de ativos funcionam

Parte do fluxo de trabalho pode incluir o gerenciamento de várias versões, ou arredondamentos, provas, iterações, o que você chamar de ativo. Você pode gerenciar todas as versões por meio de [!UICONTROL Workfront DAM].

O sistema permite o controle automático da versão do ativo quando um arquivo com o mesmo nome de um arquivo existente é carregado na mesma pasta. Consulte o administrador do sistema para verificar se essa funcionalidade foi ativada.

Se o controle de versão automático estiver ativado, um ativo terá a versão somente se for carregado na pasta que contém o ativo original. Ambos os ativos devem ter o mesmo nome de arquivo. Se o ativo for carregado em uma pasta diferente, ele entrará como um novo arquivo.
Se o controle de versão não estiver ativado, um arquivo com o mesmo nome de um arquivo existente será carregado como um novo arquivo, independentemente da pasta em que ele for colocado. Isso pode resultar em ter dois ativos com o mesmo nome na mesma pasta.

Você também pode fazer upload manual de versões de um ativo específico. Clique no ícone de edição no ativo e selecione **[!UICONTROL Fazer upload de nova versão]**.

Se você publicar um ativo com versões no Brand Connect, o usuário do Brand Connect visualizará apenas a versão mais recente do ativo.

## Status e expiração da pasta e do ativo

Os status são outra maneira de gerenciar o acesso a pastas e ativos no [!UICONTROL Workfront DAM]. Os status podem ser usados para ocultar determinados ativos ou pastas de [!UICONTROL Conexão de marca] ou para expirar um ativo ou uma pasta para que ninguém, exceto o administrador do sistema, possa acessá-lo.

* **[!UICONTROL Ativo]**—Usado para ativos e pastas. Ativos e pastas com a [!UICONTROL Ativo] estão visíveis para todos os usuários com permissões e podem ser publicados em [!UICONTROL Conexão de marca]. [!UICONTROL Ativo] é indicado com um ponto verde em um ativo ou pasta.
* **[!UICONTROL Inativo]**—Usado para ativos e pastas. Ativos e pastas com a [!UICONTROL Inativo] status são visíveis para [!UICONTROL Workfront DAM] , mas não são visíveis na variável [!UICONTROL Conexão de marca]. [!UICONTROL Inativo] é indicado com um ponto vermelho em um ativo ou pasta.
* **[!UICONTROL Não expirado]**—Usado somente para ativos. Esse é o status padrão de todos os ativos. Ativos não expirados que também [!UICONTROL Ativo] são visíveis no [!UICONTROL Conexão de marca].
* **[!UICONTROL Expirado]**—Usado somente para ativos. Ativos com a [!UICONTROL Expirado] não pode ser baixado por nenhum usuário, exceto pelo administrador do sistema. Os ativos expirados são visíveis/não são visíveis na variável [!UICONTROL Conexão de marca], dependendo das configurações do sistema.
