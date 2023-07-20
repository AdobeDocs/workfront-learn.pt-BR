---
title: Use as expressões ISBLANK e CONTAINS
description: Saiba como usar e criar as expressões ISBLANK e CONTAINS em um campo calculado em Adobe [!DNL Workfront].
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: isblank-contains.png
exl-id: 819ffec8-e7e6-4a3c-a589-1348aa09e27d
source-git-commit: 409147f9a62302d28e14b834981992a0421d4e4b
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# Use as expressões ISBLANK e CONTAINS

As expressões CONTAINS e ISBLANK são usadas para fornecer valores simples de verdadeiro ou falso. A diferença é que a expressão ISBLANK verifica se o campo contém um valor, enquanto a expressão de texto CONTAINS procura uma string específica dentro de um campo.

Por exemplo, para ver se um projeto tem uma descrição, use a expressão ISBLANK. Se o campo de descrição estiver em branco, a expressão retornará um valor true. Se o campo de descrição não estiver em branco, retornará um valor false.

![Relatório do balanceador de carga de trabalho com utilização](assets/isblank01.png)

Para procurar um valor específico na descrição, como &quot;evento de caridade&quot;, use a expressão de texto CONTAINS. Se encontrar &quot;evento de caridade&quot; na descrição, o campo calculado dirá &quot;true&quot;. Ele exibe &quot;false&quot; se não encontrar &quot;evento de caridade&quot;.

![Relatório do balanceador de carga de trabalho com utilização](assets/isblank02.png)

## ISBLANK

A expressão de texto ISBLANK inclui o nome da expressão e um ponto de dados.

**ISBLANK({data point})**

![Relatório do balanceador de carga de trabalho com utilização](assets/isblank03.png)

No exemplo acima, no qual você deseja saber se o projeto tem uma descrição, a expressão seria:

ISBLANK({description})

## CONTÉM

A expressão de texto CONTAINS inclui o nome da expressão, a palavra ou frase que você está procurando e o campo a ser procurado.

**CONTAINS(&quot;phrase&quot;,{fields})**

Certifique-se de colocar aspas na palavra ou frase que você está procurando, caso contrário a expressão não será válida.

No exemplo acima (procurar &quot;evento beneficente&quot; na descrição do projeto), a expressão seria:

**CONTAINS(&quot;evento beneficente&quot;,{description})**

![Relatório do balanceador de carga de trabalho com utilização](assets/isblank04.png)

**Nota**: a expressão CONTAINS diferencia maiúsculas de minúsculas. Por exemplo, se &quot;Evento de caridade&quot; estiver em maiúsculas no campo de descrição, coloque essa frase em maiúsculas na expressão.

**CONTAINS(&quot;Evento de caridade&quot;,{description})**

As expressões ISBLANK e CONTAINS são boas de usar se você estiver procurando ver se um valor está presente. No entanto, pode ser mais útil saber qual é o valor, para realmente vê-lo ou ter algum tipo de descritor para fornecer um melhor insight.

Por exemplo, em vez de apenas saber que um projeto foi convertido de uma solicitação, você deseja saber o nome da solicitação original.

Nesse caso, use a expressão CONTAINS juntamente com uma expressão IF.

Na maioria das vezes, as expressões de texto ISBLANK e CONTAINS são usadas com uma expressão de texto IF.
