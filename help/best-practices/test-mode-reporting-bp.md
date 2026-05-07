---
title: Prática recomendada - Relatórios no modo de texto
description: Conheça as práticas recomendadas por especialistas do Adobe Workfront sobre a configuração, gerenciamento e uso de relatórios no modo de texto do Workfront.
feature: Reports and Dashboards
role: Admin, Leader, User
level: Beginner
jira: KT-10928
exl-id: c624545c-ba42-4cc3-aafe-8be15baadb75
TQID: https://experienceleague.adobe.com/k8DYutzVcGrJc7p0x74B2iQ3nkiohWeQu1egOWZ34AI
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: f8a45b24-4be7-4f1b-909b-60d06b483a20
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 418
ht-degree: 90%

---

# Prática recomendada - Relatórios no modo de texto

## O que é uma “prática recomendada” do Adobe Workfront?

As práticas recomendadas são diretrizes para um curso de ação eficaz e eficiente; elas podem ser facilmente adotadas por qualquer usuário da empresa e replicadas com sucesso em toda a organização.

Ao revisar essas recomendações, lembre-se de que algumas práticas recomendadas do Workfront são universais, enquanto outras podem ser mais específicas para um determinado assunto. Use essas práticas recomendadas como uma base para orientar as configurações e o uso do sistema do Workfront.

## Navegar nesta página

Ao percorrer esta página, você encontrará primeiro uma lista resumida de todas as práticas recomendadas para o tópico. Isso permite revisar as recomendações sem se aprofundar nos detalhes e motivos por trás delas.

A área &quot;Por que essas práticas recomendadas?&quot;, encontrada após a lista de alto nível, fornece mais detalhes sobre algumas das práticas recomendadas e por que elas são consideradas um processo, ferramenta etc., você deve considerar a implementação com sua instância do Workfront.

</br>
</br>

## Práticas recomendadas para relatórios no modo de texto

* Use expressões de valor no modo de texto em vez de campos personalizados calculados sempre que possível, utilizando as colunas de listas de relatórios.

* Insira os cálculos usados no modo de texto na descrição do relatório.

</br>
</br>

## Por que essas práticas são recomendadas?

**Prática recomendada**

Use expressões de valor no modo de texto em vez de campos personalizados calculados sempre que possível, utilizando as colunas de listas de relatórios.



**Entenda o porquê**

As expressões de valor no modo de texto são calculadas assim que o relatório é executado e recalculadas sempre que o relatório é atualizado. Isso significa que você sempre terá dados atualizados e relatórios exatos.



Os campos calculados personalizados (usados em formulários personalizados) não são atualizados automaticamente ao exibir os dados no Workfront. Em vez disso, eles exibem os resultados do cálculo mais recente armazenado no Workfront. Isso significa que esses valores podem sempre estar “obsoletos” ou desatualizados. Os campos calculados personalizados devem ser atualizados manualmente, recalculando a expressão ou editando e salvando o objeto que contém o campo calculado. Esse pode ser um processo demorado, que também pode ser facilmente esquecido.


</br>
</br>

**Prática recomendada**

Insira os cálculos usados no modo de texto na descrição do relatório.



**Entenda o porquê**

Incluir cálculos do modo de texto na descrição do relatório ajuda outras pessoas a entender como o cálculo foi criado e que tipo de informação ele deve exibir. Isso também ajuda admins de sistema a lembrar como o relatório foi criado, caso atualizações sejam necessárias no futuro.
