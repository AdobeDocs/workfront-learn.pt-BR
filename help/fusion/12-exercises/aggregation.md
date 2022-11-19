---
title: Agregação
description: Saiba como agregar vários pacotes de informações em um único valor.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11047
thumbnail: KT11047.png
exl-id: 4626b623-8b05-41be-9cfc-917e28222855
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---

# Agregação

Saiba como agregar vários pacotes de informações em um único valor.

## Visão geral do exercício

Usando o cenário &quot;Introdução à iteração&quot; criado no último exercício, agregue as horas planejadas em cada tarefa de trabalho no projeto e envie um email para você com essas informações.

![Imagem de Agregação 1](../12-exercises/assets/aggregation-walkthrough-1.png)

## Etapas a seguir

**Adicione um filtro e SUM nas horas planejadas.**

1. Clona o cenário &quot;Introdução à iteração&quot; criado no exercício anterior e o nomeie como &quot;Introdução à agregação&quot;.
1. Adicione um filtro entre o módulo Ler tarefas do projeto e o módulo Contar o número de tarefas . Nomeie o filtro como &quot;Somente tarefas de trabalho&quot;.
1. Defina a condição como Number of Children [Operador numérico: Igual a] 0.

   ![Imagem de Agregação 2](../12-exercises/assets/aggregation-walkthrough-2.png)

1. Depois do módulo Matemática Aleatória, adicione um módulo de ferramenta Agregador Numérico.
1. Defina o módulo de origem como Ler Tarefas do Projeto.
1. Defina a função Aggregate como SUM.
1. Defina o Valor para o campo Trabalho no módulo Ler Tarefas do Projeto.
1. Renomeie este módulo como &quot;SOMA de todas as horas de execução da tarefa&quot;.

   ![Imagem de Agregação 3](../12-exercises/assets/aggregation-walkthrough-3.png)

   **Observe a sombra que mostra que a agregação termina a iteração.**

   ![Imagem de Agregação 4](../12-exercises/assets/aggregation-walkthrough-4.png)

   **Envie um email com horas agregadas.**

1. Adicione um módulo Send an email from the Email app, após o agregador numérico.
1. Envie o email para você mesmo.
1. A linha de assunto é &quot;Detalhes do projeto&quot;.
1. No campo Conteúdo , coloque &quot;Há um projeto chamado [nome do projeto] que tem um número total de [resultado] horas planejadas.&quot; O &quot;[nome do projeto]&quot; é retirado do módulo Ler um Registro e &quot;[resultado]&quot; é retirado do módulo agregador.

   ![Imagem de Agregação 5](../12-exercises/assets/aggregation-walkthrough-5.png)

1. Salve e execute uma vez. Localize o email na sua caixa de entrada.

Dentro da iteração, os pacotes individuais podem ser acessados. Mas fora da iteração, no módulo Enviar um email, somente os campos agregados podem ser acessados.
