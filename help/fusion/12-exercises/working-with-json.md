---
title: Trabalhar com JSON
description: Saiba como criar e analisar o JSON em um cenário para atender às suas necessidades de design.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11056
thumbnail: KT11056.png
exl-id: 72d5159e-72e5-4202-90de-753b3d7626de
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# Trabalhar com JSON

Saiba como criar e analisar o JSON em um cenário para atender às suas necessidades de design.

## Visão geral do exercício

O objetivo deste exercício é mostrar conceitualmente como utilizar informações enviadas em um cenário em um formato JSON, analisando-as em campos e itens que você pode mapear em todo o cenário. Em seguida, é possível coletar informações dessas matrizes mapeadas ou agregar as informações em JSON para, em seguida, serem enviadas para outro sistema que espera o JSON como uma entrada de recebimento.

![Trabalhar com imagem json 1](../12-exercises/assets/working-with-json-walkthrough-1.png)

## Etapas a serem seguidas

**Crie uma estrutura de dados e analise o JSON.**

1. Crie um novo cenário e nomeie-o como &quot;Trabalhando com dados de rosca JSON&quot;.
1. Para o módulo acionador, use o módulo Definir variável.
1. Para o nome da Variável, digite &quot;Dados em rosca&quot;.
1. Para o valor Variável, copie e cole o conteúdo do documento &quot;_Donut Data - Sample JSON.rtf&quot; encontrado na pasta Arquivos do Fusion Exercise na sua unidade de teste.

   ![Trabalhar com imagem json 2](../12-exercises/assets/working-with-json-walkthrough-2.png)

1. Renomeie esse módulo como &quot;JSON de outro conector&quot;.
1. Adicione um módulo JSON de análise.
1. Clique em Add para o campo Data structure.
1. Selecione o Gerador e cole os Dados de rosca - Dados JSON de amostra que você copiou para o campo Dados de amostra.

   ![Trabalhar com imagem json 3](../12-exercises/assets/working-with-json-walkthrough-3.png)

1. Clique em Salvar, nomeando a estrutura de dados como &quot;Dados em rosca&quot;. Em seguida, clique em Salvar.
1. Mapeie os dados de Rosca do módulo Definir variável para o campo de string JSON.

   ![Trabalhar com imagem json 4](../12-exercises/assets/working-with-json-walkthrough-4.png)

1. Salve o cenário e clique em Executar uma vez para ver a saída.

   **A saída do módulo JSON de análise deve ter esta aparência:**

   ![Trabalhar com imagem json 5](../12-exercises/assets/working-with-json-walkthrough-5.png)

   **Mapear para variáveis de matriz específicas.**

1. Adicione um roteador após o módulo JSON de análise.
1. No caminho superior, adicione um módulo Set variable.
1. Para o nome da Variável, digite &quot;Tipos de massa por rosca&quot;.
1. Para o valor Variable, use a função map para obter os tipos de baterias da matriz batters.

   ![Trabalhar com imagem json 6](../12-exercises/assets/working-with-json-walkthrough-6.png)

1. Clique em OK e depois em Executar uma vez.
1. Abra o inspetor de execução para ver o pacote de saída para cada uma das três operações, mostrando os tipos de bateria para cada uma.

   ![Trabalhar com imagem json 7](../12-exercises/assets/working-with-json-walkthrough-7.png)

   **Agregar dados do cenário ao JSON.**

1. No caminho de roteamento inferior, adicione uma agregação ao módulo JSON.
1. Para o Módulo de origem, escolha o iterador — o módulo JSON de análise.
1. Para a Estrutura de dados, crie ou escolha qualquer estrutura de dados. Neste exemplo, use dados de Rosca.
1. Vá em frente e mapeie os campos diretamente para este exemplo, como mostrado abaixo.
1. Quando você chegar ao topo e à massa, observe que são matrizes, então você precisa clicar em Adicionar item para mapeá-las.

   ![Trabalhar com imagem json 8](../12-exercises/assets/working-with-json-walkthrough-8.png)

1. Salve o cenário e clique em Executar uma vez.

Examine o inspetor de execução para o módulo Aggregate to JSON e observe como você pôde agregar três pacotes em uma única string JSON. Em seguida, você pode enviar essa cadeia de caracteres para outros sistemas que esperam JSON.

![Trabalhar com imagem json 9](../12-exercises/assets/working-with-json-walkthrough-9.png)
