---
title: Definir configurações de projeto padrão global
description: Saiba como alterar um status personalizado, definir preferências de projeto global e criar agendamentos que sejam configurações padrão globais.
feature: System Setup and Administration
role: Admin
level: Intermediate
activity: deploy
type: Tutorial
team: Technical Marketing
thumbnail: 335065.png
kt: 8753
exl-id: b961ba8c-9597-4ed4-a6d7-79689c8e290d
source-git-commit: adf12d7846d2a1b4c32513a3955c080905044576
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---

# Definir configurações de projeto padrão global

<!---
21.4 updates have been made
--->

Neste vídeo, você aprenderá a:

* Alterar um status personalizado
* Definir preferências de projeto global
* Criar e usar programações

>[!VIDEO](https://video.tv.adobe.com/v/335065/?quality=12)

## Configurações globais e de projeto, tarefa e emissão de grupo

Ao abrir o [!UICONTROL Projetos] configurações em [!DNL Workfront], você perceberá que diz &quot;[!UICONTROL Preferências de projeto do sistema]&quot; na barra de pesquisa na parte superior da janela. Isso permite que você saiba que essas configurações afetam todos na sua [!DNL Workfront] sistema — é uma configuração global.

![[!UICONTROL Preferências do projeto] em [!UICONTROL Configuração]](assets/admin-fund-system-project-preferences-1.png)

Você verá algo semelhante ao abrir o [!UICONTROL Tarefas e problemas] configurações.

![[!UICONTROL Preferências de tarefa e emissão] em [!UICONTROL Configuração]](assets/admin-fund-task-issue-preferences-2.png)

No entanto, é possível que nem todos os grupos no [!DNL Workfront] O precisa do mesmo projeto, tarefa e preferências de emissão. Por exemplo, o grupo de marketing deseja que o status de um novo projeto seja Planejamento, enquanto o grupo do gerenciador de projetos prefere o status Solicitação .

[!DNL Workfront] permite que os administradores de grupo ajustem determinados projetos, tarefas e emitam preferências para seus grupos. As preferências que podem ser ajustadas são determinadas pela variável [!DNL Workfront] administrador do sistema usando os botões de bloqueio/desbloqueio.

Comece navegando até o [!UICONTROL Configuração] Área:

1. Selecionar **[!UICONTROL Configuração]** no **[!UICONTROL Menu principal]**.
1. Expandir **[!UICONTROL Preferências do projeto]** no menu esquerdo.
1. Selecionar **[!UICONTROL Projetos]** ou **[!UICONTROL Tarefas e problemas]**, dependendo das configurações que deseja modificar.

Bloqueie uma preferência para impedir que os administradores de grupo ajustem essa configuração para seu grupo.

![Mensagem de preferência bloqueada](assets/admin-fund-preferences-locked-3.png)

Desbloqueie a preferência para disponibilizá-la para que os administradores de grupo personalizem.

![Mensagem de preferência desbloqueada](assets/admin-fund-preferences-unlocked-4.png)

Algumas configurações não podem ser desbloqueadas e continuar com as configurações globais do sistema.

![Mensagem de preferência bloqueada](assets/admin-fund-preferences-always-locked-5.png)

### Definir preferências de grupo e subgrupo

Para quaisquer configurações desbloqueadas pelo administrador do sistema, os administradores de grupo podem fazer ajustes para os grupos que gerenciam e para quaisquer subgrupos aninhados nesses grupos. Além disso, os administradores de grupo podem controlar quais configurações os administradores de subgrupo podem modificar.

1. Selecionar **[!UICONTROL Configuração]** no **[!UICONTROL Menu principal]**.
1. Clique em **[!DNL Groups]** no menu esquerdo.
1. Clique no nome do grupo ou subgrupo para abri-lo.
1. Selecionar **[!UICONTROL Preferências do projeto]** ou **[!UICONTROL Preferências de tarefas e problemas]** no menu esquerdo.
1. Faça as alterações necessárias para cada uma das preferências desbloqueadas.
1. Selecionar **[!UICONTROL Salvar]**.

![[!UICONTROL Status do projeto] seção sobre [!UICONTROL Grupo] página](assets/admin-fund-group-preferences.png)

Se sua organização não estiver usando administradores de grupo, o administrador do sistema poderá gerenciar as configurações de preferências para os diferentes grupos.

<!---
learn more URLs and guides
Create or edit a group status 
Group administrators 
Configure system-wide project preferences 
Configure project preferences for a group 
Configure task and issue preferences for a group 
Create and modify a group’s schedule 
--->
