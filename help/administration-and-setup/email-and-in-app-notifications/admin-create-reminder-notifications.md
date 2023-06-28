---
title: Configurar Notificações de Lembrete
description: Saiba como configurar notificações de lembrete específicas de objeto para informar aos usuários quando o trabalho vence em breve ou está vencido.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner
thumbnail: setupremindnote.png
jira: KT-10091
exl-id: f1ba58d7-3226-4c62-8aa4-40f88495b833
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---

<!---
this has the same content as the system administrator notification setup and mangement section of the email and inapp notificiations learning path
--->

# Configurar notificações de lembrete

Notificações de lembrete são criadas por administradores do sistema no [!UICONTROL Configuração] área. Em seguida, eles podem ser anexados e usados pelos proprietários de projetos, tarefas e problemas como lembretes de quando o trabalho vence em breve ou está vencido.

Os lembretes são específicos do objeto e devem ser anexados manualmente ao item de trabalho correspondente para que a notificação possa ser enviada.

**Criar uma notificação de lembrete**

1. Clique em **[!UICONTROL Configuração]** no **[!UICONTROL Menu principal]**.
1. Clique em **[!UICONTROL E-mail]** seção.
1. Clique em **[!UICONTROL Notificação]** seção.
1. Clique em **[!UICONTROL Novo lembrete]** guia.
1. Clique em **[!UICONTROL +Nova Notificação de Lembrete]** botão.
1. Selecione o objeto desejado no menu suspenso.
1. Preencha as informações necessárias.
1. Clique em **[!UICONTROL Salvar]**.

![[!UICONTROL Nova Notificação de Lembrete] janela](assets/admin-fund-reminder-notification-1.png)

Ao configurar o lembrete, há algumas coisas a serem consideradas:

* **[!UICONTROL Nome da Notificação de Lembrete] —** Esse é o nome que será visto pelos gerentes de projeto quando eles anexarem um lembrete a um objeto. Verifique se o nome é sucinto, mas descritivo.
* **[!UICONTROL Período de qualificação] —** O número de horas, dias, semanas ou meses antes/depois da data selecionada na seção Intervalo.
* **[!UICONTROL Tempo] —** Selecione se o lembrete deve ser enviado antes ou depois das datas planejadas, projetadas ou reais de início/término do objeto. As opções de folhas de horas estão relacionadas à data inicial, data final ou data da última atualização.
* **[!UICONTROL Critérios] —** Especifique os critérios para qualificar o lembrete a ser enviado. As opções variam dependendo do lembrete específico do objeto.
* **[!UICONTROL Destinatários] —** Selecione para quem o lembrete deve ser enviado. As opções da parte interessada variam dependendo do tipo de objeto selecionado para o lembrete.

Depois que as configurações de lembrete tiverem sido estabelecidas e salvas, a notificação de lembrete estará disponível para os proprietários do objeto usarem no [!DNL Workfront].

## Personalização de email

As notificações de lembrete usam um formato de email e uma mensagem padrão. Se quiser personalizar o email, crie um template.

<!---
paragraph above needs a hyperlink to an article
--->

![Janela Novo modelo de email](assets/admin-fund-email-customization.png)

<!---
learn more URLs
--->
