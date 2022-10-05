---
title: Filtros
description: Saiba como usar o filtro entre módulos para permitir somente determinados tipos de pacotes.
feature: Workfront Fusion
role: User
level: Beginner
kt: 11040
thumbnail: KT1101.png
source-git-commit: f367e016498d5c1814cab79e19e6e9001db2851f
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---


# Filtros

Saiba como usar o filtro entre módulos para permitir somente determinados tipos de pacotes.

## Visão geral do exercício

Adicione um filtro entre os dois módulos no cenário de mapeamento Além do básico para criar apenas projetos que tenham uma cor de projeto &quot;Vermelho&quot; no arquivo CSV.

![Filtrar imagem 1](../12-exercises/assets/filters-walkthrough-1.png)

## Etapas a seguir

1. Crie um clone do cenário &quot;Além do mapeamento básico&quot; e o nomeie como &quot;Usando o filtro poderoso&quot;.

   **Adicione um filtro antes do módulo Criar projetos Workfront para permitir que apenas projetos vermelhos sejam criados.**

   ![Filtrar imagem 2](../12-exercises/assets/filters-walkthrough-2.png)

1. Adicione um filtro clicando na linha pontilhada conectando os módulos ou clicando na chave inglesa e selecionando Set up a filter.
1. Use o campo Label para nomear o filtro &quot;Somente projetos vermelhos&quot;.
1. No campo Condição , mapeie o campo Cor do projeto (Coluna 3 no arquivo CSV). Selecione o operador Equal to (não diferencia maiúsculas de minúsculas) e digite &quot;red&quot;.
1. Clique em OK.

   ![Filtrar imagem 3](../12-exercises/assets/filters-walkthrough-3.png)

   **Teste o filtro e verifique os resultados.**

1. Clique em Salvar para salvar o cenário e em Executar uma vez.
1. Clique no inspetor de execução do filtro para ver como cada pacote foi examinado pelo filtro e foi passado ou não foi movido para o módulo Criar projetos Workfront .

   ![Filtros Imagem 4](../12-exercises/assets/filters-walkthrough-4.png)

1. Encontre os projetos criados na sua instância do Workfront.
