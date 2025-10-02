---
title: Criar instruções OU em filtros
description: A lógica de filtro flexível do Workfront permite que os usuários refinem as exibições de relatórios usando regras "AND" padrão, condições "OR" opcionais e grupos de filtros organizados para critérios complexos.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
thumbnail: create-or-statements-in-filters.png
type: Tutorial
role: User
level: Intermediate
jira: KT-9987
exl-id: 1a56f2f6-12df-43a5-943c-986a85661efa
last-substantial-update: 2025-08-11T00:00:00Z
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 31%

---

# Criar instruções OU em filtros

O vídeo explica como criar e usar filtros com várias regras no Workfront. &#x200B; Por padrão, o Workfront usa &quot;E&quot; entre as regras de filtro, o que significa que todas as condições devem ser verdadeiras para um item aparecer na lista.
Como alternativa, é possível alterar a lógica do filtro para &quot;OU&quot;, que exibe itens que atendem a qualquer uma das condições.
O vídeo também demonstra como criar filtros para tarefas usando grupos de filtros. &#x200B; Por exemplo, você pode criar dois grupos: um para tarefas incompletas atribuídas à equipe criativa que estão atrasadas e outro para tarefas incompletas atribuídas à equipe criativa que não estão atribuídas. &#x200B; Em cada grupo, a lógica &quot;AND&quot; se aplica, o que significa que todas as condições no grupo devem ser atendidas. &#x200B; A lógica &quot;OR&quot; entre grupos garante que as tarefas que atendem às condições de cada grupo sejam exibidas.

>[!VIDEO]&#x200B;(https://video.tv.adobe.com/v/3470698/?quality=12&learn=on&enablevpops=0&captions=por_br)

## Atividade de filtro OU

Você deseja encontrar tarefas incompletas atribuídas a você ou que não foram atribuídas a ninguém. Você configurou um filtro semelhante ao abaixo. Este filtro fornecerá os resultados desejados? Por que ou por que não?

![Uma imagem de uma instrução OU criada incorretamente no [!DNL Workfront]](assets/or-statement-your-turn-1.png)

### Respostas

Não, esse filtro não fornecerá os resultados desejados — tarefas não concluídas que não foram atribuídas a você ou atribuídas a ninguém — porque a regra de filtro para a conclusão da tarefa está somente em um lado do OR.

Em vez disso, esse filtro gerará uma lista que mostra:

* Tarefas atribuídas a você que não estão concluídas.
* **MAIS (OU)**
* Todas as tarefas não atribuídas, independentemente do status.

O filtro deve ser semelhante ao mostrado abaixo. Observe que esse filtro tem a regra de filtro para a integridade de tarefas em ambos os lados do OR.

![Uma imagem de uma instrução OU criada corretamente no [!DNL Workfront]](assets/or-statement-your-turn-2.png)
