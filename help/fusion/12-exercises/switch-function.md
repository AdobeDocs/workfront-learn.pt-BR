---
title: Função de comutação
description: Saiba como usar a funcionalidade do switch usando a função Switch.
feature: Workfront Fusion
role: User
level: Beginner
kt: 11051
thumbnail: KT1101.png
source-git-commit: f367e016498d5c1814cab79e19e6e9001db2851f
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---


# Função de comutação

Saiba como usar a funcionalidade do switch usando a função Switch.

## Visão geral do exercício

Para alterações de dados simples, use a função Switch para transformar um valor em outro dentro de um campo de módulo. Neste exercício, altere a chave de duas letras para o nome real do status de progresso do projeto para enviar um email.

![Função de comutação Imagem 1](../12-exercises/assets/switch-function-walkthrough-1.png)

## Etapas a seguir

1. Clona o cenário chamado &quot;Compartilhando variáveis entre caminhos de roteamento&quot;.
1. Nomeie o novo cenário como &quot;Compartilhando variáveis entre caminhos de roteamento - Switch&quot;.
1. Clique no módulo de acionador e adicione Status de progresso à seção Saídas .
1. No módulo Enviar um email, adicione Status de progresso ao campo Conteúdo .

   + Se você apenas mapear o valor proveniente do módulo Pesquisa, há um código de duas letras para o status do progresso.
   + Para &quot;alternar&quot; o código para o nome completo de cada status de progresso possível, use a função &quot;alternar&quot; da guia General functions .

1. A função switch usa o valor ou a expressão Status do Progresso como uma chave e retorna o valor de saída com base nessa chave.

   + Um valor principal é definido na primeira posição após o Status do Progresso (&quot;LT&quot;) com a saída correspondente definida na segunda posição (&quot;Late&quot;).
   + O próximo valor principal é definido na terceira posição, com a saída correspondente definida na quarta posição, etc., para quantas chaves forem desejadas.

      ![Função de comutação Imagem 2](../12-exercises/assets/switch-function-walkthrough-2.png)