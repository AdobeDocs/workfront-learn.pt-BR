---
title: Criar instruções OR em filtros
description: Saiba como usar uma instrução OU para informar à Workfront que você deseja ver essa instrução OU essa no seu relatório.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
thumbnail: create-or-statements-in-filters.png
type: Tutorial
role: User
level: Intermediate
kt: 9987
exl-id: 1a56f2f6-12df-43a5-943c-986a85661efa
source-git-commit: 252ba3ba44f22519a35899fcda9c6bca597a6c2c
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# Criar instruções OR em filtros

Por padrão, ao criar um filtro com várias linhas de critérios, o coloca um AND entre cada linha. Isso significa que cada resultado na lista quando você usa esse filtro atende a todas as regras de filtro.

Neste exemplo, temos três critérios, ou regras, para um filtro de projeto:

1. O projeto deve ter uma data de conclusão planejada que caia no mês atual.
1. O projeto deve estar no portfólio de Marketing de Eventos.
1. O projeto deve ser um projeto ativo, o que significa que deve ter um status Atual.

![Uma imagem da criação de um filtro com instruções AND em [!DNL Workfront]](assets/or-statement-1.png)

Os projetos na lista de resultados atendem a todos os três critérios, ajudando você a limitar os resultados da pesquisa para que você possa ver as informações exatas de que precisa.

![Uma imagem de uma lista filtrada em [!DNL Workfront]](assets/or-statement-2.png)

No entanto, pode haver momentos em que você queira que os resultados do filtro atendam a vários critérios, e é aí que as instruções OR podem ajudar. Com uma instrução OR, você está informando ao filtro que deseja ver este OU aquele.

## Uso de instruções OR

Instruções OR expandem ou aumentam a quantidade de informações que o filtro encontra porque, para ser exibido na lista de resultados, um item precisa atender apenas uma das regras de filtro, não todas.

Vamos analisar uma simples instrução OR: projetos que você é o gerente do projeto (proprietário) para projetos OR criados por você.

![Uma imagem da criação de um filtro com instruções OR em [!DNL Workfront]](assets/or-statement-3.png)

Depois de configurar ambas as regras de filtro, clique em E entre elas e alterne-a para OU.

![Uma imagem da criação de um filtro com instruções OR em [!DNL Workfront]](assets/or-statement-4.png)

O OU entre as duas regras de filtro expande seus critérios de pesquisa, informando à Workfront para encontrar projetos que atendam a uma ou outra dessas opções. Seu nome está no campo proprietário do projeto ou você é a pessoa que criou o projeto.

## Várias regras de filtro com instruções OR

Agora vamos observar uma instrução OU que contém várias regras de filtro em cada lado do OR. Isso usa as mesmas duas regras de antes, mas adiciona uma regra. Os projetos também devem ter um status Atual.

![Uma imagem da criação de um filtro com instruções OR em [!DNL Workfront]](assets/or-statement-5.png)

Observe que o Workfront &quot;agrupou&quot; as regras de filtro em cada lado do OU (há uma caixa cinza ao redor delas). Isso instrui a Workfront a executar as regras em cada lado do OR, localizando projetos que atendem a ambos os critérios, pois estão ligados com AND.

Neste exemplo, o Workfront procura por:

* Projetos que têm seu nome no campo proprietário do projeto que também têm um status Atual.
* **MAIS (OU)**
* Projetos criados por você que também têm status Atual.

Inserir a regra &quot;status do projeto igual a atual&quot; em cada lado do OR garante que a regra funcione em conjunto com cada uma das outras regras. Essa regra comum às vezes é chamada de &quot;constante&quot;.

>[!NOTE]
>
>Você não está limitado a uma regra de filtro repetida em cada lado do OR. Dependendo das suas necessidades, você pode ter várias. A Workfront recomenda manter essas regras repetidas no mínimo, para garantir que o filtro forneça os resultados necessários.

## O que acontece sem a regra de filtro comum?

Sem as regras de filtro comuns, você pode não obter os resultados da pesquisa previstos.

Por exemplo, se você colocar a regra &quot;status do projeto igual a atual&quot; somente em um lado do OR, ela só funcionará com as outras regras de filtro nessa seção. Na imagem abaixo, você vê que a regra &quot;status do projeto igual a atual&quot; está somente na seção superior.

![Uma imagem da criação de um filtro com instruções OR em [!DNL Workfront]](assets/or-statement-6.png)

Isso significa que a Workfront procurará:

* Projetos que têm seu nome no campo proprietário do projeto e têm um status Atual.
* **MAIS (OU)**
* Todos os projetos que você criou.

Como você pode ver, essa configuração de filtro fornece resultados ligeiramente diferentes do filtro com a regra de filtro repetida. É por isso que garantir que o filtro esteja configurado corretamente é importante para garantir que você obtenha os resultados desejados e necessários.

Você não pode usar as instruções OR frequentemente ao criar filtros. Mas fazer isso pode ajudar você a reduzir o número de filtros que precisam ser criados. Certifique-se de que os filtros não retornem muitos resultados. Uma lista longa pode dificultar a descoberta das informações exatas necessárias para os usuários.

## OU atividade de filtro

Você deseja encontrar tarefas incompletas que são atribuídas a você ou que não são atribuídas a ninguém. Você configurou um filtro para parecer com o abaixo. Esse filtro fornecerá os resultados desejados? Por que razão ou por que não?

![Uma imagem de uma instrução OR criada incorretamente em [!DNL Workfront]](assets/or-statement-your-turn-1.png)

### Respostas

Não, esse filtro não fornecerá os resultados que você espera — tarefas que não foram concluídas e que foram atribuídas a você ou atribuídas a ninguém — porque a regra de filtro para o status da tarefa está somente em um lado do OR.

Em vez disso, esse filtro gerará uma lista que mostra:

* Tarefas atribuídas a você que têm status Em andamento ou Novo.
* **MAIS (OU)**
* Todas as tarefas não atribuídas, independentemente do status.

O filtro deve ser semelhante ao abaixo. Observe que este filtro tem a regra de filtro para o status da tarefa em ambos os lados do OR.

![Uma imagem de uma instrução OR corretamente criada em [!DNL Workfront]](assets/or-statement-your-turn-2.png)
