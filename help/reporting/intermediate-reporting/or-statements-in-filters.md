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
last-substantial-update: '2025-08-11T00:00:00.000Z'
doc-type: video
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: c6dd2ac5-f5bd-4e59-9101-25b156918623
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-06T02:11:54.379Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 318
ht-degree: 31%

---

# Criar instruções OU em filtros

O vídeo explica como criar e usar filtros com várias regras no Workfront. &#x200B; Por padrão, o Workfront usa &quot;E&quot; entre as regras de filtro, o que significa que todas as condições devem ser verdadeiras para um item aparecer na lista.
Como alternativa, é possível alterar a lógica do filtro para &quot;OU&quot;, que exibe itens que atendem a qualquer uma das condições.
O vídeo também demonstra como criar filtros para tarefas usando grupos de filtros. &#x200B; Por exemplo, você pode criar dois grupos: um para tarefas incompletas atribuídas à equipe criativa que estão atrasadas e outro para tarefas incompletas atribuídas à equipe criativa que não estão atribuídas. &#x200B; Em cada grupo, a lógica &quot;AND&quot; se aplica, o que significa que todas as condições no grupo devem ser atendidas. &#x200B; A lógica &quot;OR&quot; entre grupos garante que as tarefas que atendem às condições de cada grupo sejam exibidas.

>[!VIDEO](https://video.tv.adobe.com/v/3470692/?quality=12&learn=on&enablevpops=0)

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
