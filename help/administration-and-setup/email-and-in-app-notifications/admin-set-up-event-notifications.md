---
title: Configurar notificações de eventos
description: Saiba como controlar quais emails e notificações no aplicativo os usuários recebem, gerenciando as notificações de eventos.
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
source-wordcount: '622'
ht-degree: 100%

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
>Devido à implementação em fases, a funcionalidade que permite que admins de sistema e de grupo gerenciem notificações de eventos está temporariamente indisponível para alguns clientes do [!DNL Workfront]. Siga este artigo para receber atualizações sobre a versão: “Desbloquear a configuração de notificações de eventos para grupos”.

Admins de sistema determinam quais notificações os usuários devem receber por meio do [!DNL Workfront].

A janela ![[!UICONTROL Notificações por email] na área [!UICONTROL Configuração]](assets/admin-fund-notifications-1.png)

A lista [!UICONTROL Notificações de eventos] é agrupada por tipo. Para cada notificação de evento listada, você verá cinco informações:

* **[!UICONTROL Ativo]:** a coluna [!UICONTROL Ativo] permite ativar ou desativar uma notificação em todo o sistema.
* **[!UICONTROL Nome]:** este é o nome da notificação dentro do [!DNL Workfront].
* **[!UICONTROL Descrição]:** a descrição fornece uma breve explicação sobre a ação que acionou a notificação ou que precisa ser tomada em resposta ao recebimento da notificação.
* **[!UICONTROL Assunto do email]:** o que será exibido ao usuário na linha de assunto quando o email for enviado.
* **[!UICONTROL Acesso ao grupo]:** desbloqueia as notificações, para que possam ser gerenciadas por admins de grupo.

## Ativar notificações

Para gerenciar notificações em todo o sistema, certifique-se de que a barra de pesquisa exiba [!UICONTROL Notificações de eventos do sistema].

Ative uma notificação específica para disponibilizá-la para todos os usuários, clicando no botão de alternância até que mostre uma cor azul. Se a cor do botão não estiver azul, a notificação está desativada.

Coluna ![[!UICONTROL Ativo] na página [!UICONTROL Notificações por email]](assets/admin-fund-notifications-2.png)

Quando uma notificação de evento é ativada, as mensagens são enviadas assim que o evento ocorre.

## Permitir controle de admins de grupo

Admins de grupo podem receber permissão de admins de sistema para personalizar ainda mais a lista de notificações com base em como seus grupos e subgrupos operam e em quais são seus fluxos de trabalho.

Coluna ![[!UICONTROL Acesso ao grupo] na página [!UICONTROL Notificações por email]](assets/ganotifications_01.png)

Para conceder a admins de grupo a capacidade de gerenciar as notificações de seus grupos e subgrupos, é preciso desbloquear as notificações em todo o sistema.

* Navegue até a guia “Notificação de eventos” da página “Notificações por email”.

* Certifique-se de que a barra de pesquisa exiba “Notificações de eventos do sistema”.

* Desbloqueie uma única notificação para todos os(as) admins de grupo clicando no botão de alternância da coluna “Acesso ao grupo” até que ele apresente uma cor azul.

* Desbloqueie várias notificações de uma vez marcando a caixa à esquerda de cada notificação e clicando no ícone de “cadeado aberto”, na barra de ferramentas acima da lista.

Coluna ![[!UICONTROL Acesso ao grupo] na página [!UICONTROL Notificações por email]](assets/ganotifications_02.png)

Bloqueie uma notificação desbloqueada clicando no botão de alternância até que ele apresente uma cor cinza. Bloqueie várias notificações ao mesmo tempo marcando as caixas de seleção e clicando no ícone de “cadeado aberto”, na barra de ferramentas.

Coluna ![[!UICONTROL Acesso ao grupo] na página [!UICONTROL Notificações por email]](assets/ganotifications_03.png)

As notificações desbloqueadas são exibidas a admins de grupo de nível superior para que determinem se tais notificações são necessárias para seus grupos e subgrupos. Os subgrupos herdam as configurações de notificação do grupo principal. ﻿


## Gerenciar notificações de grupo

Depois que o(a) admin de sistema desbloquear as opções de notificação, admins de grupo poderão gerenciar as notificações de um grupo na página individual do grupo, clicando em “Notificações de eventos” no menu do painel esquerdo. Em seguida, é possível ativar ou desativar as opções de notificação.

Coluna ![[!UICONTROL Acesso ao grupo] na página [!UICONTROL Notificações por email]](assets/managegroupnotifications_01.png)

Se necessário, admins de sistema podem gerenciar as notificações de um grupo na página “Notificações”, digitando o nome do grupo na barra de pesquisa na parte superior da janela.

Coluna ![[!UICONTROL Acesso ao grupo] na página [!UICONTROL Notificações por email]](assets/managegroupnotifications_02.png)

## Dicas profissionais

O [!DNL Workfront] recomenda disponibilizar algumas notificações para os usuários.

Para a maioria dos usuários:

* [!UICONTROL Quando uma tarefa for concluída, enviar email para os usuários atribuídos primariamente de todas as tarefas dependentes]
* [!UICONTROL Alguém me inclui em uma atualização direcionada]
* [!UICONTROL Alguém comenta no meu item de trabalho]
* [!UICONTROL A data de vencimento de uma tarefa à qual fui atribuído é alterada]


Especificamente para gerentes de projeto:

* [!UICONTROL Um projeto do qual participo é ativado]
* [!UICONTROL Quando um projeto for alterado de uma status positiva de progresso (no prazo) para uma status negativa de progresso (em atraso), enviar email para o proprietário do projeto]
* [!UICONTROL Quando um problema for adicionada enviar email para o proprietário do projeto]
* [!UICONTROL Uma tarefa marco foi concluída em um projeto de minha propriedade]

<!---
learn more URLs
--->
