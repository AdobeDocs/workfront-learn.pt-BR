---
title: Introdução a campos calculados e expressões
description: Saiba como criar expressões em campos calculados para coletar dados personalizados e exclusivos sobre o trabalho que está sendo feito para sua organização.
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
source-wordcount: '503'
ht-degree: 100%

---

# Introdução a campos calculados e expressões

<!-- **Note**: The expression examples shown are simple and some may be mitigated by fields already supplied by  . However, the examples are used to illustrate the foundational knowledge needed in order to build expressions in Workfront.-->

O Workfront oferece uma variedade de campos que são comuns em diversas áreas de negócios e usados regularmente para o gerenciamento de tarefas. Campos como a data de conclusão planejada, orçamento do projeto, nome do(a) responsável pela tarefa etc.

No entanto, cada organização tem dados específicos do seu setor que precisam ser coletados para descobrir se os objetivos da empresa estão sendo alcançados. Por exemplo, sua organização deseja acompanhar:

* Para qual setor um projeto contribuirá.
* Se o financiamento vem de fornecedores, é interno ou ambos.
* Qual resolução é necessária para as imagens utilizadas.

Embora esses campos não estejam diretamente integrados ao [!DNL Workfront], você pode criar campos de entrada com dados personalizados e campos de múltiplas respostas pré-preenchidos por meio de um formulário personalizado.

Esse tutorial de aprendizagem concentra-se nos campos calculados. Você aprenderá o que é um campo calculado, os diferentes tipos de informações que podem ser inseridos nele por meio de expressões de dados e como criar campos calculados para aprimorar sua coleta de dados e relatórios.

![Documento de visão geral da configuração do gerenciamento de recursos](assets/GS01.png)

## O que é um campo calculado?

Um campo calculado armazena dados personalizados criados por meio de expressões de dados e campos existentes do Workfront.

![Balanceador de carga de trabalho com relatório de utilização](assets/GS02.png)

Por exemplo, sua organização tem um sistema de numeração de projetos ou tarefas específico, que inclui:

* O ano de criação do projeto,
* As iniciais do proprietário do projeto e
* O número de referência do projeto no [!DNL Workfront].


Utilizando expressões em um campo calculado, você pode coletar as informações já armazenadas no [!DNL Workfront] e criar uma ID de projeto exclusiva (ou número de tarefa), a qual pode ser adicionada a um relatório como este:

![Balanceador de carga de trabalho com relatório de utilização](assets/GS03.png)

Dependendo dos dados necessários, os campos calculados podem ser simples, utilizando uma ou duas expressões, ou mais complicados, utilizando várias expressões incorporadas. Lembre-se de que o Workfront só pode usar os dados já armazenados ou inseridos no sistema para os campos calculados.

## Expressões de texto

As expressões de texto pesquisam, analisam e combinam informações encontradas no [!DNL Workfront] para criar dados mais significativos ou obter maiores insights sobre o trabalho que está sendo realizado em sua organização.

Por exemplo, as expressões de texto podem ser usadas para:

* Mostrar a mensagem “Acima de US$ 5.000” em uma coluna de visualização do projeto quando as despesas do projeto forem superiores a US$ 5.000 ou “Abaixo de US$ 5.000” quando estiverem abaixo disso.

* Atribuir a cada projeto um número exclusivo que inclua o ano em que o projeto foi criado, o número de referência no [!DNL Workfront], o nome do projeto e as iniciais do proprietário.

* Criar um relatório que liste todos os projetos que não estão atribuídos a um portfólio e/ou programa para usar em reuniões gerenciais.

As expressões de texto podem ser usadas em um campo personalizado para fazer esses tipos de pesquisas e combinações no Workfront.

Ao observar as possíveis expressões de texto, você encontrará várias opções.

![Documento de visão geral da configuração do gerenciamento de recursos](assets/TE01.png)

Estas são as seis expressões de texto usadas com mais frequência:

* CONCAT
* ESQUERDA / DIREITA
* CONTÉM
* SE
* ISBLANK