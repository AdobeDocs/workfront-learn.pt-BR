---
title: Entenda o log de auditoria do sistema
description: Saiba como usar o log de auditoria do sistema para descobrir quando e por quem os itens foram alterados.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner, Intermediate
thumbnail: 10040.jpeg
jira: KT-10040
exl-id: 9de6fd40-10fb-47a6-b186-3a38c411f1ac
TQID: https://experienceleague.adobe.com/xMxWQ53TUXVjS-H8EuK3nf7jt8v4vUgKoZVsmApc-JM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 267
ht-degree: 100%

---

# Entenda o log de auditoria do sistema

O log de auditoria do sistema é a melhor maneira para admins de sistema acompanharem o que está acontecendo no [!DNL Workfront]. Pense no log como uma fonte confiável para saber quem fez quais alterações e quando.

Acesse o log de auditoria na seção [!UICONTROL Preferências] da área [!UICONTROL Configuração]. Por padrão, você verá os dados dos últimos sete dias. Altere os critérios de filtro para ver os dados de diferentes intervalos de datas.

Quando um usuário executa determinadas ações, o [!UICONTROL Workfront] as registra na seção [!UICONTROL Logs de auditoria] da área [!UICONTROL Configuração].

Menu suspenso ![[!UICONTROL Tipo de log] na página [!UICONTROL Logs de auditoria] da seção [!UICONTROL Configuração]](assets/admin-fund-audit-log-1.png)

Cada ação registrada mostra:

* A data e a hora da alteração
* O tipo de log
* O nome do usuário que concluiu a ação
* O objeto
* Quaisquer detalhes associados à ação
* O endereço IP

A lista ![[!UICONTROL Log de auditoria]](assets/admin-fund-audit-log-2.JPG)

## Exportar o log de auditoria

A exportação dos dados do log de auditoria permite que admins de sistema compartilhem as informações com auditores internos/externos ou especialistas em segurança. Algumas organizações exigem que determinados registros sejam retidos para fins de conformidade com os regulamentos de segurança cibernética. Outras precisam que as informações sejam importadas para um sistema de segurança para fins de análise.

Os logs de auditoria podem ser exportados como um arquivo CSV (valores separados por vírgula), que pode ser aberto em um aplicativo de planilhas ou editor de texto simples. A exportação é limitada a 50 mil linhas por vez; portanto, se o total exceder 50 mil, use os filtros para restringir a lista.

Botão ![[!UICONTROL Exportar] na página [!UICONTROL Logs de auditoria]](assets/admin-fund-audit-log-3.png)

<!--
learn more URLs
Audit logs
Managing audit logs
-->
