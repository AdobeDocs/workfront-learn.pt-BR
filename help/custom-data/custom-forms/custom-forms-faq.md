---
title: Respostas a perguntas sobre formulários personalizados
description: Obtenha respostas para perguntas comuns sobre formulários personalizados.
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Beginner, Intermediate
activity: use
team: Technical Marketing
jira: KT-10058
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
    internal-label: Leader
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
source-git-commit: 54883ad8c8df3aaee06ba8f8dca64227594c1c77
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 88%
---
# Perguntas comuns sobre formulários personalizados

**Posso mudar o tipo de exibição de um campo depois de criá-lo? Por exemplo, posso alterar de um menu suspenso para caixas de seleção?**

Sim. O tipo de exibição pode ser alternado para outro tipo de exibição semelhante: texto para parágrafo, lista suspensa para caixas de seleção ou botões de opção etc. Para obter mais informações sobre como alterar o tipo de exibição, consulte o artigo Criar um formulário personalizado.


**Posso usar o mesmo formulário personalizado para vários objetos? Por exemplo, um formulário que criei para uma tarefa de um projeto?**

Não. Os formulários personalizados têm um relacionamento individual com um objeto. No entanto, você pode copiar o formulário personalizado e alterar o objeto para o que for necessário.


**Um formulário personalizado pode ser anexado a um modelo de projeto?**

Sim. Dessa forma, qualquer projeto criado a partir desse modelo já terá o formulário personalizado anexado a ele.


**Há um limite para o número de campos que posso ter em um formulário personalizado?**

Você pode adicionar até 500 campos em um único formulário personalizado. No entanto, utilizar mais de 100 campos em um formulário pode reduzir o seu desempenho, dependendo da complexidade do formulário personalizado. Exemplos de formulários complexos incluem os que utilizam parâmetros em cascata, campos de dados calculados personalizados e várias opções de valor em um determinado campo.


**Há um limite para o número de formulários personalizados que posso anexar a um projeto?**

Sim. Você pode anexar até 10 formulários personalizados a um objeto. Para obter mais informações, consulte este artigo: Aplicar formulários personalizados a objetos.


**Posso desativar um formulário personalizado?**

Sim. Na guia de configurações do formulário personalizado, desmarque a caixa Está ativo. Isso remove o formulário personalizado de qualquer menu suspenso no Workfront. No entanto, se o formulário personalizado já estiver anexado a um projeto, ele permanecerá nesse projeto e preservará os dados já inseridos.