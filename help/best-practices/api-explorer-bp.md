---
title: Prática recomendada - API Explorer
description: Explore as recomendações de práticas recomendadas dos especialistas do Adobe Workfront sobre como configurar, gerenciar e usar o Workfront API Explorer.
feature: Workfront API
role: Admin, Leader, User
level: Beginner
kt: 10902
exl-id: 0f3fc5ba-d01a-4337-829f-def0830ddf81
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Prática recomendada - API Explorer

## O que é uma &quot;prática recomendada&quot; do Adobe Workfront?

As melhores práticas são orientações que representam uma linha de ação eficaz e eficiente; sejam adotados facilmente por você e pelos usuários em sua empresa; e podem ser replicados com êxito em toda a organização.

À medida que você revisa essas recomendações, lembre-se de que algumas práticas recomendadas do Workfront são universais, enquanto outras podem ser mais específicas para o tópico. Use essas práticas recomendadas como estrutura para ajudar a orientar as configurações e o uso do sistema Workfront.

## Navegar nesta página

Ao rolar por essa página, primeiro você encontrará uma lista de alto nível de todas as práticas recomendadas para o tópico. Isso permite que você revise as recomendações sem entrar nos detalhes de &quot;por quê&quot;.

O &quot;Por que essas práticas recomendadas estão sendo usadas?&quot; , encontrada após a lista de alto nível, fornece mais detalhes sobre algumas práticas recomendadas e por que elas são consideradas como um processo, ferramenta etc., você deve considerar a implementação com sua instância do Workfront.

</br>
</br>

## Práticas recomendadas do API Explorer

* Estabeleça uma convenção de nomenclatura para campos personalizados usados com integrações de sistemas de terceiros.

* Rastreie todos os campos personalizados usados em integrações usando um projeto do Workfront.

* Adicione o campo de ID de objeto aos relatórios usados pelo administrador do sistema.

</br>
</br>

## Por que essas práticas recomendadas estão presentes?

**Prática recomendada**

Estabeleça uma convenção de nomenclatura para campos personalizados usados com integrações de sistemas de terceiros.

**Veja o porquê**

Certifique-se de que todos os usuários que criam formulários personalizados saibam sobre a convenção de nomenclatura, para que não utilizem acidentalmente um campo reservado para uma integração. Dependendo de suas integrações e fluxos de trabalho, o uso do mesmo campo de várias maneiras pode resultar na modificação ou substituição de dados, e pode resultar em dados incorretos nos relatórios.

</br>
</br>


**Prática recomendada**

Rastreie todos os campos personalizados usados em integrações usando um projeto do Workfront.

**Veja o porquê**

Um projeto torna o local perfeito para registrar nomes de campo personalizados, com que integração eles são usados etc. Isso ajudará você a evitar a criação de campos personalizados redundantes ou o uso do mesmo campo personalizado com várias integrações.

</br>
</br>


**Prática recomendada**

Adicione o campo de ID de objeto aos relatórios usados pelo administrador do sistema.

**Veja o porquê**

Os administradores do sistema geralmente precisam se referir a objetos no Workfront por seus números de ID ao usar APIs ou outras integrações. Inclua o campo ID nas exibições dos objetos em que você trabalha (projetos, tarefas, problemas, modelos, formulários personalizados, etc.) para facilitar o acesso e a cópia.
