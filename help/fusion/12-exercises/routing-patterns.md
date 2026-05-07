---
title: Exercício sobre padrões de roteamento
description: Reforce seu conceito de roteamento e rotas de fallback sem de fato lidar com outras APIs.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11044
thumbnail: KT11044.png
recommendations: noDisplay,catalog
exl-id: d8218115-5180-4e64-8ec1-d2d6afc88d23
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
autotag-review: '2026-05-06T16:42:16.496Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 361
ht-degree: 100%

---

# Exercício sobre padrões de roteamento

Reforce seu conceito de roteamento e rotas de fallback sem de fato lidar com outras APIs.

## Visão geral do exercício

Use o módulo Definir variável para enviar um número por vários caminhos e ver como os filtros e fallbacks se comportam durante o roteamento.

![Imagem 1 de padrões de roteamento](../12-exercises/assets/routing-patterns-walkthrough-1.png)

## Etapas a serem seguidas

1. Crie um novo cenário e nomeie-o “Padrões de roteamento e fallbacks”.
1. Para o acionador, adicione o módulo de ferramenta Definir variável. Coloque “Meu número” no nome da variável, deixe o tempo de vida da variável como Um ciclo e defina o campo Variável como “75”.

   ![Imagem 2 de padrões de roteamento](../12-exercises/assets/routing-patterns-walkthrough-2.png)

1. Adicione outro módulo e escolha o módulo Roteador. Para ambos os caminhos, escolha a ferramenta da função Incremento e clique em OK sem fazer alterações para cada um.

   + Para o primeiro caminho, crie um filtro, nomeie-o como “Menor que 100” e defina a condição como [Meu número] Menor que 100.

   + Para o segundo caminho, crie um filtro, nomeie-o como “Menos que 1.000” e defina a condição como [Meu número] Menor que 1.000. Use o operador numérico para ambos.

   ![Imagem 3 de padrões de roteamento](../12-exercises/assets/routing-patterns-walkthrough-3.png)

   ![Imagem 4 de padrões de roteamento](../12-exercises/assets/routing-patterns-walkthrough-4.png)

1. Clique em Executar uma vez e veja o pacote percorrer o caminho “Menor que 100”.
1. Em seguida, altere o campo do módulo Definir variável para 950 e clique novamente em Executar uma vez. Observe-o percorrer o segundo caminho.
1. Clique no roteador e adicione mais um caminho. Adicione o módulo de ferramenta da função Incremento. Para o filtro, clique na caixa de seleção “Rota de fallback”. Observe como a seta apontando para o caminho muda para um cursor de texto, indicando que é a rota de fallback.

   ![Imagem 5 de padrões de roteamento](../12-exercises/assets/routing-patterns-walkthrough-5.png)

1. Altere o número de Definir variável para 9.500 e clique em Executar uma vez. Como o número não é inferior a 100 nem inferior a 1.000, o pacote percorre a rota de fallback.

Se você adicionar mais um caminho com um módulo de ferramenta da função Incremento, mas não definir nenhum filtro, o que acontecerá quando você clicar novamente em Executar uma vez? Um pacote entrará na rota de fallback com a adição da quarta rota?

+ Não, porque sem um filtro definido, todos os pacotes sempre seguirão por esse caminho em vez da rota de fallback.
