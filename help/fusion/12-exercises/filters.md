---
title: Exercício de filtros
description: Saiba como usar o filtro em vários módulos para encontrar somente determinados tipos de pacotes.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11040
thumbnail: KT1101.png
recommendations: noDisplay,catalog
exl-id: d2cec1ea-7ff9-48ae-8bfb-0c767d346079
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:43:22.961Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 230
ht-degree: 100%

---

# Exercício de filtros

Saiba como usar o filtro em vários módulos para encontrar somente determinados tipos de pacotes.

## Visão geral do exercício

Adicione um filtro para os dois módulos no cenário Além do mapeamento básico para criar apenas projetos que tenham a cor “Vermelho” no arquivo CSV.

![Filtros - Imagem 1](../12-exercises/assets/filters-walkthrough-1.png)

## Etapas a serem seguidas

1. Crie um clone do cenário “Além do mapeamento básico” e nomeie-o como “Usar o filtro avançado”.

   **Adicione um filtro no módulo Criar projetos do Workfront para permitir a criação apenas de projetos em vermelho.**

   ![Filtros - Imagem 2](../12-exercises/assets/filters-walkthrough-2.png)

1. Adicione um filtro clicando na linha pontilhada que conecta os módulos ou no ícone de chave inglesa e selecionando Configurar um filtro.
1. Use o campo Rótulo para nomear o filtro como “Somente projetos em vermelho”.
1. No campo Condição, mapeie o campo Cor do projeto (coluna 3 no arquivo CSV). Selecione o operador Igual a (sem distinção entre maiúsculas e minúsculas) e digite “vermelho”.
1. Clique em OK.

   ![Filtros - Imagem 3](../12-exercises/assets/filters-walkthrough-3.png)

   **Teste o filtro e verifique os resultados.**

1. Salve o cenário e clique em Executar uma vez.
1. Clique no inspetor de execução do filtro para ver como cada pacote foi examinado pelo filtro e se eles foram bem-sucedidos ou falharam na transição para o módulo Criar projetos do Workfront.

   ![Filtros - Imagem 4](../12-exercises/assets/filters-walkthrough-4.png)

1. Encontre os projetos criados na sua instância do Workfront.
