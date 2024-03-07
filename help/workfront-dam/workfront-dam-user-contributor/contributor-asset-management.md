---
title: Entenda o gerenciamento de ativos como colaborador
description: Aprenda a gerenciar ativos no [!UICONTROL DAM do Workfront] para melhorar o seu fluxo de trabalho.
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8996
exl-id: a09d0b0e-2631-414e-87e6-385ddbeb5cd2
doc-type: video
source-git-commit: 2cb3cc67f4f1fcd1345f178bf525d7b00f6271cf
workflow-type: ht
source-wordcount: '460'
ht-degree: 100%

---

# Entenda o gerenciamento de ativos como colaborador

Neste vídeo, você aprenderá a:

* Usar o menu “Editar” de um ativo
* Definir uma data de vencimento
* Exibir notificações
* Estabelecer configurações de notificação individuais
* Fazer upload de uma versão de ativo
* Criar uma nova pasta
* Aplicar um modelo de metadados a uma pasta
* Estabelecer permissões de pasta

>[!VIDEO](https://video.tv.adobe.com/v/335256/?quality=12&learn=on)

## Como as versões de ativos funcionam

Parte do seu fluxo de trabalho pode incluir o gerenciamento de múltiplas versões (ou rodadas, provas, iterações, como desejar chamá-las) de um ativo. Você pode gerenciar todas as versões por meio do [!UICONTROL DAM do Workfront].

O sistema permite o controle automático de versões de ativos quando um arquivo com o mesmo nome de um arquivo existente é carregado na mesma pasta. Consulte o(a) admin de sistema para saber se essa funcionalidade foi ativada.

Se o controle automático de versão estiver ativado, o ativo só terá um controle de versão se for carregado na pasta que contém o ativo original. Ambos os ativos precisam ter o mesmo nome de arquivo. Se o ativo for carregado em uma pasta diferente, ele será inserido como um novo arquivo.
Se o controle de versão não estiver ativado, um arquivo com o mesmo nome de um arquivo já existente será enviado como um novo arquivo, independentemente da pasta em que ele seja inserido. Isso pode resultar na existência de dois ativos com o mesmo nome na mesma pasta.

Você também pode fazer o upload manual de versões de um ativo específico. Clique no ícone de edição do ativo e selecione **[!UICONTROL Fazer upload de nova versão]**.

Se você publicar um ativo com versões no Brand Connect, o usuário do Brand Connect verá somente a versão mais recente do ativo.

## Status e vencimento de pastas e ativos

Os status são outra maneira de gerenciar o acesso a pastas e ativos no [!UICONTROL DAM do Workfront]. Os status podem ser usados para ocultar determinados ativos ou pastas dos usuários do [!UICONTROL Brand Connect], ou para encerrar um ativo ou pasta, para que ninguém além do(a) admin de sistema possa acessá-los.

* **[!UICONTROL Ativo:]** usado para ativos e pastas. Ativos e pastas com o status [!UICONTROL Ativo] podem ser vistos por todos os usuários com permissão e podem ser publicados no [!UICONTROL Brand Connect]. O status [!UICONTROL Ativo] é indicado por um ponto verde em um ativo ou pasta.
* **[!UICONTROL Inativo:]** usado para ativos e pastas. Ativos e pastas com o status [!UICONTROL Inativo] podem ser vistos por usuários do [!UICONTROL DAM do Workfront], mas não são visíveis no [!UICONTROL Brand Connect]. O status [!UICONTROL Inativo] é indicado por um ponto vermelho em um ativo ou pasta.
* **[!UICONTROL Não expirado:]** usado apenas para ativos. Este é o status padrão de todos os ativos. Ativos não expirados que também possuem o status [!UICONTROL Ativo] são visíveis no [!UICONTROL Brand Connect].
* **[!UICONTROL Expirado:]** usado apenas para ativos. Ativos com o status [!UICONTROL Expirado] não podem ser baixados por nenhum usuário, exceto por admins de sistema. A visibilidade de ativos expirados no [!UICONTROL Brand Connect] depende das configurações do sistema.
