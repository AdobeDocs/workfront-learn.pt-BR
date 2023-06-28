---
title: Criar uma expressão de dados SUB, SUM, DIV ou PROD
description: Saiba como usar e criar as expressões matemáticas básicas em um campo calculado em Adobe [!DNL Workfront].
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335177.png
jira: KT-8914
exl-id: e767b73b-1591-4d96-bb59-2f2521e3efa3
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 0%

---

# Criar uma expressão de dados SUB, SUM, DIV ou PROD

Neste vídeo, você aprenderá:

* O que as expressões SUB, SUM, DIV e PROD fazem
* Como criar uma expressão de dados SUB em um campo calculado

>[!VIDEO](https://video.tv.adobe.com/v/335177/?quality=12&learn=on)

## Informações adicionais: expressão ROUND

### Criar uma expressão ROUND

A expressão ROUND pega qualquer número e o arredonda para um determinado número de casas decimais.

Na maioria das vezes, a expressão de dados ROUND é usada juntamente com outra expressão de dados e quando o campo de formato é deixado como Texto ou Número.

Vamos criar um campo calculado para determinar a diferença entre o número de horas planejadas e realmente conectadas em uma tarefa, que exigirá a expressão SUB e terá esta aparência:

**SUB({workRequired},{actualWorkRequired})**

E como o tempo é rastreado em minutos e o formato preferido é mostrar as informações em horas, a expressão também precisa ser dividida por 60 e ter esta aparência:

**DIV( SUB({workRequired},{actualWorkRequired}),60)**

Se o formato for alterado para Number ao criar o campo calculado no formulário personalizado, será possível alterar o formato do número ao adicionar o campo em uma exibição.

![Relatório do balanceador de carga de trabalho com utilização](assets/round01.png)

No entanto, se o formato do campo ao criar um campo personalizado for deixado como Texto, o formato não poderá ser facilmente alterado na exibição. A expressão ROUND deve ser usada para evitar que números como este sejam vistos em seu projeto:

![Relatório do balanceador de carga de trabalho com utilização](assets/round02.png)

<b>Usar a expressão de dados ROUND em um campo calculado</b>

A expressão ROUND inclui o nome da expressão (ROUND) e, normalmente, dois pontos de dados. Esses pontos de dados podem ser uma expressão ou um campo no Workfront, seguido por um número para indicar quantas casas decimais você gostaria de ir.

Uma expressão seria estruturada assim: ROUND(ponto de dados, #)

Na expressão que calcula a diferença entre as horas planejadas e reais, use esta expressão —DIV(SUB({workRequired},{actualWorkRequired}),60) — como o primeiro ponto de dados. Em seguida, verifique se qualquer número proveniente dessa expressão não ultrapassa 2 casas decimais à direita.

![Relatório do balanceador de carga de trabalho com utilização](assets/round03.png)

A expressão pode ser escrita assim: ROUND(DIV(SUB({workRequired},{actualWorkRequired}),60),2).
