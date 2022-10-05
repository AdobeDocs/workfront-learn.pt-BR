---
title: Prática recomendada - Relatório do modo de texto
description: Explore as recomendações de práticas recomendadas dos especialistas do Adobe Workfront sobre como configurar, gerenciar e usar os relatórios do modo de texto do Workfront.
feature: Reports and Dashboards
role: Admin, Leader, User
level: Beginner
kt: 10928
exl-id: c624545c-ba42-4cc3-aafe-8be15baadb75
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---

# Prática recomendada - Relatório do modo de texto

## O que é uma &quot;prática recomendada&quot; do Adobe Workfront?

As melhores práticas são orientações que representam uma linha de ação eficaz e eficiente; sejam adotados facilmente por você e pelos usuários em sua empresa; e podem ser replicados com êxito em toda a organização.

À medida que você revisa essas recomendações, lembre-se de que algumas práticas recomendadas do Workfront são universais, enquanto outras podem ser mais específicas para o tópico. Use essas práticas recomendadas como estrutura para ajudar a orientar as configurações e o uso do sistema Workfront.

## Navegar nesta página

Ao rolar por essa página, primeiro você encontrará uma lista de alto nível de todas as práticas recomendadas para o tópico. Isso permite que você revise as recomendações sem entrar nos detalhes de &quot;por quê&quot;.

O &quot;Por que essas práticas recomendadas estão sendo usadas?&quot; , encontrada após a lista de alto nível, fornece mais detalhes sobre algumas práticas recomendadas e por que elas são consideradas como um processo, ferramenta etc., você deve considerar a implementação com sua instância do Workfront.

</br>
</br>

## Práticas recomendadas para relatórios do modo de texto

* Use expressões de valor do modo de texto em vez de campos personalizados calculados sempre que possível em colunas de relatório de lista.

* Coloque os cálculos usados em um cálculo do modo de texto na descrição do relatório.

</br>
</br>

## Por que essas práticas recomendadas estão presentes?

**Prática recomendada**

Use expressões de valor do modo de texto em vez de campos personalizados calculados sempre que possível em colunas de relatório de lista.



**Veja o porquê**

As expressões de valor do modo de texto são calculadas no momento em que o relatório é executado e são recalculadas sempre que o relatório é atualizado. Isso significa que você sempre terá dados atualizados e relatórios precisos.



Os campos personalizados calculados (usados em formulários personalizados) não são atualizados automaticamente quando os dados são exibidos no Workfront. Em vez disso, eles exibem os resultados do cálculo mais recente armazenado no Workfront. Isso significa que esses valores podem estar &quot;obsoletos&quot; ou desatualizados em qualquer momento. Os campos personalizados calculados devem ser atualizados manualmente, recalcular a expressão ou editando e salvando o objeto que contém o campo calculado. Isso pode ser demorado, assim como fácil de esquecer.


</br>
</br>

**Prática recomendada**

Coloque os cálculos usados em um cálculo do modo de texto na descrição do relatório.



**Veja o porquê**

Incluir quaisquer cálculos do modo de texto na descrição do relatório ajuda outras pessoas a entender como o cálculo foi criado e que tipo de informação deve ser exibida. Ele também lembra aos administradores do sistema como o relatório foi criado, caso sejam necessárias atualizações no futuro.
