---
title: Use as expressões ISBLANK e CONTAINS
description: Saiba como usar e criar as expressões ISBLANK e CONTAINS em um campo calculado no Adobe [!DNL Workfront].
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: isblank-contains.png
exl-id: 819ffec8-e7e6-4a3c-a589-1348aa09e27d
source-git-commit: 2b9a31b45ff94222a77c05292ee5b9d8229f5f0b
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# Use as expressões ISBLANK e CONTAINS

As expressões CONTAINS e ISBLANK são usadas para fornecer valores simples verdadeiros ou falsos. A diferença é que a expressão ISBLANK verifica se o campo tem um valor enquanto a expressão de texto CONTÉM procura uma string específica em um campo.

Por exemplo, para ver se um projeto tem uma descrição, use a expressão ISBLANK. Se o campo de descrição estiver em branco, a expressão retornará um valor true. Se o campo de descrição não estiver em branco, retornará um valor false.

![Balanceador de carga de trabalho com relatório de utilização](assets/isblank01.png)

Para procurar um valor específico na descrição, como &quot;evento de caridade&quot;, use a expressão de texto CONTÉM . Se encontrar &quot;evento de caridade&quot; na descrição, o campo calculado exibirá &quot;true&quot;. Ele exibe &quot;false&quot; se não encontrar &quot;evento de caridade&quot;.

![Balanceador de carga de trabalho com relatório de utilização](assets/isblank02.png)

## ISBLANK

A expressão de texto ISBLANK inclui o nome da expressão e um ponto de dados.

**ISBLANK(ponto de dados)**

![Balanceador de carga de trabalho com relatório de utilização](assets/isblank03.png)

No exemplo acima, onde você quer saber se o projeto tem uma descrição, a expressão seria:

ISBLANK(Descrição)

## CONTÉM

A expressão de texto CONTÉM inclui o nome da expressão, a palavra ou frase que você está procurando e o campo a ser procurado.

**CONTAINS(&quot;phrase&quot;,field)**

Assegure-se de colocar aspas na palavra ou frase que está procurando, caso contrário, a expressão não será válida.

No exemplo acima (procurando por &quot;evento de caridade&quot; na descrição do projeto), a expressão seria:

**CONTAINS(&quot;evento de caridade&quot;,Descrição)**

![Balanceador de carga de trabalho com relatório de utilização](assets/isblank04.png)

**Observação**: A expressão CONTAINS diferencia maiúsculas de minúsculas. Por exemplo, se &quot;Evento de caridade&quot; estiver capitalizado no campo de descrição, coloque essa frase em maiúsculas e minúsculas na expressão.

**CONTAINS(&quot;Evento de caridade&quot;,Descrição)**

As expressões ISBLANK e CONTAINS são boas de usar se você deseja ver se há um valor presente. No entanto, pode ser mais útil saber qual é o valor, para realmente visualizá-lo ou ter algum tipo de descritor para fornecer melhor insight.

Por exemplo, em vez de apenas saber que um projeto foi convertido de uma solicitação, você deseja saber o nome da solicitação original.

Nesse caso, use a expressão CONTAINS juntamente com uma expressão IF.

Na maioria das vezes, as expressões de texto ISBLANK e CONTAINS são usadas com uma expressão de texto IF.
