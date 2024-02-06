---
title: Relatórios de provas
description: Saiba como usar as funções de relatório para gerenciar o progresso da prova.
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: report-on-proofs.png
jira: KT-10233
exl-id: 9a1a9e16-61cc-4f95-977a-8870b7fd0dda
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '445'
ht-degree: 100%

---

# Relatórios de provas

Os recursos de prova digital do [!DNL Workfront] permitem gerenciar projetos e fluxos de trabalho de prova relacionados sem sair do [!DNL Workfront]. Obtenha insights valiosos sobre o andamento do trabalho de revisão com tipos de relatórios, origens e nomes de campos que exibem informações de revisão e aprovação.

Recomendamos conversar com o(a) consultor(a) do [!DNL Workfront] para criar relatórios que atendam aos requisitos da sua organização. Alguns dos relatórios exigem conhecimento sobre o modo de relatórios de texto do [!DNL Workfront].

Comece com esses relatórios básicos para ajudar suas equipes a gerenciar provas em um processo de revisão e aprovação no [!DNL Workfront].

## [!UICONTROL Aprovação da revisão]

Este tipo de relatório ajuda você a monitorar aprovações pendentes para garantir que os prazos estejam sendo cumpridos.

![Selecione [!UICONTROL Aprovação de prova] no menu suspenso [!UICONTROL Novo relatório]](assets/proof-system-setups-proof-approval-report.png)

As opções de visualização e filtro incluem: [!UICONTROL data de decisão], [!UICONTROL aprovação de prova], [!UICONTROL estágio de aprovação], [!UICONTROL modelo de fluxo de trabalho] e [!UICONTROL informações do solicitante]. Com os relatórios do modo de texto, você pode criar um agrupamento para organizar a lista por nome de documento. Consulte [Entenda o modo de texto básico para agrupamentos](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/basic-text-mode-for-groupings.html?lang=pt-BR).

Ao gerar relatórios de aprovação, certifique-se de obter informações da versão mais recente das provas. O [!DNL Workfront] recomenda incluir esta fonte e nome de campo no filtro:

**[!UICONTROL Aprovação de prova]>>[!UICONTROL É a versão atual do documento]**

![Guia Filtros no Report Builder](assets/proof-system-setups-proof-approval-report-is-current-version.png)

Isso é útil quando você está gerando relatórios de provas que tenham várias versões, para que o relatório liste apenas a versão atual de cada prova que precisa de aprovação. Isso filtra as versões anteriores nas quais você não precisa mais trabalhar.

## [!UICONTROL Versão do Documento]

Esse tipo de relatório permite gerenciar e monitorar versões no [!DNL Workfront].

![Selecione [!UICONTROL Versão do documento] no menu suspenso [!UICONTROL Novo relatório]](assets/proof-system-setups-document-version-report.png)

As opções de visualização incluem as seguintes informações: [!UICONTROL versão do documento], [!UICONTROL documento], [!UICONTROL registrado por], [!UICONTROL status de aprovação da prova], [!UICONTROL criador da prova] e [!UICONTROL fornecedor do documento].

Os agrupamentos podem ser feitos por [!UICONTROL versão do documento], [!UICONTROL registrado por], [!UICONTROL status de aprovação da prova] ou informações do proprietário da prova.

Os filtros incluem: [!UICONTROL versão do documento], [!UICONTROL nível de acesso], [!UICONTROL documento], [!UICONTROL registrado por], [!UICONTROL status de aprovação da prova], [!UICONTROL criador da prova] e informações do fornecedor do documento.

Você pode exibir o nome do estágio atualmente ativo do processo de revisão em cada documento do relatório utilizando esta coluna em uma visualização:

**[!UICONTROL Versões do documento] >> [!UICONTROL Estágios de prova ativos]**

![Guia Filtros no Report Builder](assets/proof-system-setups-active-proof-stages.png)

Se não houver estágio ativo no momento, a coluna ficará em branco.

Esta combinação de origem de campo >> nome de campo também está disponível como um filtro no relatório.

Use a origem de campo [!UICONTROL Criador da prova] para relatar informações sobre o usuário que criou a prova. Escolha a origem de campo [!UICONTROL Nome] para exibir o nome do(a) criador(a) da prova em uma visualização.

**[!UICONTROL Criador da prova] >> [!UICONTROL Nome]**

Esta combinação de fonte de campo >> nome de campo também está disponível como um filtro.

![Guia Filtros no Report Builder](assets/proof-system-setups-proof-creator-name.png)

<!--
Learn More Icon
Learn how to create reports in [!DNL Workfront] with the Report Creation class.
Access to proofing functionality
-->
