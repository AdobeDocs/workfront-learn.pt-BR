---
title: Introdução a campos calculados e expressões
description: Saiba como criar expressões em campos calculados para coletar dados personalizados exclusivos sobre o trabalho que está sendo feito para sua organização.
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: gs-calc-fields-expressions.png
exl-id: fbd17f01-9e97-4ead-9a56-7ce4f81255ec
source-git-commit: 409147f9a62302d28e14b834981992a0421d4e4b
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---

# Introdução a campos calculados e expressões

<!-- **Note**: The expression examples shown are simple and some may be mitigated by fields already supplied by  . However, the examples are used to illustrate the foundational knowledge needed in order to build expressions in Workfront.-->

O Workfront fornece uma variedade de campos que são comuns em várias áreas de negócios e são usados regularmente para gerenciamento de trabalho. Campos como data de conclusão planejada, orçamento do projeto, nome do destinatário da tarefa etc.

No entanto, cada organização tem dados específicos para seu setor e empresa que precisam ser coletados para entender se os objetivos da empresa estão sendo atendidos. Por exemplo, sua organização deseja acompanhar:

* Para qual linha de negócios um projeto contribuirá.
* Se o financiamento vem de fornecedores, internos ou ambos.
* Qual resolução é necessária para imagens usadas?

Embora esses campos não sejam inerentemente [!DNL Workfront], você pode criar campos de entrada de dados personalizados e campos de resposta pré-preenchidos e de seleção múltipla por meio de um formulário personalizado.

Este caminho de aprendizagem se concentra no campo calculado. Você aprenderá o que é um campo calculado, os diferentes tipos de informações que você pode obter no campo calculado por meio de expressões de dados e como criar esses campos calculados para aprimorar a coleta de dados e os relatórios.

![O gerenciamento de recursos configura um pager](assets/GS01.png)

## O que é um campo calculado?

Um campo calculado armazena dados personalizados criados usando expressões de dados e campos existentes do Workfront.

![Relatório do balanceador de carga de trabalho com utilização](assets/GS02.png)

Por exemplo, sua organização tem um sistema de numeração de projeto ou número de trabalho específico que inclui:

* Ano de criação do projeto,
* As iniciais do proprietário do projeto e
* A variável [!DNL Workfront] número de referência do projeto.


Usando expressões em um campo calculado, você pode pegar cada parte das informações já armazenadas no [!DNL Workfront] e criar essa ID de projeto exclusiva, ou número de trabalho, que pode ser adicionado a um relatório como este:

![Relatório do balanceador de carga de trabalho com utilização](assets/GS03.png)

Dependendo dos dados específicos necessários, os campos calculados podem ser simples, usando uma ou duas expressões, ou mais complicados, usando várias expressões incorporadas. Lembre-se de que o Workfront só pode usar os dados já armazenados ou extraídos do sistema para campos calculados.

## Expressões de texto

As expressões de texto pesquisam, dissecam e combinam informações encontradas em [!DNL Workfront] para criar dados mais significativos ou obter mais informações sobre o trabalho que está sendo feito para a sua organização.

Por exemplo, expressões de texto podem ser usadas para:

* Mostrar &quot;Acima de US$ 5.000&quot; quando as despesas do projeto forem superiores a US$ 5.000, ou &quot;Abaixo de US$ 5.000&quot; quando as despesas estiverem abaixo disso, em uma coluna de uma exibição de projeto.

* Atribua a cada projeto um número exclusivo que inclua o ano em que o projeto foi criado, a  [!DNL Workfront] número de referência, o nome e as iniciais do proprietário do projeto.

* Crie um relatório que liste todos os projetos que não estão atribuídos a um portfólio e/ou programa para que você possa usá-lo em suas reuniões de gerente.

Expressões de texto podem ser usadas em um campo personalizado para fazer esses tipos de pesquisas e combinações no Workfront.

Ao observar as possíveis expressões de texto, você encontrará várias opções.

![O gerenciamento de recursos configura um pager](assets/TE01.png)

Há seis expressões de texto usadas com mais frequência:

* CONCAT
* ESQUERDA / DIREITA
* CONTÉM
* SE
* ISBLANK