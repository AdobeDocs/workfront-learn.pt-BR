---
title: Criar instruções OR em filtros
description: Saiba como usar uma instrução OR para informar ao Workfront que você deseja ver isso OU aquilo em seu relatório.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
thumbnail: create-or-statements-in-filters.png
type: Tutorial
role: User
level: Intermediate
jira: KT-9987
exl-id: 1a56f2f6-12df-43a5-943c-986a85661efa
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '915'
ht-degree: 0%

---

# Criar instruções OR em filtros

Ao criar um filtro com várias linhas de critérios, por padrão, o Workfront coloca um AND entre cada linha. Isso significa que cada resultado na lista quando você usa esse filtro atende a todas as regras de filtro.

Neste exemplo, temos três critérios, ou regras, para um filtro de projeto:

1. O projeto deve ter uma data de conclusão planejada para o mês atual.
1. O projeto deve estar no portfólio de Marketing de eventos.
1. O projeto deve ser um projeto ativo, o que significa que deve ter um status Atual.

![Uma imagem de criação de um filtro com instruções AND em [!DNL Workfront]](assets/or-statement-1.png)

Os projetos na lista de resultados atendem a todos esses três critérios, ajudando a restringir os resultados da pesquisa para que você possa ver as informações exatas de que precisa.

![Uma imagem de uma lista filtrada no [!DNL Workfront]](assets/or-statement-2.png)

No entanto, pode haver ocasiões em que você deseje que os resultados do filtro atendam a vários critérios e, nesse momento, as instruções OR podem ajudar. Com uma instrução OR, você informa ao filtro que deseja ver itens que correspondam a QUALQUER UMA de suas instruções OR, em vez de TODAS as suas instruções AND.

## Uso de instruções OR

As instruções OR expandem ou aumentam a quantidade de informações que o filtro encontra porque, para aparecer na lista de resultados, um item precisa atender apenas a uma das regras de filtro, não a todas.

Vejamos uma instrução OR simples: projetos que você é o gerente (proprietário) de projetos OR que foram criados por você.

![Uma imagem de criação de um filtro com instruções OR em [!DNL Workfront]](assets/or-statement-3.png)

Após configurar ambas as regras de filtro, clique no AND entre elas e alterne-o para OR.

![Uma imagem de criação de um filtro com instruções OR em [!DNL Workfront]](assets/or-statement-4.png)

O OR entre as duas regras de filtro expande os critérios de pesquisa, informando ao Workfront para localizar projetos que atendam a uma ou outra dessas opções: seu nome está no campo de proprietário do projeto ou você é a pessoa que criou o projeto.

## Várias regras de filtro com instruções OR

Agora vamos observar uma instrução OR que contém várias regras de filtro em cada lado do OR. Isso usa as mesmas duas regras de antes, mas adiciona uma regra: os projetos também devem ter um status Atual.

![Uma imagem de criação de um filtro com instruções OR em [!DNL Workfront]](assets/or-statement-5.png)

Observe que o Workfront &quot;agrupou&quot; as regras de filtro em cada lado do OR (há uma caixa cinza ao redor delas). Isso instrui o Workfront a executar as regras em cada lado do OR em conjunto, localizando projetos que atendem a ambos os critérios porque estão unidos com AND.

Neste exemplo, o Workfront procura por:

* Projetos que têm seu nome no campo proprietário do projeto e também o status Atual.
* **MAIS (OU)**
* Projetos que você criou que também têm um status de Atual.

Inserir a regra &quot;status do projeto igual ao atual&quot; em cada lado do OR garante que a regra funcione em conjunto com cada uma das outras regras. Essa regra comum às vezes é chamada de &quot;constante&quot;.

>[!NOTE]
>
>Você não está limitado a uma regra de filtro repetida em cada lado do OR. Dependendo das suas necessidades, você pode ter vários. A Workfront recomenda manter essas regras repetidas no mínimo, para garantir que o filtro forneça os resultados necessários.

## O que acontece sem a regra de filtro comum?

Sem as regras de filtro comuns, talvez você não obtenha os resultados da pesquisa previstos.

Por exemplo, se você colocar a regra &quot;status do projeto igual a Atual&quot; somente em um lado do OR, ela só funcionará com as outras regras de filtro nessa seção. Na imagem abaixo, você vê que a regra &quot;status do projeto igual ao atual&quot; está somente na seção superior.

![Uma imagem de criação de um filtro com instruções OR em [!DNL Workfront]](assets/or-statement-6.png)

Isso significa que a Workfront procurará:

* Projetos que têm seu nome no campo proprietário do projeto e o status Atual.
* **MAIS (OU)**
* Todos os projetos criados.

Como você pode ver, essa configuração de filtro fornece resultados um pouco diferentes do filtro com a regra de filtro repetida. É por isso que garantir que o filtro esteja configurado corretamente é importante para garantir que você obtenha os resultados desejados e necessários.

Não é possível usar instruções OR com frequência ao criar filtros. Mas isso pode ajudá-lo a reduzir o número de filtros que precisam ser criados. Apenas certifique-se de que seus filtros não retornem muitos resultados - uma longa lista pode dificultar a localização das informações exatas necessárias para os usuários.

## Atividade de filtro OU

Você deseja encontrar tarefas incompletas que estão atribuídas a você ou que não estão atribuídas a ninguém. Você configura um filtro para ser semelhante ao mostrado abaixo. Esse filtro fornecerá os resultados desejados? Por que ou não?

![Imagem de uma instrução OR criada incorretamente em [!DNL Workfront]](assets/or-statement-your-turn-1.png)

### Respostas

Não, esse filtro não fornecerá os resultados desejados — tarefas não concluídas que não foram atribuídas a você ou atribuídas a ninguém — porque a regra de filtro para o status da tarefa está somente em um lado do OR.

Em vez disso, esse filtro gerará uma lista que mostra:

* Tarefas atribuídas a você com status Em andamento ou Novo.
* **MAIS (OU)**
* Todas as tarefas não atribuídas, independentemente do status.

O filtro deve ter a aparência abaixo. Observe que esse filtro tem a regra de filtro para o status da tarefa em ambos os lados do OR.

![Imagem de uma instrução OR criada corretamente em [!DNL Workfront]](assets/or-statement-your-turn-2.png)
