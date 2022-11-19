---
title: Padrões de roteamento
description: Reforce seu conceito de roteamento e rotas de fallback sem lidar com outras APIs.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11044
thumbnail: KT11044.png
exl-id: d8218115-5180-4e64-8ec1-d2d6afc88d23
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---

# Padrões de roteamento

Reforce seu conceito de roteamento e rotas de fallback sem lidar com outras APIs.

## Visão geral do exercício

Use o módulo Definir variável para enviar um número por vários caminhos e ver como os filtros e fallbacks se comportam ao rotear.

![Padrões de roteamento Imagem 1](../12-exercises/assets/routing-patterns-walkthrough-1.png)

## Etapas a seguir

1. Crie um novo cenário e o chame de &quot;Padrões de roteamento e fallbacks&quot;.
1. Para o acionador , adicione o módulo de ferramenta Definir variável . Coloque &quot;Meu número&quot; para o nome da variável, deixe o tempo de vida da variável como Um ciclo e defina o campo Variável como &quot;75&quot;.

   ![Padrões de roteamento Imagem 2](../12-exercises/assets/routing-patterns-walkthrough-2.png)

1. Adicione outro módulo e escolha o módulo Roteador. Para ambos os caminhos, escolha a ferramenta Incrementar função e clique em OK sem fazer alterações para cada um.

   + Para o primeiro caminho, crie um filtro, nomeie-o como &quot;Menos de 100&quot; e defina a condição como [Meu número] Menos de 100.

   + Para o segundo caminho, crie um filtro, nomeie-o como &quot;Menos de 1000&quot; e defina a condição como [Meu número] Menos de 1000. Use o operador Numérico para ambos.

   ![Padrões de roteamento Imagem 3](../12-exercises/assets/routing-patterns-walkthrough-3.png)

   ![Padrões de roteamento Imagem 4](../12-exercises/assets/routing-patterns-walkthrough-4.png)

1. Clique em Executar uma vez e observe o pacote passar pelo caminho &quot;Menos de 100&quot;.
1. Em seguida, altere o campo Set Variable module para 950 e Run again. Observe que ele corre pelo segundo caminho.
1. Clique no roteador e adicione mais um caminho. Adicione o módulo de ferramenta Increment function . Para o filtro, clique na caixa de seleção &quot;A rota de fallback&quot;. Observe como a seta apontando para esse caminho muda para um sinal de interpolação, indicando que é a rota de fallback.

   ![Padrões de roteamento Imagem 5](../12-exercises/assets/routing-patterns-walkthrough-5.png)

1. Altere o número da variável Set para 9500 e Run once. Como o número não é menor que 100 ou menos que 1000, o pacote percorre a rota de fallback.

Se você adicionar mais um caminho com um módulo de ferramenta de função Incrementar, mas não definir um filtro, o que acontecerá quando você clicar em Executar novamente? Um pacote poderá descer pela rota de fallback com a quarta rota adicionada?

+ Não, porque sem filtro definido, cada pacote sempre seguirá por esse caminho em vez da rota de fallback.
