---
title: Prática recomendada - Relatório no modo de texto
description: Explore as recomendações de práticas recomendadas dos especialistas do Adobe Workfront sobre a configuração, gerenciamento e uso dos relatórios em modo de texto do Workfront.
feature: Reports and Dashboards
role: Admin, Leader, User
level: Beginner
jira: KT-10928
exl-id: c624545c-ba42-4cc3-aafe-8be15baadb75
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---

# Prática recomendada - Relatório no modo de texto

## O que é uma &quot;prática recomendada&quot; do Adobe Workfront?

As práticas recomendadas são diretrizes que representam um curso de ação eficaz e eficiente; são facilmente adotadas por você e pelos usuários em sua empresa; e podem ser replicadas com sucesso em toda a organização.

Ao revisar essas recomendações, lembre-se de que algumas práticas recomendadas do Workfront são universais, enquanto outras podem ser mais específicas ao tópico. Use essas práticas recomendadas como uma estrutura para ajudar a orientar as configurações e o uso do sistema Workfront.

## Navegando nesta página

Ao percorrer essa página, primeiro você encontrará uma lista de alto nível de todas as práticas recomendadas para o tópico. Isso permite analisar as recomendações sem mergulhar nos detalhes do &quot;por quê&quot;.

O &quot;Por que essas práticas recomendadas?&quot; A área, localizada após a lista de alto nível, fornece mais detalhes sobre algumas das práticas recomendadas e por que elas são consideradas um processo, ferramenta, etc. Você deve considerar a implementação com sua instância do Workfront.

</br>
</br>

## Práticas recomendadas para relatórios no modo de texto

* Use expressões de valor em modo texto em vez de campos personalizados calculados sempre que possível nas colunas de relatório de lista.

* Coloque cálculos usados em um cálculo de modo de texto na descrição do relatório.

</br>
</br>

## Por que essas práticas recomendadas?

**Prática recomendada**

Use expressões de valor em modo texto em vez de campos personalizados calculados sempre que possível nas colunas de relatório de lista.



**Veja o porquê**

As expressões de valor em modo de texto são calculadas no momento em que o relatório é executado e são recalculadas sempre que o relatório é atualizado. Isso significa que você sempre terá dados atualizados e relatórios precisos.



Os campos personalizados calculados (usados em formulários personalizados) não são atualizados automaticamente quando os dados são exibidos no Workfront. Em vez disso, eles exibem os resultados do cálculo mais recente armazenado no Workfront. Isso significa que esses valores podem estar &quot;obsoletos&quot; ou desatualizados em um determinado momento. Os campos personalizados calculados devem ser atualizados manualmente, recalculando a expressão ou editando e salvando o objeto que contém o campo calculado. Isso pode ser demorado, bem como fácil de esquecer de fazer.


</br>
</br>

**Prática recomendada**

Coloque cálculos usados em um cálculo de modo de texto na descrição do relatório.



**Veja o porquê**

Incluir qualquer cálculo em modo de texto na descrição do relatório ajuda outras pessoas a entender como o cálculo foi criado e que tipo de informação ele deve ser exibido. Ele também lembra aos administradores de sistema como o relatório foi criado, caso atualizações sejam necessárias no futuro.
