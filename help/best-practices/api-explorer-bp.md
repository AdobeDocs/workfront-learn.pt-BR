---
title: 'Prática recomendada: API Explorer'
description: Conheça as práticas recomendadas de especialistas do Adobe Workfront sobre configurar, gerenciar e usar o API Explorer do Workfront.
feature: Workfront API
role: Admin, Leader, User
level: Beginner
jira: KT-10902
exl-id: 0f3fc5ba-d01a-4337-829f-def0830ddf81
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 100%

---

# Prática recomendada: API Explorer

## O que é uma “prática recomendada” do Adobe Workfront?

As práticas recomendadas são diretrizes para um curso de ação eficaz e eficiente; elas podem ser facilmente adotadas por qualquer usuário da empresa e replicadas com sucesso em toda a organização.

Ao revisar essas recomendações, lembre-se de que algumas práticas recomendadas do Workfront são universais, enquanto outras podem ser mais específicas para um determinado assunto. Use essas práticas recomendadas como uma base para orientar as configurações e o uso do sistema do Workfront.

## Navegar nesta página

Ao percorrer esta página, você encontrará primeiro uma lista resumida de todas as práticas recomendadas para o tópico. Isso permite revisar as recomendações sem se aprofundar nos detalhes e motivos por trás delas.

A seção “Por que essas práticas são recomendadas?” , encontrada após a lista resumida, fornece mais detalhes sobre algumas práticas recomendadas e por que elas são consideradas como um processo, ferramenta ou recurso que você deve considerar implementar na sua instância do Workfront.

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

Um projeto é o lugar perfeito para registrar nomes de campos personalizados, com que integração eles são usados etc. Isso ajuda a evitar a criação de campos personalizados redundantes ou o uso do mesmo campo personalizado com múltiplas integrações.

</br>
</br>


**Prática recomendada**

Adicione o campo de ID do objeto aos relatórios usados pelo(a) admin de sistema.

**Entenda o porquê**

Admins de sistema geralmente reconhecem objetos no Workfront por seus números de ID ao usar APIs ou outras integrações. Inclua o campo de ID nas visualizações dos objetos nos quais está trabalhando (projetos, tarefas, problemas, modelos, formulários personalizados etc.) para facilitar o acesso e a cópia.
