---
title: Agregação avançada
description: Entenda como usar agrupamentos ao agregar. (Deve ter entre 60 e 160 caracteres, mas tem 49 caracteres)
feature: Workfront Fusion
role: User
level: Beginner
kt: 11048
thumbnail: KT11048.png
source-git-commit: 1f7a4da813805691fc0e52d3ad1ea708f9e07a9a
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---


# Agregação avançada

Entenda como usar agrupamentos ao agregar.

## Visão geral do exercício

Chame um serviço da Web para retornar detalhes sobre vários países e identificar a população total de todos os países, agrupada por sub-região.

![Imagem de Agregação Avançada 1](../12-exercises/assets/advanced-aggregation-walkthrough-1.png)

## Etapas a seguir

**Obtenha detalhes do país.**

![Imagem de Agregação Avançada 2](../12-exercises/assets/advanced-aggregation-walkthrough-2.png)

1. Crie um novo cenário e o nomeie como &quot;Agregação avançada&quot;.
1. Defina o módulo de acionador para um HTTP - Faça um módulo de solicitação.
1. Use este URL, https://restcountries.eu/rest/v2/ lang/es, que fornece uma lista de todos os países onde o espanhol é falado.
1. Deixe o Método como Get.
1. Clique na caixa de seleção Analisar resposta .
1. Renomeie este módulo como &quot;Obter países&quot;.
1. Clique em Salvar e executar uma vez.

   **O resultado é um único pacote, mas vem em uma matriz com 24 coleções, uma para cada país de língua espanhola.**

   ![Imagem de Agregação Avançada 3](../12-exercises/assets/advanced-aggregation-walkthrough-3.png)

   **É necessário coletar informações de sub-região para cada um dos países, de modo que será necessário fazer uma solicitação HTTP adicional.**

1. Adicione outra solicitação para obter informações da sub-região. Ele só retornará o primeiro país, mas está tudo bem por enquanto. Adicionar outro HTTP Faça um módulo de solicitação e use o URL https://restcountries.eu/rest/v2/name/.
1. Para obter o nome do primeiro país, vá para o painel de mapeamento, clique em Dados e, em seguida, em Nome na matriz. O [1] no campo de dados significa que ele retornará o primeiro item na matriz.

   + Clique no número e altere o índice, se necessário, mas, nesse caso, você deseja apenas o primeiro item.

   ![Imagem de Agregação Avançada 4](../12-exercises/assets/advanced-aggregation-walkthrough-4.png)

1. Marque a opção Parse response no painel de mapeamento e clique em OK.
1. Renomeie este &quot;Obter detalhes do país&quot;.
1. Clique em Salvar e, em seguida, em Executar uma vez.

   + O resultado são informações de um único país.

1. Para obter os outros países, você precisa iterar através da matriz. Adicione um iterador, que obtém uma lista de itens e gera um pacote para cada item na lista.

   **Adicione o iterador e o agregador.**

1. Clique com o botão direito do mouse entre os módulos HTTP e adicione o módulo Controle de fluxo do iterador.
1. No campo Array , selecione Data no módulo Get Countries .

   ![Imagem de Agregação Avançada 5](../12-exercises/assets/advanced-aggregation-walkthrough-5.png)

1. No módulo Obter detalhes do país, atualize o campo URL para obter o campo de nome do iterador em vez do módulo Obter países .

   ![Imagem de Agregação Avançada 6](../12-exercises/assets/advanced-aggregation-walkthrough-6.png)

1. Agora, adicione um agregador numérico depois de Obter detalhes do país para agrupar e somar as populações.
1. O módulo de origem é o módulo iterador.
1. A função de agregação é SUM.
1. O valor é [dados:público] no módulo Obter detalhes do país.
1. Clique na opção Mostrar configurações avançadas na parte inferior e agrupe por [dados:sub-região] no módulo Obter detalhes do país.

   ![Imagem de Agregação Avançada 7](../12-exercises/assets/advanced-aggregation-walkthrough-7.png)

   **Termine com um agregador de texto para agregar o que você agrupou no agregador numérico.**

1. Adicione um agregador de texto ao final.
1. O módulo de origem é o agregador numérico.
1. Na área de texto, insira &quot;O público total de [CHAVE] é [resultado].&quot;

   ![Imagem de Agregação Avançada 8](../12-exercises/assets/advanced-aggregation-walkthrough-8.png)

1. Salve e execute uma vez.

   + Revise a saída do módulo final.
