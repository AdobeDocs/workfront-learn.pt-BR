---
title: Configurar notificações de evento
description: Saiba como controlar quais e-mails e notificações no aplicativo os usuários recebem gerenciando notificações de eventos.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate
thumbnail: 10093.jpeg
kt: 10093
exl-id: 6bd3a777-0ed8-4383-ad8e-f1238e334e78
source-git-commit: 1f7a4da813805691fc0e52d3ad1ea708f9e07a9a
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 4%

---

<!---
this has the same content as the system administrator notification setup and mangement section of the email and inapp notificiations learning path
--->

<!---
add URL link in the note at the top of the LP
--->

# Configurar notificações de evento

>[!NOTE]
>
>Devido a uma implantação em fases, a funcionalidade que permite que administradores de sistema e grupo gerenciem notificações de eventos não está temporariamente disponível para alguns [!DNL Workfront] clientes. Siga este artigo para obter atualizações sobre a versão: Desbloqueie a configuração de notificações de eventos para grupos.

Os administradores do sistema determinam quais notificações os usuários devem receber por meio de [!DNL Workfront].

![[!UICONTROL Notificações por email] na janela [!UICONTROL Configuração] area](assets/admin-fund-notifications-1.png)

O [!UICONTROL Notificações de evento] é agrupada por tipo. Para cada notificação de evento listada, você verá cinco informações:

* **[!UICONTROL Ativo] —** O [!UICONTROL Ativo] permite ativar ou desativar uma notificação em todo o sistema.
* **[!UICONTROL Nome] —** Este é o nome da notificação no [!DNL Workfront].
* **[!UICONTROL Descrição] —** A descrição fornece uma breve explicação das medidas tomadas para desencadear uma notificação ou que devem ser tomadas em resposta à recepção da notificação.
* **[!UICONTROL Assunto do email] —** O que será exibido ao usuário na linha de assunto quando o email for enviado aos usuários.
* **[!UICONTROL Acesso de grupo] —** Desbloqueie notificações para que elas possam ser gerenciadas pelos administradores do grupo.

## Ativar notificações

Para gerenciar notificações em um nível de sistema global, verifique se a barra de pesquisa informa [!UICONTROL Notificações de evento do sistema].

Ative uma notificação específica para torná-la disponível para todos os usuários clicando no botão de alternância para que o azul seja exibido. Se o azul estiver oculto, a notificação ficará desativada.

![[!UICONTROL Ativo] coluna em [!UICONTROL Notificações por email] página](assets/admin-fund-notifications-2.png)

Quando uma notificação de evento é ativada, as mensagens são enviadas instantaneamente quando o evento ocorre.

## Permitir controle de administrador de grupo

Os administradores de grupo podem receber permissão, por administradores de sistema, para personalizar ainda mais a lista de notificação, com base em como seus grupos e subgrupos funcionam e quais são seus fluxos de trabalho.

![[!UICONTROL Acesso de grupo] coluna em [!UICONTROL Notificações por email] página](assets/ganotifications_01.png)

Para dar aos administradores de grupo a capacidade de gerenciar notificações de seus grupos e subgrupos, as notificações no nível do sistema precisam ser desbloqueadas.

* Navegue até a guia Notificação de eventos da página Notificações por email .

* Certifique-se de que a barra de pesquisa informe as Notificações de Eventos do Sistema.

* Desbloqueie uma única notificação para todos os administradores de grupo clicando no botão de alternância na coluna Acesso a grupo para que o azul apareça.

* Desbloqueie várias notificações de uma vez, marcando a caixa à esquerda de cada notificação e clicando no ícone de desbloqueio na barra de ferramentas acima da lista.

![[!UICONTROL Acesso de grupo] coluna em [!UICONTROL Notificações por email] página](assets/ganotifications_02.png)

Bloqueie uma notificação desbloqueada clicando no botão para que o cinza apareça. Bloqueie várias notificações ao mesmo tempo, marcando as caixas de seleção e clicando no ícone de desbloqueio na barra de ferramentas.

![[!UICONTROL Acesso de grupo] coluna em [!UICONTROL Notificações por email] página](assets/ganotifications_03.png)

As notificações desbloqueadas são exibidas para administradores de grupos de nível superior a fim de determinar se essa notificação é necessária para seus grupos e subgrupos. Os subgrupos herdam as configurações de notificação do grupo pai principal. ﻿


## Gerenciar notificações de grupo

Depois que o administrador do sistema tiver desbloqueado as opções de notificação, os administradores do grupo poderão gerenciar as notificações de um grupo na página Grupo individual, clicando em Notificações de evento no menu do painel esquerdo. Em seguida, é possível ativar ou desativar as opções de notificação.

![[!UICONTROL Acesso de grupo] coluna em [!UICONTROL Notificações por email] página](assets/managegroupnotifications_01.png)

Se necessário, os administradores do sistema podem gerenciar as notificações de um grupo na página Notificações, inserindo o nome do grupo na barra de pesquisa na parte superior da janela.

![[!UICONTROL Acesso de grupo] coluna em [!UICONTROL Notificações por email] página](assets/managegroupnotifications_02.png)

## Dicas Pro

Há algumas notificações [!DNL Workfront] A recomenda disponibilizar para seus usuários.

Para a maioria dos usuários:

* [!UICONTROL Quando uma tarefa for concluída, enviar email para os usuários atribuídos primariamente de todas as tarefas dependentes]
* [!UICONTROL Alguém tiver me incluído em uma atualização direcionada]
* [!UICONTROL Alguém comenta sobre meu item de trabalho]
* [!UICONTROL A data de vencimento muda em uma tarefa à qual estou atribuído]


Especificamente para os gestores de projeto:

* [!UICONTROL Um projeto em que estou torna-se ativo]
* [!UICONTROL Quando um projeto for alterado de uma status positiva de progresso (no prazo) para uma status negativa de progresso (em atraso), enviar email para o proprietário do projeto]
* [!UICONTROL Quando um problema for adicionada enviar email para o proprietário do projeto.]
* [!UICONTROL A tarefa de marco é concluída em um projeto que eu possuo]

<!---
learn more URLs
--->
