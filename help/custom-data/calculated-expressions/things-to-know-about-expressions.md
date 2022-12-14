---
title: O que você deve saber sobre expressões de campo calculado
description: Obtenha um vislumbre de uma lista de conceitos que são bons para saber ao trabalhar com campos calculados personalizados em [!DNL Workfront].
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: to-know-expressions.png
exl-id: 512a3071-f47f-4fd4-bf5f-9b18bef8ba59
source-git-commit: 402027429b116f3bd0328595b7c8635dea468fab
workflow-type: tm+mt
source-wordcount: '959'
ht-degree: 0%

---

# O que você deve saber sobre expressões de campo calculado

Esta é uma lista de conceitos que devem ser conhecidos ao trabalhar com campos calculados personalizados no Workfront.

## Casar assuntos em nomes de expressões

Quando se trata de nomes de expressões, o uso de maiúsculas e minúsculas é importante. Ao escrever inicialmente um nome de expressão, você pode usar letras maiúsculas, minúsculas ou uma combinação de ambos.

![Mensagem de erro sem maiúsculas no nome da expressão](assets/ttk-casingmatters01.png)

No entanto, a expressão deve ser escrita como todas as letras maiúsculas para que o sistema reconheça a expressão e salve o campo.



## As horas são armazenadas em minutos

As horas no banco de dados do Workfront são armazenadas em minutos. Se estiver fazendo referência a campos como Horas Planejadas ou Horas Reais, divida por 60 para mostrar o tempo em horas e não em minutos.

## O espaçamento não afeta expressões

A maneira recomendada para gravar expressões é com pouco ou nenhum espaçamento entre cada expressão.

* IF(ISBLANK({description}), &quot;Sem Descrição&quot;, &quot;Tem Descrição&quot;)

![Expressões sem espaçamento entre campos](assets/spacing01.png)

No entanto, se o espaçamento ajudar a visualizar o que está acontecendo, algum espaçamento poderá ser adicionado às expressões. Os espaços extras não devem impedir que a expressão reúna ou calcule um valor em [!DNL Workfront].

* IF (ISBLANK ({description}), &quot;Sem Descrição&quot;, &quot;Tem Descrição&quot; )

![Expressões com espaçamento entre campos](assets/spacing02.png)

As únicas coisas que não podem ter espaços entre elas são os campos e as chaves. Caso contrário, você receberá uma mensagem de erro e não poderá salvar o campo ou o formulário personalizado.

![Erro com espaçamento entre o nome do campo e o colchete](assets/spacing03.png)

## As aspas devem ser retas

Ao usar aspas em uma expressão, verifique se as aspas são retas (&quot;). Se as aspas estiverem curvas (&quot;), a [!DNL Workfront] O sistema continuará exibindo uma mensagem de &quot;Expressão personalizada inválida&quot;.

![Erro com aspas curvas](assets/curvedquotes01.png)

## Os cálculos são atualizados no salvamento do formulário e na edição de objetos

Esse é um aspecto importante dos campos calculados para serem compreendidos.

As informações exibidas em um campo calculado permanecerão as mesmas e se tornarão obsoletas, a menos que o formulário personalizado seja recalculado.

As expressões podem ser atualizadas usando a opção Recalcular expressões no menu Mais em um objeto.

Você deseja ver o número de dias em que um problema foi aberto. Crie um campo calculado chamado &quot;Dias abertos&quot; com a expressão DATEDIFF.

* Nome do campo = Dias abertos
* Expressão = DATEDIFF({entryDate},$$TODAY)

Depois de salvo, o número de dias entre a data em que o problema foi criado pela primeira vez ou inserido no Workfront e a data de hoje pode ser exibido na página de detalhes de um objeto ou em uma visualização de relatório.

Ao visualizar a mesma página de detalhes ou exibição de relatório no dia seguinte, você espera que esse número aumente em um. Se o número for 5 hoje, deverá ser 6 amanhã. O dia seguinte deve ser 7, 8, etc.

No entanto, o campo continuará sendo exibido 5 todos os dias. O campo deve ser &quot;executado novamente&quot; ou recalculado para atualizar as informações.

Para atualizar um campo usando a opção Recalcular expressões :

* Clique no nome do objeto para abri-lo.
* Clique no menu Mais .
* Selecione Recalcular expressões na lista.

![Opção Recalcular expressão no objeto](assets/recalculate01.png)

Também é possível recalcular várias expressões ao mesmo tempo usando o recurso &quot;edição em massa&quot; em uma lista ou relatório. Suponha que você tenha criado um relatório mostrando uma lista de problemas com o cálculo de Dias em Abertura que aparece em uma coluna. Se quiser recalcular todos os problemas de uma só vez:

* Selecione todos os problemas no relatório.
* Selecione a opção de edição para editar todos os problemas selecionados em massa.
* Clique no rótulo Forms personalizado à esquerda para rolar para baixo até a seção formulários personalizados.
* Marque a caixa Recalcular expressões personalizadas na parte inferior da seção Forms personalizado .
* Clique em Salvar alterações.

![Opção de expressão Recalculate para vários objetos](assets/recalculate02.png)

A tela é atualizada para mostrar informações atualizadas no campo calculado.

**Observação**: Embora existam outras maneiras de atualizar ou recalcular expressões em um campo calculado, essa é a maneira mais rápida e fácil.

## Os cálculos podem variar de formulário para formulário no mesmo campo

Assim que um campo calculado é salvo em um formulário personalizado e o formulário personalizado é salvo, o campo calculado é adicionado à Biblioteca de campos para que possa ser usado em outros formulários personalizados.

No entanto, se você tiver um campo calculado no formulário A e o mesmo campo calculado no formulário B, o pensamento inicial será que os cálculos são exatamente os mesmos. Nem sempre é assim. O campo calculado no formulário A pode ser calculado de forma totalmente diferente no formulário B.

Quando um campo personalizado calculado é selecionado da biblioteca de campos e adicionado a um formulário personalizado, o campo é adicionado, mas o cálculo fica em branco. Um motivo para isso acontecer é que o cálculo pode estar referindo-se a campos que não existem para outro tipo de objeto.

Por exemplo, você criou um campo calculado, &quot;Dias para concluir&quot;, para determinar o tempo necessário para concluir uma tarefa em um projeto.

* WEEKDAYDIFF({atualStartDate},{atualCompletionDate})

Você quer fazer a mesma coisa para uma iteração. Você pode usar a mesma expressão; no entanto, os campos disponíveis para um objeto de tarefa nem sempre estão disponíveis para um objeto de iteração. So [!DNL Workfront] oferece a chance de criar o cálculo com os campos de objeto corretos.

**Pro-dica**: Copie a expressão calculada da caixa Cálculo para o campo Instruções ao criar campos personalizados. Esse campo não é apagado quando um campo personalizado calculado é adicionado ao formulário personalizado da Biblioteca de campos.

Dependendo da necessidade, os campos calculados em formulários personalizados podem ser bastante simples ou complexos. As expressões podem incorporar ou aninhar outras expressões e valores para fornecer o nível de detalhes necessário para obter uma imagem melhor do que está acontecendo com o trabalho que está sendo feito em sua organização.

<!--Depending on the need, calculated fields in custom forms can be quite simple or very complex. Expressions can embed, or nest, other expressions and values to provide the level of detail needed to get a better picture of what is going on with the work being done at your organization. 

Most of the examples and exercises in this course have been relatively simple to provide a base understanding of the expressions most commonly used and how to build those expressions in a custom calculated field. 

Now you’re ready to start building your own calculated custom fields.-->
