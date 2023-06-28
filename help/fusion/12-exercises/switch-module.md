---
title: Módulo de comutação
description: Entenda como usar o módulo Switch quando precisar executar transformações de dados mais complexas ou dinâmicas.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11052
thumbnail: KT11052.png
exl-id: 1b810168-582d-4d7d-b061-d152af546bc8
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 0%

---

# Módulo de comutação

Entenda como usar o módulo Switch quando precisar executar transformações de dados mais complexas ou dinâmicas.

## Visão geral do exercício

Procure projetos de correspondência direta na unidade de teste e altere o nome de cada projeto com base em um valor selecionado em um campo personalizado anexado ao projeto.

![Módulo do switch Imagem 1](../12-exercises/assets/switch-module-walkthrough-1.png)

## Etapas a serem seguidas

1. Crie um novo cenário e nomeie-o como &quot;Usando o módulo Switch&quot;.
1. Para o módulo acionador, use o módulo Workfront Search.
1. Configure sua conexão com o Workfront e defina o tipo de registro como Projeto.
1. Nos critérios de Pesquisa, especifique que deseja ver apenas os projetos que têm um valor no campo personalizado Canal.
1. Para saídas, selecione ID, Name, Reference Number e o campo personalizado Channel.

   ![Imagem 2 do módulo do switch](../12-exercises/assets/switch-module-walkthrough-2.png)

1. Adicione o módulo Switch em Ferramentas.
1. Para o campo de Entrada, mapeie o campo personalizado Canal do módulo de Pesquisa.

   ![Imagem 3 do módulo do switch](../12-exercises/assets/switch-module-walkthrough-3.png)

1. Em seguida, adicione casos para cada valor possível vindo do campo personalizado Channel. O valor possível vai para o campo Pattern. Você deseja que o campo de saída inclua um código específico de 3 letras seguido pelo número de referência do projeto e, em seguida, o nome do projeto.

   **Seu painel de mapeamento deve ter esta aparência:**

   ![Imagem 4 do módulo do switch](../12-exercises/assets/switch-module-walkthrough-4.png)

1. Você pode adicionar quantos casos adicionais desejar. Observe o campo Else na parte inferior. Isso será usado se o valor de entrada não corresponder a nenhum dos casos.

   **Atualize o nome do projeto no Workfront.**

   ![Imagem 5 do módulo do switch](../12-exercises/assets/switch-module-walkthrough-5.png)

1. Adicione um módulo Atualizar registro do Workfront.
1. No campo ID, mapeie para a ID do módulo do acionador.
1. Defina o Tipo de registro como Projeto.
1. Selecione o campo Nome na seção Selecionar campos a serem mapeados e mapeie-o para a saída do módulo Switch.
1. Salve o cenário e execute uma vez. Exibir os nomes de projeto atualizados na unidade de teste.
