---
title: 'Prática recomendada: status'
description: Conheça as práticas recomendadas de especialistas do Adobe Workfront sobre configurar, gerenciar e usar os status do Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10926
exl-id: c3a4fe42-339c-4063-ad67-045868bbc6b1
TQID: https://experienceleague.adobe.com/Kn7jpCG-G7sEt6kKykK0MBlFTHkiXUqVC6mrodKm-rA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 591
ht-degree: 87%

---

# Prática recomendada: status

## O que é uma “prática recomendada” do Adobe Workfront?

As práticas recomendadas são diretrizes para um curso de ação eficaz e eficiente; elas podem ser facilmente adotadas por qualquer usuário da empresa e replicadas com sucesso em toda a organização.

Ao revisar essas recomendações, lembre-se de que algumas práticas recomendadas do Workfront são universais, enquanto outras podem ser mais específicas para um determinado assunto. Use essas práticas recomendadas como uma base para orientar as configurações e o uso do sistema do Workfront.

## Navegar nesta página

Ao percorrer esta página, você encontrará primeiro uma lista resumida de todas as práticas recomendadas para o tópico. Isso permite revisar as recomendações sem se aprofundar nos detalhes e motivos por trás delas.

A área &quot;Por que essas práticas recomendadas?&quot;, encontrada após a lista de alto nível, fornece mais detalhes sobre algumas das práticas recomendadas e por que elas são consideradas um processo, ferramenta etc., você deve considerar a implementação com sua instância do Workfront.

</br>
</br>

## Práticas recomendadas para status

* Ao renomear os status padrão do Workfront, mantenha a mesma finalidade original do status.

* Se você criar um status de projeto personalizado para “Cancelado”, iguale o status a “Inativo”.

* Reduza ao mínimo o número de status personalizados globais.

* Não use status de projeto no lugar de tarefas para indicar o andamento de um projeto.


</br>
</br>



## Por que essas práticas são recomendadas?

**Prática recomendada**

Ao renomear os status padrão do Workfront, mantenha a mesma finalidade original do status.



**Entenda o porquê**

Algumas ações no Workfront são acionadas por certos status padrão do sistema. Alterar a intenção de um status pode afetar o comportamento do Workfront em determinadas situações, afetar os relatórios etc.



Por exemplo, o status de tarefa padrão “Concluído” orienta o Workfront a alterar a porcentagem concluída de uma tarefa para 100%. O status “Concluído” também informa ao Workfront que o trabalho nas tarefas dependentes já pode ser iniciado. Se você tiver alterado o nome do status para “Aguardando” para indicar que o trabalho em uma tarefa está pausado, o Workfront interpretará a tarefa como concluída e iniciará as próximas etapas do projeto.

</br>
</br>



**Prática recomendada**

Se você criar um status de projeto personalizado para “Cancelado”, iguale o status a “Inativo”.



**Entenda o porquê**

Se você igualar “Cancelado” a “Concluído”, não poderá usar o status para cancelar um projeto, a menos que todas as tarefas sejam marcadas como concluídas e todos os problemas sejam resolvidos. No entanto, se você igualar “Cancelado” a “Inativo”, poderá cancelar o projeto sem precisar alterar o registro histórico.


</br>
</br>

**Prática recomendada**

Reduza ao mínimo o número de status personalizados globais.



**Entenda o porquê**

Menos é mais. Além de exigir um processo de manutenção desnecessário, utilizar muitos status personalizados gera confusão, principalmente em projetos multifuncionais. Em vez disso, utilize status personalizados apenas em grupos. Isso mantém o ambiente do Workfront mais organizado e melhor posicionado para a inclusão de outros grupos no futuro. Converse com o seu comitê de governança/supervisão e partes interessadas para identificar os status que os grupos da sua organização precisam usar.


</br>
</br>

**Prática recomendada**

Não use status de projeto no lugar de tarefas para indicar o andamento de um projeto.



**Entenda o porquê**

Mantenha os status do projeto simples para indicar fases de alto nível da progressão, como Planejamento, Atual, Concluído etc. Permita que as tarefas, os status das tarefas e o percentual de conclusão da tarefa informem como o trabalho está progredindo no geral no projeto. Esses indicadores de tarefas são acumulados na porcentagem total de conclusão do projeto, na condição do projeto e no status de progresso do projeto, e são indicadores melhores e mais precisos sobre o andamento do projeto se comparados ao status. Além disso, essas informações sobre as tarefas geram melhores relatórios de projeto.
