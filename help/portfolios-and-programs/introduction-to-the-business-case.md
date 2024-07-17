---
title: Entenda sobre o [!UICONTROL Business Case]
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
ht-degree: 100%

---

# Entenda sobre o [!UICONTROL Business Case]

Como gerente, sua meta é garantir que os projetos contribuam de maneira positiva para os objetivos e iniciativas gerais da empresa. Para tomar decisões informadas, você precisa de informações de gerentes de projeto sobre o que é necessário para que seus projetos avancem. Isso pode ser feito através do [!UICONTROL Business Case].

## O que é um [!UICONTROL Business Case]?

Pense em um [!UICONTROL Business Case] como um blueprint ou proposta para o trabalho que precisa ser concluído. Ele captura estimativas preliminares de alto nível que ajudam você a planejar e gerenciar portfólios. É o local onde as possíveis despesas, recursos e riscos são inseridos para analisar os benefícios deste projeto para a empresa.

## Campos recomendados do [!UICONTROL Business Case] para a priorização de projetos

Cada seção do [!UICONTROL Business Case] fornece informações exclusivas e importantes sobre o projeto. Vamos dar uma olhada nas seções que fornecem informações à ferramenta [!UICONTROL Otimizador de portfólios], que ajuda a priorizar os projetos do seu portfólio.

## [!UICONTROL Informações do Projeto]

A maior parte das informações inseridas na seção [!UICONTROL Informações do projeto] envolve detalhes gerais do projeto, como o patrocinador do projeto e o programa ao qual o projeto pertence.

No entanto, há uma informação que pode afetar a priorização do projeto: o [!UICONTROL benefício planejado].

![Uma imagem da área [!UICONTROL Benefício planejado] na seção [!UICONTROL Informações do projeto] do [!UICONTROL Business Case]](assets/05-portfolio-management4.png)

O [!UICONTROL Benefício planejado] representa o valor estimado em dólares que sua empresa poderá receber se o projeto for concluído.

Esta é uma das seções que pode ser um ponto de inflexão para que sua empresa avance com o projeto. Se você puder mostrar que o projeto contribuirá significativamente para os resultados financeiros da sua empresa, maiores serão as chances de que ele seja implementado mais rapidamente.

## [!UICONTROL Despesas]

As [!UICONTROL Despesas] representam os custos não laborais que podem ser incorridos ao decorrer de um projeto.

![Uma imagem da seção [!UICONTROL Despesas] no [!UICONTROL Business Case]](assets/06-portfolio-management5.png)

Por exemplo, as despesas de uma conferência de usuários podem incluir o pagamento do local, presentes de recordação ou itens para a sinalização do lobby do local.

## [!UICONTROL Estimativa de Recurso]

A seção [!UICONTROL Orçamento de recursos] permite estimar a mão de obra que você considera necessária para o projeto avançar. As informações são extraídas do [!UICONTROL Planejador de recursos] do [!DNL Workfront's].

![Uma imagem da seção [!UICONTROL Orçamento de recursos] no [!UICONTROL Business Case]](assets/07-portfolio-management6.png)

Inserir as necessidades para cada função de trabalho permite criar um orçamento estimado do que é necessário para o projeto e fornece insights sobre os valores do orçamento do portfólio que poderão ser usados para o projeto.

>[!NOTE]
>
>Você deve ter conjuntos de recursos configurados no [!DNL Workfront] para usar esta seção do [!UICONTROL Business Case].

## [!UICONTROL Riscos]

Todos temos altas expectativas de que nosso projeto corra bem. Mas é importante identificar os riscos e criar um plano de ação adequado. A seção [!UICONTROL Riscos] do [!UICONTROL Business Case] pode ajudar com isso.

![Uma imagem da seção [!UICONTROL Riscos] no [!UICONTROL Business Case]](assets/08-portfolio-management7.png)

Você deve realizar um brainstorming com sua equipe e identificar possíveis riscos para o projeto. Quando for possível estimar a probabilidade de ocorrência e os custos resultantes de um risco, certifique-se de inserir esses valores. O Workfront multiplicará o custo potencial pela probabilidade e colocará esse valor em um fundo de [!UICONTROL Risco potencial], o qual será subtraído do [!UICONTROL Benefício planejado] do projeto ao calcular o [!UICONTROL Valor líquido].

## [!UICONTROL Scorecards]

[!UICONTROL Cartões de pontuação] ajudam a determinar até que ponto um projeto proposto se alinha com as metas e iniciativas gerais definidas para o portfólio ou para a empresa.

Cada cartão de pontuação tem uma lista de perguntas e respostas com valores associados a elas. Quando o cartão de pontuação estiver preenchido, o [!DNL Workfront] poderá calcular o quão alinhado está o projeto com os objetivos predeterminados da organização.

![Uma imagem da seção [!UICONTROL Cartões de pontuação] no [!UICONTROL Business Case]](assets/09-portfolio-management8.png)

>[!NOTE]
>
>Gerentes de projeto não poderão ver os valores atribuídos a cada resposta. Somente os usuários que criam os cartões de pontuação podem ver os valores.

## O [!UICONTROL Business Case] não é obrigatório

O [!UICONTROL Business Case] é flexível. Você pode preencher apenas algumas seções ou nenhuma. Nenhum dos campos é obrigatório. No entanto, quanto mais informações você preencher, mais fácil será analisar e priorizar projetos que contam com o mesmo orçamento ou recursos.

Depois de preencher o [!UICONTROL Business Case], clique no botão **[!UICONTROL Enviar]** no painel de resumo do lado direito da janela. Isso mudará o status do projeto para [!UICONTROL Solicitado]. Agora você pode usar a [!UICONTROL Otimização de portfólio] para priorizar projetos do mesmo portfólio.

>[!NOTE]
>
>A pontuação de alinhamento no painel de resumo do [!UICONTROL Business Case] é gerada quando você preenche o cartão de pontuação. A pontuação de alinhamento é um dos valores utilizados no cálculo da pontuação do [!UICONTROL  Otimizador de portfólio].

<!-- 
Learn more graphic and links to documentation articles
* Overview of areas of the business case 
* Create a business case for a project   
* Create a scorecard 
* Apply a scorecard to a project and generate an alignment score 
-->
