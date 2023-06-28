---
title: Filtros
description: Saiba como usar o filtro entre módulos para permitir somente determinados tipos de pacotes.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11040
thumbnail: KT1101.png
exl-id: d2cec1ea-7ff9-48ae-8bfb-0c767d346079
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# Filtros

Saiba como usar o filtro entre módulos para permitir somente determinados tipos de pacotes.

## Visão geral do exercício

Adicione um filtro entre os dois módulos no cenário Além do mapeamento básico para criar projetos com uma cor de projeto &quot;Vermelho&quot; no arquivo CSV.

![Imagem de filtros 1](../12-exercises/assets/filters-walkthrough-1.png)

## Etapas a serem seguidas

1. Crie um clone do cenário &quot;Além do mapeamento básico&quot; e o nomeie como &quot;Usando o filtro poderoso&quot;.

   **Adicione um filtro antes do módulo Criar projetos Workfront para permitir que somente projetos vermelhos sejam criados.**

   ![Imagem de filtros 2](../12-exercises/assets/filters-walkthrough-2.png)

1. Adicione um filtro clicando na linha pontilhada que conecta os módulos ou clicando na chave inglesa e selecionando Set up a filter.
1. Use o campo Rótulo para nomear o filtro como &quot;Somente projetos vermelhos&quot;.
1. No campo Condição, mapeie o campo Cor do projeto (coluna 3 no arquivo CSV). Selecione o operador Equal to (não diferencia maiúsculas de minúsculas) e digite &quot;red&quot;.
1. Clique em OK.

   ![Imagem de filtros 3](../12-exercises/assets/filters-walkthrough-3.png)

   **Teste o filtro e verifique os resultados.**

1. Clique em Salvar para salvar o cenário e em Executar uma vez.
1. Clique no inspetor de execução do filtro para ver como cada pacote foi examinado pelo filtro e passou ou falhou ao seguir para o módulo Criar projetos Workfront.

   ![Imagem de filtros 4](../12-exercises/assets/filters-walkthrough-4.png)

1. Encontre os projetos criados na sua instância do Workfront.
