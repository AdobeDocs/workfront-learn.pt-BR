---
title: Exercício sobre a função Alternar
description: Saiba como alternar funcionalidades utilizando a função Alternar.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11051
thumbnail: KT1101.png
recommendations: noDisplay,catalog
exl-id: 3142fae2-5210-4f63-9d2c-66dec58867fa
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
autotag-review: '2026-05-06T16:41:24.173Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 240
ht-degree: 100%

---

# Exercício sobre a função Alternar

Saiba como alternar funcionalidades utilizando a função Alternar.

## Visão geral do exercício

Para alterações simples de dados, use a função Alternar para transformar um valor de um campo de módulo em outro valor. Neste exercício, altere a chave de duas letras para o nome real do status de progresso do projeto e envie-o por email.

![Função Alternar - Imagem 1](../12-exercises/assets/switch-function-walkthrough-1.png)

## Etapas a serem seguidas

1. Clone o cenário chamado “Compartilhar variáveis entre caminhos de roteamento”.
1. Nomeie o novo cenário como “Compartilhamento de variáveis entre caminhos de roteamento - Alternar”.
1. Clique no módulo acionador e adicione Status do progresso à seção Saídas.
1. No módulo Enviar um email, adicione Status do progresso ao campo Conteúdo.

   + Se você apenas sobrescrever o valor proveniente do módulo Pesquisar, haverá um código de duas letras como o status do progresso.
   + Para “alternar” o código pelo nome completo de cada possível status do progresso, use a função “alternar” da guia Funções gerais.

1. A função Alternar usa o valor ou expressão do status do progresso como chave e, em seguida, retorna o valor de saída com base nessa chave.

   + Um valor-chave é definido na primeira posição após o status do progresso (“AT”) com a saída correspondente definida na segunda posição (“Atrasado”).
   + O valor-chave seguinte é definido na terceira posição, com a saída correspondente definida na quarta posição, e esse processo se repete para o número de chaves desejadas.

     ![Função Alternar - Imagem 2](../12-exercises/assets/switch-function-walkthrough-2.png)
