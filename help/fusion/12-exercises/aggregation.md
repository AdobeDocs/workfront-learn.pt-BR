---
title: Exercício de agregação
description: Saiba como agregar vários pacotes de informações em um mesmo valor.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11047
thumbnail: KT11047.png
recommendations: noDisplay,catalog
exl-id: 4626b623-8b05-41be-9cfc-917e28222855
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:46:06.511Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 302
ht-degree: 100%

---

# Exercício de agregação

Saiba como agregar vários pacotes de informações em um mesmo valor.

## Visão geral do exercício

Usando o cenário “Introdução à iteração” que você criou no último exercício, agregue as horas planejadas em cada tarefa em andamento do projeto e envie um email a si mesmo com essas informações.

![Agregação - Imagem 1](../12-exercises/assets/aggregation-walkthrough-1.png)

## Etapas a serem seguidas

**Adicione um filtro para SOMAR as horas planejadas.**

1. Clone o cenário “Introdução à iteração” criado no exercício anterior e nomeie-o como “Introdução à agregação”.
1. Adicione um filtro entre o módulo “Ler tarefas do projeto” e o módulo “Contar o número de tarefas”. Nomeie o filtro como “Somente tarefas em andamento”.
1. Defina a condição como “Número de tarefas derivadas” [Operador numérico: igual a] 0.

   ![Agregação - Imagem 2](../12-exercises/assets/aggregation-walkthrough-2.png)

1. Após o módulo “Matemática aleatória”, adicione um módulo de ferramenta “Agregador numérico”.
1. Defina o módulo de origem como “Ler tarefas do projeto”.
1. Defina a função “Agregar” como SOMA.
1. Defina o valor como o campo “Trabalho” do módulo “Ler tarefas do projeto”.
1. Renomeie este módulo como “SOMA de todas as horas planejadas da tarefa”.

   ![Agregação - Imagem 3](../12-exercises/assets/aggregation-walkthrough-3.png)

   **Observe a sombra que mostra que a agregação encerra a iteração.**

   ![Agregação - Imagem 4](../12-exercises/assets/aggregation-walkthrough-4.png)

   **Enviar um email com horas agregadas.**

1. Adicione um módulo “Enviar um email” do aplicativo de email após o agregador numérico.
1. Envie o email a si mesmo(a).
1. A linha de assunto deve ser “Detalhes do projeto”.
1. No campo “Conteúdo”, insira “Há um projeto chamado [nome do projeto] com um total de [resultado] horas planejadas”. O “[nome do projeto]” é retirado do módulo “Ler um registro”, e o “[resultado]” é retirado do módulo agregador.

   ![Agregação - Imagem 5](../12-exercises/assets/aggregation-walkthrough-5.png)

1. Salve e execute uma vez. Localize o email na sua caixa de entrada.

Os pacotes individuais podem ser acessados dentro da iteração. Porém fora da iteração, no módulo “Enviar um email”, somente os campos agregados podem ser acessados.
