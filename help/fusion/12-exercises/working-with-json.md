---
title: Exercício sobre trabalhar com JSON
description: Saiba como criar e analisar JSON em um cenário para atender às suas necessidades de design.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11056
thumbnail: KT11056.png
recommendations: noDisplay,catalog
exl-id: 72d5159e-72e5-4202-90de-753b3d7626de
source-git-commit: f033b210268e8979ee15abe812e6ad85673eeedb
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Exercício sobre trabalhar com JSON

Saiba como criar e analisar JSON em um cenário para atender às suas necessidades de design.

## Visão geral do exercício

O objetivo deste exercício é oferecer uma apresentação conceitual de como utilizar as informações enviadas para um cenário em formato JSON, analisando-as em campos e itens que você pode mapear em todo o cenário. Em seguida, é possível coletar informações dessas matrizes mapeadas ou agregar as informações no JSON para enviá-las a outro sistema que utiliza o JSON como um meio de recebimento.

![Trabalhar com JSON - Imagem 1](../12-exercises/assets/working-with-json-walkthrough-1.png)

## Etapas a serem seguidas

**Crie uma estrutura de dados e analise o JSON.**

1. Crie um novo cenário e nomeie-o como “Trabalhar com dados JSON de rosca”.
1. Para o módulo acionador, use o módulo Definir variável.
1. Digite “Dados em rosca” como o nome da variável.
1. Para o valor da variável, copie e cole o conteúdo do documento “_Donut Data - Sample JSON.rtf”, encontrado na pasta Arquivos de exercício do Fusion na sua unidade de teste.

   ![Trabalhar com JSON - Imagem 2](../12-exercises/assets/working-with-json-walkthrough-2.png)

1. Renomeie esse módulo como “JSON de outro conector”.
1. Adicione um módulo Analisar JSON.
1. Clique em Adicionar no campo Estrutura de dados.
1. Selecione o Gerador e cole os dados em rosca (dados JSON de amostra que você copiou para o campo Dados de amostra).

   ![Trabalhar com JSON - Imagem 3](../12-exercises/assets/working-with-json-walkthrough-3.png)

1. Clique em Salvar e nomeie a estrutura de dados como “Dados em rosca”. Em seguida, clique em Salvar.
1. Mapeie os dados em rosca do módulo Definir variável para o campo de string JSON.

   ![Trabalhar com JSON - Imagem 4](../12-exercises/assets/working-with-json-walkthrough-4.png)

1. Salve o cenário e clique em Executar uma vez para ver o resultado.

   **A saída do módulo Analisar JSON deve ter esta aparência:**

   ![Trabalhar com JSON - Imagem 5](../12-exercises/assets/working-with-json-walkthrough-5.png)

   **Definir variáveis de matriz específicas.**

1. Adicione um roteador após o módulo Analisar JSON.
1. No caminho superior, adicione um módulo Definir variáveis.
1. Insira “Tipos de massa por rosca” como o nome da variável.
1. Para o valor da variável, use a função de mapeamento para obter os tipos de massa da matriz Massas.

   ![Trabalhar com JSON - Imagem 6](../12-exercises/assets/working-with-json-walkthrough-6.png)

1. Clique em OK e depois em Executar uma vez.
1. Abra o inspetor de execução para ver o pacote resultante de cada uma das três operações, mostrando os tipos de massa para cada uma.

   ![Trabalhar com JSON - Imagem 7](../12-exercises/assets/working-with-json-walkthrough-7.png)

   **Agregar dados do cenário ao JSON.**

1. No caminho de roteamento inferior, adicione um módulo Agregar ao JSON.
1. No módulo de origem, escolha o iterador: o módulo Analisar JSON.
1. Em Estrutura de dados, crie ou escolha qualquer estrutura de dados. Neste exemplo, use Dados em rosca.
1. Prossiga e mapeie os campos diretamente neste exemplo, como mostrado abaixo.
1. Quando chegar às massas e coberturas, observe que elas são matrizes, o que significa que você precisa clicar em Adicionar item para mapeá-las.

   ![Trabalhar com JSON - Imagem 8](../12-exercises/assets/working-with-json-walkthrough-8.png)

1. Salve o cenário e clique em Executar uma vez.

Observe o inspetor de execução do módulo Agregar ao JSON e perceba como foram agregados três pacotes a uma única string JSON. Em seguida, você pode enviar essa string para outros sistemas que esperam o JSON.

![Trabalhar com JSON - Imagem 9](../12-exercises/assets/working-with-json-walkthrough-9.png)
