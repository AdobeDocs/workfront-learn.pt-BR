---
title: Módulo de switch
description: Entenda como usar o módulo Switch quando precisar executar transformações de dados mais complexas ou dinâmicas.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11052
thumbnail: KT11052.png
exl-id: 1b810168-582d-4d7d-b061-d152af546bc8
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Módulo de switch

Entenda como usar o módulo Switch quando precisar executar transformações de dados mais complexas ou dinâmicas.

## Visão geral do exercício

Procure projetos de correspondência direta na unidade de teste e altere o nome de cada projeto com base em um valor selecionado em um campo personalizado anexado ao projeto.

![Módulo de switch Imagem 1](../12-exercises/assets/switch-module-walkthrough-1.png)

## Etapas a seguir

1. Crie um novo cenário e o nomeie como &quot;Usando o módulo Switch&quot;.
1. Para o módulo acionador, use o módulo Pesquisa do Workfront.
1. Configure sua conexão com o Workfront e defina o tipo de registro como Projeto.
1. Nos critérios de Pesquisa, especifique que deseja ver apenas os projetos que têm um valor no campo personalizado Canal .
1. Para saídas, selecione ID, Nome, Número de referência e o campo personalizado Canal .

   ![Módulo de switch Imagem 2](../12-exercises/assets/switch-module-walkthrough-2.png)

1. Adicione o módulo Switch a partir de Ferramentas.
1. Para o campo Input , mapeie o campo personalizado Channel do módulo Search .

   ![Módulo de switch Imagem 3](../12-exercises/assets/switch-module-walkthrough-3.png)

1. Em seguida, adicione casos para cada valor possível proveniente do campo personalizado Canal . O valor possível vai para o campo Padrão. Você deseja que o campo de saída inclua um código de 3 letras específico seguido pelo número de referência do projeto e, em seguida, pelo nome do projeto.

   **O painel de mapeamento deve ter esta aparência:**

   ![Módulo de switch Imagem 4](../12-exercises/assets/switch-module-walkthrough-4.png)

1. Você pode adicionar quantos casos adicionais desejar. Observe o campo Else na parte inferior. Isso será usado se o valor de entrada não corresponder a nenhum dos casos.

   **Atualize o nome do projeto no Workfront.**

   ![Módulo de switch Imagem 5](../12-exercises/assets/switch-module-walkthrough-5.png)

1. Adicione um módulo Workfront Update Record.
1. No campo ID , mapeie para a ID do módulo do acionador.
1. Defina o Tipo de Registro como Projeto.
1. Selecione o campo Nome na seção Selecionar campos para mapear e mapeie-o para a saída do módulo Switch.
1. Salve o cenário e execute uma vez. Exiba os nomes de projeto atualizados em sua unidade de teste.
