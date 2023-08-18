---
title: Compreender o [!UICONTROL Business Case]
description: Saiba como usar o [!UICONTROL Business Case] no Workfront para avaliar projetos solicitados e compará-los com outros projetos em seu portfólio.
activity: use
team: Technical Marketing
feature: Strategic Planning
thumbnail: introduction-to-the-business-case.png
type: Tutorial
last-substantial-update: 2023-08-18T00:00:00Z
jira: KT-13836
role: User
level: Intermediate
exl-id: febb7378-81d4-4348-ac57-e9c4756966c0
source-git-commit: 64789af613bd6b38e58bd2c15df622729b883b22
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 0%

---

# Compreender o [!UICONTROL Business Case]

Como gerente, é seu objetivo garantir que os projetos contribuam para as metas e iniciativas gerais da empresa de forma positiva. Para tomar decisões conscientes, você precisa de informações dos gerentes de projeto sobre o que eles precisarão para que seus projetos avancem. Isso pode ser feito por meio da [!UICONTROL Business Case].

## O que é uma [!UICONTROL Business Case]?

Pense em um [!UICONTROL Business Case] como um blueprint ou proposta para o trabalho que precisa ser feito. Ele captura estimativas preliminares de alto nível que ajudam a planejar e gerenciar portfólios. É onde possíveis despesas, recursos e riscos são inseridos para criar um &quot;caso&quot; sobre por que esse projeto beneficiaria a empresa.

## [!UICONTROL Business Case] campos recomendados para priorização de projeto

Cada seção do [!UICONTROL Business Case] O fornece informações exclusivas e importantes sobre o projeto. Vamos analisar as seções que fornecem informações para o [!UICONTROL Otimizador de Portfolio] , que ajudará você a priorizar os projetos no seu portfólio.

## [!UICONTROL Informações do Projeto]

A maioria das informações inseridas no [!UICONTROL Informações do projeto] Esta seção envolve detalhes gerais do projeto, como o patrocinador do projeto e o programa ao qual o projeto pertence.

No entanto, há uma informação que pode afetar a priorização do projeto...[!UICONTROL Benefício Planejado].

![Uma imagem do [!UICONTROL Benefício Planejado] na área [!UICONTROL Informações do projeto] seção do [!UICONTROL Business Case]](assets/05-portfolio-management4.png)

A variável [!UICONTROL Benefício Planejado] representa o valor em dólar estimado do qual sua empresa pode se beneficiar se o projeto for concluído.

Essa é uma das seções que podem ser um ponto de inflexão para fazer com que sua empresa avance com esse projeto. Se você puder mostrar que o projeto contribuirá significativamente para os resultados financeiros da sua empresa, então as chances são maiores de que ele possa ser enviado mais rapidamente.

## [!UICONTROL Despesas]

[!UICONTROL Despesas] representam os custos não mão de obra que podem ser incorridos durante a vida útil de um projeto.

![Uma imagem do [!UICONTROL Despesas] na seção [!UICONTROL Business Case]](assets/06-portfolio-management5.png)

Por exemplo, as despesas de uma conferência de usuários podem incluir o pagamento do local, itens para sacos de presente ou sinais para o lobby do local.

## [!UICONTROL Estimativa de Recurso]

A variável [!UICONTROL Estimativa de Recursos] permite estimar a mão de obra que você acha que será necessária para o projeto avançar. As informações são extraídas do [!DNL Workfront's] [!UICONTROL Planejador de recursos].

![Uma imagem do [!UICONTROL Estimativa de Recursos] na seção [!UICONTROL Business Case]](assets/07-portfolio-management6.png)

Inserindo necessidades estimadas para cada função de trabalho, isso cria um orçamento possível necessário para o projeto e fornece informações sobre quanto do orçamento do portfólio pode ser usado para o projeto.

>[!NOTE]
>
>É necessário ter conjuntos de recursos configurados em [!DNL Workfront] para usar esta seção do [!UICONTROL Business Case].

## [!UICONTROL Riscos]

Você sempre tem a maior esperança de que seu projeto funcione sem problemas. Mas é importante identificar os riscos e planejá-los de acordo. É aí que o [!UICONTROL Riscos] na seção [!UICONTROL Business Case] pode ajudar.

![Uma imagem do [!UICONTROL Riscos] na seção [!UICONTROL Business Case]](assets/08-portfolio-management7.png)

Você deve fazer um brainstorming com sua equipe e identificar quaisquer riscos ao projeto. Para riscos em que você pode estimar o custo se o risco ocorrer e a probabilidade de que ele ocorrerá, certifique-se de inserir esses valores. A Workfront multiplicará o custo potencial pela probabilidade e colocará isso em uma [!UICONTROL Risco potencial] fundo que será subtraído do orçamento do projeto [!UICONTROL Benefício Planejado] ao calcular sua [!UICONTROL Valor Líquido].

## [!UICONTROL Scorecards]

[!UICONTROL Scorecards] ajuda a determinar como um projeto proposto se alinha às metas e iniciativas gerais definidas para o portfólio ou para a empresa.

Cada cartão de pontuação tem uma lista de perguntas e respostas com valores anexados a elas. Quando o cartão de pontuação é preenchido, [!DNL Workfront] O pode calcular o alinhamento do projeto com as metas predeterminadas de sua organização.

![Uma imagem do [!UICONTROL Scorecards] na seção [!UICONTROL Business Case]](assets/09-portfolio-management8.png)

>[!NOTE]
>
>Os gerentes de projeto não poderão ver os valores atribuídos a cada resposta. Somente os usuários que criam os cartões de pontuação podem ver os valores.

## [!UICONTROL Business Case] não obrigatório

A variável [!UICONTROL Business Case] O é flexível. Você pode preencher apenas algumas seções ou nenhuma. Nenhum dos campos é obrigatório. No entanto, quanto mais informações você preencher, mais fácil será analisar e priorizar projetos que disputam o mesmo orçamento ou recursos.

Quando a variável [!UICONTROL Business Case] for preenchido, clique no link **[!UICONTROL Enviar]** no painel de resumo no lado direito da janela. Isso alterará o status do projeto para [!UICONTROL Solicitado]. Agora você está pronto para usar [!UICONTROL Otimização de Portfolio] para priorizar projetos no mesmo portfólio.

>[!NOTE]
>
>A pontuação de alinhamento no [!UICONTROL Business Case] o painel de resumo é gerado ao preencher o cartão de pontuação. A pontuação de alinhamento é um dos valores usados no cálculo da [!UICONTROL Otimizador de Portfolio] pontuação.

<!-- 
Learn more graphic and links to documentation articles
* Overview of areas of the business case 
* Create a business case for a project   
* Create a scorecard 
* Apply a scorecard to a project and generate an alignment score 
-->
