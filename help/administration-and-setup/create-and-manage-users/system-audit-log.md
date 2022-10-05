---
title: Compreender o log de auditoria do sistema
description: Saiba como usar o log de auditoria do sistema para analisar quando as alterações foram feitas e quando os itens foram alterados.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner, Intermediate
thumbnail: 10040.jpeg
kt: 10040
exl-id: 9de6fd40-10fb-47a6-b186-3a38c411f1ac
source-git-commit: adf12d7846d2a1b4c32513a3955c080905044576
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---

# Entender o log de auditoria do sistema

O registro de auditoria do sistema é a melhor maneira de o administrador do sistema ficar de olho no que está acontecendo [!DNL Workfront]. Pense no log como sua fonte de verdade para quem fez o que mudou e quando.

Acesse o log de auditoria ao acessar a [!UICONTROL Preferências] na seção [!UICONTROL Configuração] área. Por padrão, você vê dados dos últimos sete dias. Altere os critérios de filtro para ver dados de intervalos de datas diferentes.

Quando um usuário executa determinadas ações, [!UICONTROL Workfront] registrá-los no [!UICONTROL Logs de auditoria] da seção [!UICONTROL Configuração] área.

![[!UICONTROL Tipo de log] no menu suspenso da [!UICONTROL Logs de auditoria] em [!UICONTROL Configuração]](assets/admin-fund-audit-log-1.png)

Cada ação registrada ou registrada mostra:

* A data e a hora da alteração
* O tipo de log
* O nome do usuário que concluiu a ação
* O objeto
* Quaisquer detalhes associados à ação
* O endereço IP

![[!UICONTROL Log de auditoria] lista](assets/admin-fund-audit-log-2.JPG)

## Exportar o log de auditoria

A exportação dos dados do log de auditoria permite que os administradores do sistema compartilhem as informações com auditores internos/externos ou especialistas em segurança. Algumas organizações exigem que determinados registros sejam retidos para fins de conformidade com as regulamentações de segurança cibernética. Outros precisam das informações importadas para um sistema de segurança para análise.

Os logs de auditoria podem ser exportados em um arquivo CSV (valor separado por vírgulas), que pode ser aberto em um aplicativo de planilha ou editor de texto simples. A exportação é limitada a 50.000 linhas de uma vez, portanto, use os filtros para restringir a lista se o total exceder 50.000.

![[!UICONTROL Exportar] botão ligado [!UICONTROL Logs de auditoria] página](assets/admin-fund-audit-log-3.png)

<!---
learn more URLs
Audit logs
Managing audit logs
--->
