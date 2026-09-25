---
title: 'Prática recomendada: API Explorer'
description: Conheça as práticas recomendadas de especialistas do Adobe Workfront sobre configurar, gerenciar e usar o API Explorer do Workfront.
feature: Workfront API
role: Admin, Leader, User
level: Beginner
jira: KT-10902
exl-id: 0f3fc5ba-d01a-4337-829f-def0830ddf81
TQID: 'https://experienceleague.adobe.com/RUQeNzEb0eg9DKSKepugb0HD4O2ODql-0mWBn-ptgxk'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
    internal-label: APIs
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
  - id: 682536a8-4872-5ee6-a8a6-8012d713482c
    internal-label: Workfront API
subfeature_v2:
  - id: bb1dd007-4a34-496d-9d3b-2278fdaadac1
    internal-label: API Explorer
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
    internal-label: Leader
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
source-git-commit: 54883ad8c8df3aaee06ba8f8dca64227594c1c77
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 75%
---
# Prática recomendada: API Explorer

## O que é uma “prática recomendada” do Adobe Workfront?

As práticas recomendadas são diretrizes para um curso de ação eficaz e eficiente; elas podem ser facilmente adotadas por qualquer usuário da empresa e replicadas com sucesso em toda a organização.

Ao revisar essas recomendações, lembre-se de que algumas práticas recomendadas do Workfront são universais, enquanto outras podem ser mais específicas para um determinado assunto. Use essas práticas recomendadas como uma base para orientar as configurações e o uso do sistema do Workfront.

## Navegar nesta página

Ao percorrer esta página, você encontrará primeiro uma lista resumida de todas as práticas recomendadas para o tópico. Isso permite revisar as recomendações sem se aprofundar nos detalhes e motivos por trás delas.

A área &quot;Por que essas práticas recomendadas?&quot;, encontrada após a lista de alto nível, fornece mais detalhes sobre algumas das práticas recomendadas e por que elas são consideradas um processo, ferramenta etc., você deve considerar a implementação com sua instância do Workfront.

</br>
</br>

## Práticas recomendadas para o API Explorer

* Estabeleça uma convenção de nomeação para os campos personalizados usados com integrações de sistemas de terceiros.

* Monitore todos os campos personalizados usados em integrações por meio de um projeto do Workfront.

* Adicione o campo de ID do objeto aos relatórios usados pelo(a) admin de sistema.

</br>
</br>

## Por que essas práticas são recomendadas?

**Prática recomendada**

Estabeleça uma convenção de nomeação para os campos personalizados usados com integrações de sistemas de terceiros.

**Entenda o porquê**

Certifique-se de que todos os criadores de formulários personalizados estejam a par da convenção de nomeação, para que não usem um campo reservado para uma integração acidentalmente. Dependendo das suas integrações e fluxos de trabalho, usar o mesmo campo de diversas maneiras pode resultar na modificação ou substituição de dados, bem como no registro de dados incorretos nos relatórios.

</br>
</br>


**Prática recomendada**

Monitore todos os campos personalizados usados em integrações por meio de um projeto do Workfront.

**Entenda o porquê**

Um projeto é o local perfeito para registrar nomes de campo personalizados, com que integração eles são usados, etc. Isso ajudará a evitar a criação de campos personalizados redundantes ou o uso do mesmo campo personalizado com várias integrações.

</br>
</br>


**Prática recomendada**

Adicione o campo de ID do objeto aos relatórios usados pelo(a) admin de sistema.

**Entenda o porquê**

Admins de sistema geralmente reconhecem objetos no Workfront por seus números de ID ao usar APIs ou outras integrações. Inclua o campo de ID nas exibições dos objetos em que você trabalha (projetos, tarefas, problemas, modelos, formulários personalizados etc.) para facilitar o acesso e a cópia.
