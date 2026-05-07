---
title: Exercício do módulo de comutação
description: Entenda como usar o módulo de comutação quando precisar executar transformações de dados mais complexas ou dinâmicas.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11052
thumbnail: KT11052.png
recommendations: noDisplay,catalog
exl-id: 1b810168-582d-4d7d-b061-d152af546bc8
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
autotag-review: '2026-05-06T16:40:26.747Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 327
ht-degree: 100%

---

# Exercício do módulo de comutação

Entenda como usar o módulo de comutação quando precisar executar transformações de dados mais complexas ou dinâmicas.

## Visão geral do exercício

Procure projetos de correspondência direta na unidade de teste e altere o nome de cada projeto com base num valor selecionado num campo personalizado anexado ao projeto.

![Módulo Alternar Imagem 1](../12-exercises/assets/switch-module-walkthrough-1.png)

## Etapas a serem seguidas

1. Crie um novo cenário e nomeie-o como “Usando o módulo Alternar”.
1. Para o módulo acionador, use o módulo Workfront Search.
1. Configure sua conexão com o Workfront e defina o tipo de registro como Projeto.
1. Nos critérios de Pesquisa, especifique que deseja ver apenas os projetos que têm um valor no campo personalizado Canal.
1. Para saídas, selecione ID, Nome, Número de referência e o campo personalizado Canal.

   ![Módulo Alternar Imagem 2](../12-exercises/assets/switch-module-walkthrough-2.png)

1. Adicione o módulo Alternar em Ferramentas.
1. Para o campo de Entrada, mapeie o campo personalizado Canal a partir do módulo de Pesquisa.

   ![Módulo Alternar Imagem 3](../12-exercises/assets/switch-module-walkthrough-3.png)

1. Em seguida, adicione casos para cada valor possível proveniente do campo personalizado Canal. O valor possível vai para o campo Padrão. Você deseja que o campo de saída inclua um código específico de três letras seguido pelo número de referência do projeto e, em seguida, o nome do projeto.

   **Seu painel de mapeamento deve ter esta aparência:**

   ![Módulo Alternar Imagem 4](../12-exercises/assets/switch-module-walkthrough-4.png)

1. Você pode incluir quantos casos adicionais desejar. Observe o campo Mais na parte inferior. Isso será usado se o valor de entrada não corresponder a nenhum dos casos.

   **Atualize o nome do projeto no Workfront.**

   ![Módulo Alternar Imagem 5](../12-exercises/assets/switch-module-walkthrough-5.png)

1. Adicione um módulo Atualizar registro do Workfront.
1. No campo ID, mapeie para a ID do módulo acionador.
1. Defina o tipo de registro como Projeto.
1. Selecione o campo Nome na seção Selecionar campos a serem mapeados e mapeie-o para a saída do módulo Alternar.
1. Salve seu cenário e execute uma vez. Visualize os nomes de projeto atualizados na unidade de teste.
