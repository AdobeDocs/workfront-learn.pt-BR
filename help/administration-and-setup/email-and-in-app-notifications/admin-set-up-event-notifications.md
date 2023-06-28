---
title: Configurar notificações de eventos
description: Saiba como controlar quais emails e notificações no aplicativo os usuários recebem gerenciando notificações de eventos.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate
thumbnail: 10093.jpeg
jira: KT-10093
exl-id: 6bd3a777-0ed8-4383-ad8e-f1238e334e78
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
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

# Configurar notificações de eventos

>[!NOTE]
>
>Devido a uma implantação em fases, a funcionalidade que permite aos administradores de sistema e grupo gerenciar notificações de eventos não está disponível temporariamente para alguns [!DNL Workfront] clientes. Siga este artigo para obter atualizações sobre a versão: Desbloquear a configuração de notificações de eventos para grupos.

Os administradores do sistema determinam quais notificações os usuários devem receber por meio do [!DNL Workfront].

![[!UICONTROL Notificações por email] na janela [!UICONTROL Configuração] área](assets/admin-fund-notifications-1.png)

A variável [!UICONTROL Notificações de Eventos] é agrupada por tipo. Para cada notificação de evento listada, você verá cinco informações:

* **[!UICONTROL Ativo] —** A variável [!UICONTROL Ativo] permite ativar ou desativar uma notificação em um nível do sistema.
* **[!UICONTROL Nome] —** Este é o nome da notificação em [!DNL Workfront].
* **[!UICONTROL Descrição] —** A descrição fornece uma breve explicação de qual ação ocorreu para acionar uma notificação ou precisa ser executada em resposta ao recebimento da notificação.
* **[!UICONTROL Assunto do email] —** O que será exibido ao usuário na linha de assunto quando o email for enviado aos usuários.
* **[!UICONTROL Acesso de grupo] —** Desbloqueie as notificações para que elas possam ser gerenciadas por administradores de grupo.

## Ativar notificações

Para gerenciar notificações em um nível de sistema global, verifique se a barra de pesquisa diz [!UICONTROL Notificações de Eventos do Sistema].

Ative uma notificação específica para disponibilizá-la a todos os usuários clicando no botão de alternância para que o azul seja exibido. Se o azul estiver oculto, a notificação estará desativada.

![[!UICONTROL Ativo] coluna em [!UICONTROL Notificações por email] página](assets/admin-fund-notifications-2.png)

Quando uma notificação de evento é ativada, as mensagens são enviadas instantaneamente quando o evento ocorre.

## Permitir controle de administrador de grupo

Os administradores de grupo podem receber permissão, por administradores de sistema, para personalizar ainda mais a lista de notificações com base em como seus grupos e subgrupos funcionam e quais são seus workflows.

![[!UICONTROL Acesso de grupo] coluna em [!UICONTROL Notificações por email] página](assets/ganotifications_01.png)

Para conceder aos administradores de grupos a capacidade de gerenciar notificações para seus grupos e subgrupos, as notificações no nível do sistema precisam ser desbloqueadas.

* Navegue até a guia Notificação de Eventos da página Notificações por Email.

* Certifique-se de que a barra de pesquisa diga Notificações de eventos do sistema.

* Desbloqueie uma única notificação para todos os administradores de grupo clicando na alternância na coluna Acesso de grupo para que o azul apareça.

* Desbloqueie várias notificações de uma vez, marcando a caixa à esquerda de cada notificação e clicando no ícone de desbloqueio na barra de ferramentas acima da lista.

![[!UICONTROL Acesso de grupo] coluna em [!UICONTROL Notificações por email] página](assets/ganotifications_02.png)

Bloqueie uma notificação desbloqueada clicando no botão de alternância para que a cor cinza apareça. Bloquear várias notificações ao mesmo tempo marcando as caixas de seleção e clicando no ícone de desbloqueio na barra de ferramentas.

![[!UICONTROL Acesso de grupo] coluna em [!UICONTROL Notificações por email] página](assets/ganotifications_03.png)

As notificações desbloqueadas são exibidas para administradores de grupos de nível superior para determinar se essa notificação é necessária para seus grupos e subgrupos. Os subgrupos herdam as configurações de notificação do grupo principal. ﻿


## Gerenciar notificações de grupo

Depois que o administrador do sistema tiver desbloqueado as opções de notificação, os administradores de grupo poderão gerenciar as notificações de um grupo na página Grupo individual, clicando em Notificações de evento no menu do painel esquerdo. Em seguida, você poderá ativar ou desativar as opções de notificação.

![[!UICONTROL Acesso de grupo] coluna em [!UICONTROL Notificações por email] página](assets/managegroupnotifications_01.png)

Se necessário, os administradores do sistema podem gerenciar as notificações de um grupo na página Notificações digitando o nome do grupo na barra de pesquisa na parte superior da janela.

![[!UICONTROL Acesso de grupo] coluna em [!UICONTROL Notificações por email] página](assets/managegroupnotifications_02.png)

## Dicas profissionais

Há algumas notificações [!DNL Workfront] A recomenda disponibilizar o para seus usuários.

Para a maioria dos usuários:

* [!UICONTROL Quando uma tarefa for concluída, enviar email para os usuários atribuídos primariamente de todas as tarefas dependentes]
* [!UICONTROL Alguém tiver me incluído em uma atualização direcionada]
* [!UICONTROL Quando alguém comentar no meu item de trabalho, envie email para os atribuídos]
* [!UICONTROL A data de conclusão de uma tarefa atribuída a mim mudou]


Especificamente para gerentes de projeto:

* [!UICONTROL Quando uma status de projeto for alterada de ideia/aprovado/solicitado/em planejamento para atual, enviar email para a equipe]
* [!UICONTROL Quando um projeto for alterado de uma status positiva de progresso (no prazo) para uma status negativa de progresso (em atraso), enviar email para o proprietário do projeto]
* [!UICONTROL Quando um problema for adicionada enviar email para o proprietário do projeto.]
* [!UICONTROL Quando uma etapa for concluída, enviar email para o proprietário do projeto]

<!---
learn more URLs
--->
