---
title: Definir as configurações globais padrão do projeto
description: Saiba como alterar um status personalizado, definir as preferências globais do projeto e criar agendas como configurações globais padrão.
feature: System Setup and Administration
role: Admin
level: Intermediate
activity: deploy
type: Tutorial
team: Technical Marketing
thumbnail: 335065.png
jira: KT-8753
exl-id: b961ba8c-9597-4ed4-a6d7-79689c8e290d
doc-type: video
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: ht
source-wordcount: '379'
ht-degree: 100%

---

# Definir as configurações globais padrão do projeto

<!---
21.4 updates have been made
--->

Neste vídeo, você aprenderá a:

* Alterar um status personalizado
* Definir as preferências globais do projeto
* Criar e usar agendas

>[!VIDEO](https://video.tv.adobe.com/v/335065/?quality=12&learn=on&enablevpops)

## Configurações de projetos, tarefas e problemas globais e de grupos

Quando abrir as configurações dos [!UICONTROL projetos] no [!DNL Workfront], você notará a mensagem “[!UICONTROL Preferências do projeto do sistema]” na barra de pesquisa, na parte superior da janela. Isso indica que essas configurações afetam todos os usuários do sistema do [!DNL Workfront], ou seja, é uma configuração global.

Página ![[!UICONTROL Preferências do projeto] em [!UICONTROL Configuração]](assets/admin-fund-system-project-preferences-1.png)

Você verá algo semelhante ao abrir as configurações de [!UICONTROL Tarefas e problemas].

![[!UICONTROL Preferências de tarefas e problemas] em [!UICONTROL Configuração]](assets/admin-fund-task-issue-preferences-2.png)

No entanto, é possível que nem todos os grupos no [!DNL Workfront] precisem das mesmas preferências de projetos, tarefas e problemas. Por exemplo, o grupo de marketing deseja que o status de um novo projeto seja “Planejamento”, enquanto o grupo de gerentes de projetos prefere o status “Solicitação”.

O [!DNL Workfront] permite que admins de grupo ajustem determinadas preferências de projetos, tarefas e problemas para seus grupos. As preferências que podem ser ajustadas são determinadas por admins de sistema do [!DNL Workfront], usando os botões “bloquear/desbloquear”.

Comece navegando até a área [!UICONTROL Configuração]:

1. Selecione **[!UICONTROL Configuração]** no **[!UICONTROL Menu principal]**.
1. Expanda **[!UICONTROL Preferências do projeto]** no menu esquerdo.
1. Selecione **[!UICONTROL Projetos]** ou **[!UICONTROL Tarefas e problemas]**, dependendo das configurações que você deseja modificar.

Bloqueie uma preferência para impedir que admins de grupo ajustem essa configuração em seus grupos.

![Mensagem de preferência bloqueada](assets/admin-fund-preferences-locked-3.png)

Desbloqueie a preferência para permitir que admins de grupo a personalizem.

![Mensagem de preferência desbloqueada](assets/admin-fund-preferences-unlocked-4.png)

Algumas configurações não podem ser desbloqueadas e permanecem como configurações globais do sistema.

![Mensagem de preferência bloqueada](assets/admin-fund-preferences-always-locked-5.png)

### Definir preferências de grupo e subgrupo

Admins de grupo podem ajustar configurações desbloqueadas por admins de sistema nos grupos que gerenciam e em quaisquer subgrupos aninhados. Além disso, admins de grupo podem controlar quais configurações admins de subgrupo podem modificar.

1. Selecione **[!UICONTROL Configuração]** no **[!UICONTROL Menu principal]**.
1. Clique em **[!DNL Groups]** no menu esquerdo.
1. Clique no nome do grupo ou subgrupo para abri-lo.
1. Selecione **[!UICONTROL Preferências do projeto]** ou **[!UICONTROL Preferências de tarefas e problemas]** no menu esquerdo.
1. Faça as alterações necessárias em cada uma das preferências desbloqueadas.
1. Selecione **[!UICONTROL Salvar]**.

Seção ![[!UICONTROL Status do projeto] na página [!UICONTROL Grupo]](assets/admin-fund-group-preferences.png)

Se a sua organização não utiliza admins de grupo, o(a) admin de sistema poderá gerenciar as preferências dos diferentes grupos.

<!---
learn more URLs and guides
Create or edit a group status 
Group administrators 
Configure system-wide project preferences 
Configure project preferences for a group 
Configure task and issue preferences for a group 
Create and modify a group’s schedule 
--->
