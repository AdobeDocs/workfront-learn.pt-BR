---
title: Trabalhar com JSON
description: Saiba como criar e analisar o JSON em um cenário para atender às suas necessidades de design.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11056
thumbnail: KT11056.png
exl-id: 72d5159e-72e5-4202-90de-753b3d7626de
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# Trabalhar com JSON

Saiba como criar e analisar o JSON em um cenário para atender às suas necessidades de design.

## Visão geral do exercício

A finalidade deste exercício é mostrar conceitualmente como utilizar as informações enviadas para um cenário em um formato JSON, analisando-as em campos e itens que você pode mapear no cenário. Em seguida, você pode coletar informações desses arrays mapeados ou agregar as informações em JSON para então ser enviado a outro sistema que espera JSON como entrada de recebimento.

![Trabalhar com a imagem json 1](../12-exercises/assets/working-with-json-walkthrough-1.png)

## Etapas a seguir

**Crie uma estrutura de dados e analise o JSON.**

1. Crie um novo cenário e o nomeie como &quot;Trabalhando com dados de rosca JSON&quot;.
1. Para o módulo de acionador, use o módulo Definir variável .
1. Para o nome da variável, digite &quot;Dados de rosca&quot;.
1. Para o valor Variável, copie e cole o conteúdo do documento &quot;_Donut Data - Sample JSON.rtf&quot; encontrado na pasta Arquivos de Exercício de Fusão na unidade de teste.

   ![Trabalhar com a imagem json 2](../12-exercises/assets/working-with-json-walkthrough-2.png)

1. Renomeie este módulo como &quot;JSON de outro conector&quot;.
1. Adicione um módulo JSON de análise.
1. Clique em Add para o campo Data structure .
1. Selecione o Gerador e cole os dados de rosca - Amostra de dados JSON que você copiou para o campo de dados de amostra .

   ![Trabalhando com a imagem json 3](../12-exercises/assets/working-with-json-walkthrough-3.png)

1. Clique em Salvar, nomeando a estrutura de dados como &quot;Dados de rosca&quot;. Em seguida, clique em Salvar.
1. Mapeie os dados de Rosca do módulo de variável Set para o campo de string JSON.

   ![Trabalhando com a imagem json 4](../12-exercises/assets/working-with-json-walkthrough-4.png)

1. Salve o cenário e clique em Executar uma vez para ver a saída.

   **A saída do módulo JSON de análise deve ser semelhante a esta:**

   ![Trabalhar com a imagem json 5](../12-exercises/assets/working-with-json-walkthrough-5.png)

   **Mapeie para variáveis específicas de matriz.**

1. Adicione um roteador após o módulo JSON de análise.
1. No caminho superior, adicione um módulo Definir variável.
1. Para o nome da variável, digite &quot;Tipos de lote por rosca&quot;.
1. Para o valor Variable , use a função map para obter os tipos de bateria da matriz batters.

   ![Trabalhar com a imagem json 6](../12-exercises/assets/working-with-json-walkthrough-6.png)

1. Clique em OK e em Executar uma vez.
1. Abra o inspetor de execução para ver o pacote de saída para cada uma das três operações, mostrando os tipos de bateria para cada uma.

   ![Trabalhando com a imagem json 7](../12-exercises/assets/working-with-json-walkthrough-7.png)

   **Agregar dados de cenário ao JSON.**

1. No caminho de roteamento inferior, adicione um Aggregate ao módulo JSON.
1. Para o Módulo de Origem, escolha o iterador — o módulo JSON de Análise.
1. Para a Estrutura de dados, crie ou escolha qualquer estrutura de dados. Neste exemplo, use dados de Rosca.
1. Vá em frente e mapeie os campos diretamente para este exemplo, conforme mostrado abaixo.
1. Quando chegar ao batedor e ao topo, observe que são arrays, portanto, é necessário clicar em Adicionar item para mapeá-los.

   ![Trabalhando com a imagem json 8](../12-exercises/assets/working-with-json-walkthrough-8.png)

1. Salve o cenário e clique em Executar uma vez.

Examine o Inspetor de execução do módulo Aggregate to JSON e observe como você conseguiu agregar três pacotes em uma única string JSON. Em seguida, você pode enviar essa sequência de caracteres para outros sistemas que esperam JSON.

![Trabalhando com a imagem json 9](../12-exercises/assets/working-with-json-walkthrough-9.png)
