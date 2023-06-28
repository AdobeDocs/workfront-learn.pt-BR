---
title: Agregação
description: Saiba como agregar vários pacotes de informações em um único valor.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11047
thumbnail: KT11047.png
exl-id: 4626b623-8b05-41be-9cfc-917e28222855
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---

# Agregação

Saiba como agregar vários pacotes de informações em um único valor.

## Visão geral do exercício

Usando o cenário &quot;Introdução à iteração&quot; que você criou no último exercício, agregue as horas planejadas em cada tarefa em funcionamento no projeto e envie um email para você mesmo com essas informações.

![Imagem de Agregação 1](../12-exercises/assets/aggregation-walkthrough-1.png)

## Etapas a serem seguidas

**Adicione um filtro e SOME as horas planejadas.**

1. Clone o cenário &quot;Introdução à iteração&quot; criado no exercício anterior e nomeie-o como &quot;Introdução à agregação&quot;.
1. Adicione um filtro entre o módulo Ler tarefas do projeto e o módulo Contar o número de tarefas. Nomeie o filtro como &quot;Somente tarefas em execução&quot;.
1. Defina a condição como Número de filhos [Operador Numérico: Igual a] 0.

   ![Imagem de Agregação 2](../12-exercises/assets/aggregation-walkthrough-2.png)

1. Após o módulo Matemática Aleatória, adicione um módulo de ferramenta Agregador Numérico.
1. Defina o módulo de origem para Ler tarefas do projeto.
1. Defina a função Aggregate como SUM.
1. Defina o Valor no campo Trabalho do módulo Ler tarefas do projeto.
1. Renomeie este módulo como &quot;SOMA de todas as horas planejadas da tarefa&quot;.

   ![Imagem de Agregação 3](../12-exercises/assets/aggregation-walkthrough-3.png)

   **Observe a sombra que mostra que a agregação encerra a iteração.**

   ![Imagem de Agregação 4](../12-exercises/assets/aggregation-walkthrough-4.png)

   **Envie um email com horas agregadas.**

1. Adicione um módulo Enviar email do aplicativo Email, após o agregador numérico.
1. Envie o email para si mesmo.
1. A linha de assunto é &quot;Detalhes do projeto&quot;.
1. No campo Conteúdo, coloque &quot;Existe um projeto chamado [nome do projeto] que tem um número total de [resultado] horas planejadas.&quot; O &quot;[nome do projeto]&quot; é retirado do módulo Ler um registro e &quot;[resultado]&quot; é retirado do módulo agregador.

   ![Imagem de Agregação 5](../12-exercises/assets/aggregation-walkthrough-5.png)

1. Salvar e executar uma vez. Localize o email em sua caixa de entrada.

Na iteração, os pacotes individuais podem ser acessados. Mas fora da iteração, no módulo Send an email, somente os campos agregados podem ser acessados.
