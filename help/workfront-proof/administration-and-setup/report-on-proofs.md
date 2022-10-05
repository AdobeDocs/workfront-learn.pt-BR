---
title: Relatório sobre provas
description: Saiba como usar os recursos de relatório do para gerenciar o progresso da prova.
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: report-on-proofs.png
kt: 10233
exl-id: 9a1a9e16-61cc-4f95-977a-8870b7fd0dda
source-git-commit: a0aa8328842d2db1235edc42664eb0b18f4038e4
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# Relatório sobre provas

[!DNL Workfront]Os recursos de revisão digital da permitem que você gerencie projetos e fluxos de trabalho de revisão relacionados em um único local — [!DNL Workfront]. Obtenha informações valiosas sobre o trabalho de revisão de provas que está sendo feito com tipos de relatório, fontes de campo e nomes de campo que exibem informações de revisão e aprovação.

Recomendamos trabalhar com a [!DNL Workfront] consultor da para criar relatórios que atendam às necessidades de sua organização. Alguns relatórios exigem familiaridade com [!DNL Workfront]relatório do modo de texto do .

Comece com esses relatórios básicos e padrão para ajudar suas equipes a gerenciar provas durante um processo de revisão e aprovação em [!DNL Workfront].

## [!UICONTROL Aprovação da revisão]

Esse tipo de relatório ajuda você a rastrear aprovações de prova pendentes para garantir que os prazos sejam cumpridos.

![Selecionar [!UICONTROL Aprovação de prova] do [!UICONTROL Novo relatório] menu suspenso](assets/proof-system-setups-proof-approval-report.png)

As opções de visualização e filtro incluem [!UICONTROL data de decisão], [!UICONTROL aprovação de prova], [!UICONTROL estágio do aprovador], [!UICONTROL modelo de fluxo de trabalho]e [!UICONTROL informações do solicitante]. Com o relatório do modo de texto, é possível criar um agrupamento que organiza a lista por nome de documento.

Ao gravar relatórios de aprovação de prova, verifique se você está obtendo informações relacionadas à versão mais recente das provas. [!DNL Workfront] A recomenda incluir essa fonte de campo e o nome do campo no filtro:

**[!UICONTROL Aprovação de prova]>>[!UICONTROL É Versão do Documento Atual]**

![Guia Filtros no construtor de relatórios](assets/proof-system-setups-proof-approval-report-is-current-version.png)

Isso é útil quando você está relatando provas que têm várias versões, de modo que o relatório lista somente a versão atual de cada prova que precisa de aprovação. Isso filtra as versões anteriores nas quais você não precisa mais trabalhar.

## [!UICONTROL Versão do Documento]

Esse tipo de relatório permite gerenciar e rastrear versões no [!DNL Workfront].

![Selecionar [!UICONTROL Versão do documento] do [!UICONTROL Novo relatório] menu suspenso](assets/proof-system-setups-document-version-report.png)

As opções de exibição incluem informações do [!UICONTROL versão do documento], [!UICONTROL documento], [!UICONTROL digitado por], [!UICONTROL status de aprovação de prova], [!UICONTROL criador de prova]e [!UICONTROL provedor de documento].

Os agrupamentos podem ser feitos por [!UICONTROL versão do documento], [!UICONTROL digitado por], [!UICONTROL status de aprovação de prova]ou informações do proprietário da prova.

Os filtros incluem [!UICONTROL versão do documento], [!UICONTROL nível de acesso], [!UICONTROL documento], [!UICONTROL digitado por], [!UICONTROL status de aprovação de prova], [!UICONTROL criador de prova]e informações do provedor de documentos.

Você pode exibir o nome da etapa de prova que está ativa atualmente para cada documento no relatório com esta coluna em uma exibição:

**[!UICONTROL Versões do documento] >> [!UICONTROL Estágios de prova ativos]**

![Guia Filtros no construtor de relatórios](assets/proof-system-setups-active-proof-stages.png)

Se nenhum estágio estiver ativo no momento, a coluna ficará em branco.

Esse campo source >> nome do campo também está disponível como filtro em um relatório.

Use o [!UICONTROL Criador de prova] fonte do campo para relatar informações sobre o usuário que criou a prova. Escolha a [!UICONTROL Nome] fonte do campo para exibir o nome do criador de prova em uma visualização.

**[!UICONTROL Criador de prova] >> [!UICONTROL Nome]**

Essa combinação de nome de campo > fonte> também está disponível como filtro.

![Guia Filtros no construtor de relatórios](assets/proof-system-setups-proof-creator-name.png)

<!--
Learn More Icon
Learn how to create reports in [!DNL Workfront] with the Report Creation class.
Access to proofing functionality
-->
