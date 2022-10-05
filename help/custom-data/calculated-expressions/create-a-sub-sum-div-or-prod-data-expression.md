---
title: Criar uma expressão de dados SUB, SUM, DIV ou PROD
description: Saiba como usar e criar as expressões matemáticas básicas em um campo calculado no Adobe [!DNL Workfront].
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335177.png
kt: 8914
exl-id: e767b73b-1591-4d96-bb59-2f2521e3efa3
source-git-commit: 2b9a31b45ff94222a77c05292ee5b9d8229f5f0b
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 0%

---

# Criar uma expressão de dados SUB, SUM, DIV ou PROD

Neste vídeo, você aprenderá:

* O que as expressões SUB, SUM, DIV e PROD fazem
* Como criar uma expressão de dados SUB em um campo calculado

>[!VIDEO](https://video.tv.adobe.com/v/335177/?quality=12)

## Informações adicionais: expressão ROUND

### Criar uma expressão ROUND

A expressão ROUND pega qualquer número e arredonda-o para um determinado número de casas decimais.

Na maioria das vezes, a expressão de dados ROUND é usada juntamente com outra expressão de dados e quando o campo de formato é deixado como Texto ou Número.

Vamos criar um campo calculado para determinar a diferença entre o número de horas planejadas e realmente conectadas a uma tarefa, o que exigirá a expressão SUB e terá a seguinte aparência:

**SUB(Horas Planejadas, Horas Reais)**

E como o tempo é rastreado em minutos e o formato preferido é mostrar as informações em horas, a expressão também precisa ser dividida por 60 e ter esta aparência:

**DIV(SUB(Horas Planejadas, Horas Reais),60)**

Se o formato for alterado para Number ao criar o campo calculado no formulário personalizado, é possível alterar o formato do número ao adicionar o campo em uma visualização.

![Balanceador de carga de trabalho com relatório de utilização](assets/round01.png)

No entanto, se o formato do campo, ao criar um campo personalizado, for deixado como Texto, o formato não poderá ser facilmente alterado na exibição. A expressão ROUND deve ser usada para evitar ver números como este no seu projeto:

![Balanceador de carga de trabalho com relatório de utilização](assets/round02.png)

Use a expressão ROUND data em um campo calculado A expressão ROUND inclui o nome da expressão (ROUND) e, normalmente, dois pontos de dados. Esses pontos de dados podem ser uma expressão ou um campo em [!DNL Workfront], seguido por um número para indicar quantas casas decimais você gostaria de ir.

Uma expressão seria estruturada desta forma: ROUND(ponto de dados, #)

Na expressão que calcula a diferença entre horas planejadas e reais, use esta expressão — DIV(SUB(Horas Planejadas, Horas Reais),60) — como o primeiro ponto de dados. Em seguida, verifique se o número que vier dessa expressão não passa de 2 casas à direita do decimal.

![Balanceador de carga de trabalho com relatório de utilização](assets/round03.png)

A expressão poderia ser escrita desta forma: ROUND(DIV(SUB(Horas Planejadas, Horas Reais),60),2).
