---
title: O que você deve saber sobre expressões de campo calculado
description: Dê uma olhada numa lista de conceitos úteis ao trabalhar com campos calculados personalizados em [!DNL Workfront].
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: to-know-expressions.png
exl-id: 512a3071-f47f-4fd4-bf5f-9b18bef8ba59
source-git-commit: 71f9ec5fad80664cc1d1f12c6772b131ee46c59c
workflow-type: tm+mt
source-wordcount: '959'
ht-degree: 0%

---

# O que você deve saber sobre expressões de campo calculado

Esta é uma lista de conceitos úteis ao trabalhar com campos calculados personalizados no Workfront.

## Geração de maiúsculas e minúsculas em nomes de expressão

Quando se trata de nomes de expressão, o uso de maiúsculas e minúsculas é importante. Ao escrever inicialmente um nome de expressão, você pode usar letras maiúsculas, minúsculas ou uma combinação de ambas.

![Mensagem de erro sem capitalização no nome da expressão](assets/T2K01.png)

No entanto, a expressão deve ser escrita como todas as letras maiúsculas para que o sistema reconheça a expressão e salve o campo.



## As horas são armazenadas em minutos

As horas no banco de dados do Workfront são armazenadas em minutos. Se você estiver fazendo referência a campos como Horas planejadas ou Horas efetivas, divida por 60 para mostrar o tempo em horas e não em minutos.

## O espaçamento não afeta expressões

A maneira recomendada de escrever expressões é com pouco ou nenhum espaçamento entre cada expressão.

* IF(ISBLANK({description}),&quot;Sem descrição&quot;,&quot;Tem descrição&quot;)

![Expressões sem espaçamento entre campos](assets/T2K02.png)

No entanto, se o espaçamento ajudar a ver o que está acontecendo, algum espaçamento poderá ser adicionado às expressões. Os espaços extras não devem impedir que a expressão colete ou calcule um valor em [!DNL Workfront].

* IF (ISBLANK ({description}), &quot;Sem descrição&quot; , &quot;Tem descrição&quot; )

![Expressões com espaçamento entre campos](assets/T2K03.png)

As únicas coisas que não podem ter espaços entre elas são os campos e as chaves. Caso contrário, você receberá uma mensagem de erro e não poderá salvar o campo ou o formulário personalizado.

![Erro com espaçamento entre o nome do campo e a chave](assets/T2K04.png)

## As aspas devem ser retas

Ao usar aspas em uma expressão, verifique se as aspas são retas (&quot;). Se as aspas forem curvas (&quot;), a variável [!DNL Workfront] O sistema continuará exibindo a mensagem &quot;Expressão personalizada inválida&quot;.

![Erro com aspas curvas](assets/T2K05.png)

## Atualização de cálculos ao salvar o formulário e editar o objeto

Esse é um aspecto importante dos campos calculados para compreender.

As informações exibidas em um campo calculado permanecerão as mesmas e se tornarão obsoletas, a menos que o formulário personalizado seja recalculado.

As expressões podem ser atualizadas usando a opção Recalcular Expressões no menu Mais em um objeto.

Você quer ver o número de dias que uma ocorrência ficou aberta. Crie um campo calculado chamado &quot;Dias em Aberto&quot; com a expressão DATEDIFF.

* Nome do Campo = Dias em Aberto
* Expressão = DATEDIFF({entryDate},$$TODAY)

Depois de salvo, o número de dias entre quando o problema foi criada ou inserida pela primeira vez no Workfront e a data de hoje podem ser mostrados na página de detalhes de um objeto ou em uma exibição de relatório.

Ao visualizar a mesma página de detalhes ou visualização de relatório no dia seguinte, você espera que esse número seja incrementado em um. Se o número for 5 hoje, deve ser 6 amanhã. O dia seguinte deve ser 7, depois 8 etc.

No entanto, o campo continuará exibindo 5 todos os dias. O campo deve ser &quot;executado novamente&quot; ou recalculado para atualizar as informações.

Para atualizar um campo usando a opção Recalcular Expressões:

* Clique no nome do objeto para abri-lo.
* Clique no menu Mais.
* Selecione Recalcular Expressões na lista.

![Opção Recalcular expressão no objeto](assets/T2K06.png)

Você também pode recalcular várias expressões ao mesmo tempo usando o recurso de &quot;edição em massa&quot; em uma lista ou relatório. Suponha que você tenha criado um relatório mostrando uma lista de problemas com o cálculo de Dias abertos que aparece em uma coluna. Se quiser recalcular todos os problemas de uma só vez:

* Selecione todos os problemas no relatório.
* Selecione a opção de edição para editar todas as ocorrências selecionadas em massa.
* Clique no rótulo Forms personalizado à esquerda para rolar para baixo até a seção de formulários personalizados.
* Marque a caixa Recalcular expressões personalizadas na parte inferior da seção Forms personalizada.
* Clique em Salvar alterações.

![Opção Recalcular expressão para vários objetos](assets/T2K07.png)

A tela é atualizada para mostrar as informações atualizadas no campo calculado.

**Nota**: Embora existam outras maneiras de atualizar ou recalcular expressões em um campo calculado, essa é a maneira mais rápida e fácil.

## Os cálculos podem variar de formulário para formulário no mesmo campo

Assim que um campo calculado for salvo em um formulário personalizado, e ele for salvo, o campo calculado será adicionado à Biblioteca de campos para que possa ser usado em outros formulários personalizados.

No entanto, se você tiver um campo calculado no formulário A e o mesmo campo calculado no formulário B, a ideia inicial é que os cálculos sejam exatamente os mesmos. Nem sempre é assim. O campo calculado no formulário A poderia estar calculando de uma maneira totalmente diferente no formulário B.

Quando um campo personalizado calculado é selecionado na biblioteca de campos e adicionado a um formulário personalizado, o campo é adicionado, mas o cálculo está em branco. Isso acontece porque o cálculo pode se referir a campos que não existem para outro tipo de objeto.

Por exemplo, você criou um campo calculado, &quot;Dias para concluir&quot;, para determinar quanto tempo levou para concluir uma tarefa em um projeto.

* WEEKDAYDIFF({atualStartDate},{atualCompletionDate})

Você deseja fazer a mesma coisa para uma iteração. Você pode usar a mesma expressão; no entanto, os campos disponíveis para um objeto de tarefa nem sempre estão disponíveis para um objeto de iteração. Então [!DNL Workfront] dá a você a chance de construir o cálculo com os campos de objeto corretos.

**Dica**: copie a expressão calculada da caixa Cálculo para o campo Instruções ao criar campos personalizados. Esse campo não é apagado quando um campo personalizado calculado é adicionado ao formulário personalizado na Biblioteca de campos.

Dependendo da necessidade, os campos calculados em formulários personalizados podem ser bastante simples ou muito complexos. As expressões podem incorporar ou aninhar outras expressões e valores para fornecer o nível de detalhes necessário para obter uma imagem melhor do que está acontecendo com o trabalho feito na organização.

<!--Depending on the need, calculated fields in custom forms can be quite simple or very complex. Expressions can embed, or nest, other expressions and values to provide the level of detail needed to get a better picture of what is going on with the work being done at your organization. 

Most of the examples and exercises in this course have been relatively simple to provide a base understanding of the expressions most commonly used and how to build those expressions in a custom calculated field. 

Now you’re ready to start building your own calculated custom fields.-->
