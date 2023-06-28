---
title: Entender o log de auditoria do sistema
description: Saiba como usar o log de auditoria do sistema para revisar quando as alterações foram feitas e quando os itens serão adicionados.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner, Intermediate
thumbnail: 10040.jpeg
jira: KT-10040
exl-id: 9de6fd40-10fb-47a6-b186-3a38c411f1ac
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---

# Entender o log de auditoria do sistema

O log de auditoria do sistema é a melhor maneira para o administrador do sistema acompanhar o que está acontecendo no [!DNL Workfront]. Pense no log como sua fonte de verdade para quem fez o que muda e quando.

Acesse o log de auditoria acessando o [!UICONTROL Preferências] na seção [!UICONTROL Configuração] área. Por padrão, você vê dados dos últimos sete dias. Altere os critérios de filtro para ver os dados de intervalos de datas diferentes.

Quando um usuário executa determinadas ações, [!UICONTROL Workfront] registra-os na variável [!UICONTROL Logs de auditoria] seção do [!UICONTROL Configuração] área.

![[!UICONTROL Tipo de log] menu suspenso no [!UICONTROL Logs de auditoria] página em [!UICONTROL Configuração]](assets/admin-fund-audit-log-1.png)

Cada ação registrada ou registrada mostra:

* A data e a hora da alteração
* O tipo de log
* O nome do usuário que concluiu a ação
* O objeto
* Quaisquer detalhes associados à ação
* O endereço IP

![[!UICONTROL Log de auditoria] lista](assets/admin-fund-audit-log-2.JPG)

## Exportar o log de auditoria

A exportação dos dados do log de auditoria permite que os administradores do sistema compartilhem as informações com auditores internos/externos ou especialistas em segurança. Algumas organizações exigem que determinados registros sejam retidos para fins de conformidade com as regulamentações de segurança cibernética. Outros precisam das informações importadas em um sistema de segurança para análise.

Os logs de auditoria podem ser exportados em um arquivo CSV (valores separados por vírgula), que pode ser aberto em um aplicativo de planilha ou em um editor de texto simples. A exportação é limitada a 50.000 linhas de cada vez, portanto, use os filtros para restringir a lista se o total exceder 50.000.

![[!UICONTROL Exportar] botão ligado [!UICONTROL Logs de auditoria] página](assets/admin-fund-audit-log-3.png)

<!---
learn more URLs
Audit logs
Managing audit logs
--->
