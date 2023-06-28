---
title: Prática recomendada - API Explorer
description: Explore as práticas recomendadas dos especialistas da Adobe Workfront para configurar, gerenciar e usar o API Explorer da Workfront.
feature: Workfront API
role: Admin, Leader, User
level: Beginner
jira: KT-10902
exl-id: 0f3fc5ba-d01a-4337-829f-def0830ddf81
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Prática recomendada - API Explorer

## O que é uma &quot;prática recomendada&quot; do Adobe Workfront?

As práticas recomendadas são diretrizes que representam um curso de ação eficaz e eficiente; são facilmente adotadas por você e pelos usuários em sua empresa; e podem ser replicadas com sucesso em toda a organização.

Ao revisar essas recomendações, lembre-se de que algumas práticas recomendadas do Workfront são universais, enquanto outras podem ser mais específicas ao tópico. Use essas práticas recomendadas como uma estrutura para ajudar a orientar as configurações e o uso do sistema Workfront.

## Navegando nesta página

Ao percorrer essa página, primeiro você encontrará uma lista de alto nível de todas as práticas recomendadas para o tópico. Isso permite analisar as recomendações sem mergulhar nos detalhes do &quot;por quê&quot;.

O &quot;Por que essas práticas recomendadas?&quot; A área, localizada após a lista de alto nível, fornece mais detalhes sobre algumas das práticas recomendadas e por que elas são consideradas um processo, ferramenta, etc. Você deve considerar a implementação com sua instância do Workfront.

</br>
</br>

## Práticas recomendadas do API Explorer

* Estabeleça uma convenção de nomenclatura para campos personalizados usados com integrações de sistemas de terceiros.

* Rastreie todos os campos personalizados usados em integrações usando um projeto do Workfront.

* Adicione o campo ID de objeto aos relatórios usados pelo administrador do sistema.

</br>
</br>

## Por que essas práticas recomendadas?

**Prática recomendada**

Estabeleça uma convenção de nomenclatura para campos personalizados usados com integrações de sistemas de terceiros.

**Veja o porquê**

Certifique-se de que todos os usuários que criam formulários personalizados conheçam a convenção de nomenclatura, para que não usem acidentalmente um campo reservado para uma integração. Dependendo das suas integrações e fluxos de trabalho, o uso do mesmo campo de várias maneiras pode resultar na modificação ou substituição dos dados, além de resultar em dados incorretos nos relatórios.

</br>
</br>


**Prática recomendada**

Rastreie todos os campos personalizados usados em integrações usando um projeto do Workfront.

**Veja o porquê**

Um projeto é o local perfeito para registrar nomes de campo personalizados, com que integração eles são usados, etc. Isso ajudará a evitar a criação de campos personalizados redundantes ou o uso do mesmo campo personalizado com várias integrações.

</br>
</br>


**Prática recomendada**

Adicione o campo ID de objeto aos relatórios usados pelo administrador do sistema.

**Veja o porquê**

Os administradores de sistema geralmente precisam se referir a objetos no Workfront por seus números de ID ao usar APIs ou outras integrações. Inclua o campo de ID nas exibições dos objetos em que você trabalha (projetos, tarefas, problemas, modelos, formulários personalizados etc.) para facilitar o acesso e a cópia.
