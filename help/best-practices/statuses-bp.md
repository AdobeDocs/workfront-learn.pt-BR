---
title: Prática recomendada - Status
description: Explore as recomendações de práticas recomendadas dos especialistas do Adobe Workfront sobre como configurar, gerenciar e usar os status do Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
kt: 10926
exl-id: c3a4fe42-339c-4063-ad67-045868bbc6b1
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 0%

---

# Prática recomendada - Status

## O que é uma &quot;prática recomendada&quot; do Adobe Workfront?

As melhores práticas são orientações que representam uma linha de ação eficaz e eficiente; sejam adotados facilmente por você e pelos usuários em sua empresa; e podem ser replicados com êxito em toda a organização.

À medida que você revisa essas recomendações, lembre-se de que algumas práticas recomendadas do Workfront são universais, enquanto outras podem ser mais específicas para o tópico. Use essas práticas recomendadas como estrutura para ajudar a orientar as configurações e o uso do sistema Workfront.

## Navegar nesta página

Ao rolar por essa página, primeiro você encontrará uma lista de alto nível de todas as práticas recomendadas para o tópico. Isso permite que você revise as recomendações sem entrar nos detalhes de &quot;por quê&quot;.

O &quot;Por que essas práticas recomendadas estão sendo usadas?&quot; , encontrada após a lista de alto nível, fornece mais detalhes sobre algumas práticas recomendadas e por que elas são consideradas como um processo, ferramenta etc., você deve considerar a implementação com sua instância do Workfront.

</br>
</br>

## Práticas recomendadas para status

* Ao renomear os status padrão do Workfront, mantenha a finalidade original do status igual.

* Se você criar um status de projeto personalizado para Cancelado, equipare o status a Adiado.

* Reduza os status personalizados globais.

* Não use os status do projeto no lugar de tarefas para indicar a progressão de um projeto.


</br>
</br>



## Por que essas práticas recomendadas estão presentes?

**Prática recomendada**

Ao renomear os status padrão do Workfront, mantenha a finalidade original do status igual.



**Veja o porquê**

Algumas ações no Workfront são acionadas pelos status padrão do sistema. Alterar a intenção de um status pode afetar o comportamento do Workfront em determinadas situações, afetar os relatórios etc.



Por exemplo, o status padrão da tarefa de Concluir informa ao Workfront para alterar a porcentagem de conclusão de uma tarefa para 100%. O status Concluído também permite que a Workfront saiba que o trabalho em tarefas dependentes pode começar. Se você alterou o nome do status para Aguardando, para indicar que um trabalho em uma tarefa está pausado, o Workfront pensará que a tarefa foi concluída e iniciará as próximas etapas no projeto.

</br>
</br>



**Prática recomendada**

Se você criar um status de projeto personalizado para Cancelado, equipare o status a Adiado.



**Veja o porquê**

Se você equipar Cancelado com Concluído, não poderá usar o status para cancelar um projeto, a menos que todas as tarefas sejam marcadas como concluídas e todos os problemas sejam fechados. Mas se você equipar Cancelado com Atrasado, poderá cancelar o projeto sem alterar nada no registro histórico.


</br>
</br>

**Prática recomendada**

Reduza os status personalizados globais.



**Veja o porquê**

Menos é mais. Além de criar manutenção desnecessária, muitos status personalizados criam confusão, especialmente ao trabalhar em projetos multifuncionais. Em vez disso, torne os status personalizados específicos do grupo. Isso mantém o ambiente do Workfront mais limpo e melhor posicionado para expansão em outros grupos no futuro. Trabalhe com seu comitê de governança/supervisão e com os participantes para identificar os status que os grupos de sua organização precisam usar.


</br>
</br>

**Prática recomendada**

Não use os status do projeto no lugar de tarefas para indicar a progressão de um projeto.



**Veja o porquê**

Mantenha os status do projeto simples para indicar fases de alto nível de progressão, como Planejamento, Atual, Concluído etc. Deixe que as tarefas, os status da tarefa e a porcentagem de tarefas concluídas informem como o trabalho está progredindo no projeto. Esses indicadores de nível de tarefa são acumulados na porcentagem de conclusão do projeto, na condição do projeto e no status do progresso do projeto, todos melhores e mais precisos indicadores de progressão do projeto do que um status do projeto. Além disso, essas informações de nível de tarefa fornecem melhores relatórios do projeto.
