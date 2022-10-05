---
title: Repositórios de dados
description: Saiba como sincronizar nomes de empresas entre dois sistemas. (Deve ter entre 60 e 160 caracteres, mas tem 59 caracteres)
feature: Workfront Fusion
role: User
level: Beginner
kt: 11055
thumbnail: KT11055.png
source-git-commit: c348222464180e994e7b414d1b84e07f58b6b2ae
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 0%

---


# Repositórios de dados

Saiba como sincronizar nomes de empresas entre dois sistemas.

## Visão geral do exercício

Esta é a primeira parte de uma sincronização unidirecional de empresas no Workfront e em outro sistema. Por enquanto, ele só sincroniza entre um armazenamento de dados Fusion e o Workfront. Uma tabela em um armazenamento de dados rastreia a Workfront ID (WFID) e a ID da empresa no arquivo CSV (CID) de cada empresa. Isso permite uma sincronização bidirecional em algum ponto no futuro.

![Armazenamento de dados Imagem 1](../12-exercises/assets/data-stores-walkthrough-1.png)

## Etapas a seguir

**Baixe o arquivo do Workfront.**

1. Na pasta &quot;Fusion Exercise Files&quot; da Workfront, selecione &quot;_Companies.csv&quot; e clique em Detalhes do Documento.
1. Copie o primeiro número de ID do endereço de URL.
1. Em Fusion, crie um novo cenário chamado &quot;Uso de armazenamentos de dados para sincronizar dados&quot;.
1. Para o módulo de acionador, selecione o módulo Documento de download do Workfront.
1. Configure sua conexão com o Workfront e inclua a ID do documento copiada do URL do Workfront.
1. Nomeie este módulo como &quot;Obter arquivo de empresas&quot;.
1. Agora, adicione um módulo CSV de análise.
1. Para o campo Number of columns , digite 2.
1. Mapeie dados do módulo Baixar documento no campo CSV.
1. Nomeie este módulo como &quot;Arquivo de empresas de análise&quot;.
1. Salve o cenário e clique em Executar uma vez.

   **Crie um armazenamento de dados e uma estrutura de dados.**

1. Adicione um módulo de registros de Pesquisa do armazenamento de dados.
1. Crie um novo armazenamento de dados chamado &quot;Sincronização da empresa&quot;.
1. No armazenamento de dados, crie uma estrutura de dados chamada &quot;Company sync (struc)&quot;.
1. Crie quatro campos.

   + CID - A ID da empresa no arquivo CSV
   + Nome da empresa
   + WFID - A ID da empresa do Workfront
   + Data de criação - Certifique-se de que o tipo de dados é a data

   ![Armazenamento de dados Imagem 2](../12-exercises/assets/data-stores-walkthrough-2.png)

1. Clique em Salvar na estrutura de dados, defina o tamanho do armazenamento de dados como 1 e salve o armazenamento de dados.
1. Continuando no módulo do Data Store, configure um Filtro em que a CID seja igual à ID da empresa do módulo CSV de análise (Coluna 1).
1. Clique em Show advanced settings e selecione a opção para &quot;continuar a execução do cenário ou da rota, mesmo que esse módulo retorne sem resultados.&quot;

   ![Armazenamento de dados Imagem 3](../12-exercises/assets/data-stores-walkthrough-3.png)

1. Renomeie este módulo como &quot;Empresas correspondentes&quot;.
1. Adicione um módulo de registros Workfront Search.
1. Escolha Empresa como o tipo de registro.
1. O critério de pesquisa é o nome da empresa no Workfront que é igual ao nome da empresa no arquivo CSV.
1. Para saídas, selecione o nome da empresa e a ID.

   ![Armazenamento de dados Imagem 4](../12-exercises/assets/data-stores-walkthrough-4.png)

1. Clique em OK e renomeie este módulo como &quot;Empresas correspondentes&quot;.

   **Crie caminhos diferentes com base no fato de a empresa existir no Workfront ou no armazenamento de dados.**

   **Caminho de roteamento 1 - Criar uma empresa.**

1. Adicione um módulo de roteador à direita do módulo de registros do Workfront Search.
1. Adicione um módulo Criar registro do Workfront ao caminho superior.
1. Defina o tipo de registro como Empresa.
1. Selecione Nome em Campos a serem Mapeados. Mapeie o campo de nome para a saída do módulo CSV de análise (Coluna 2).
1. Renomeie este módulo como &quot;Criar empresa&quot;.

   ![Armazenamento de dados Imagem 5](../12-exercises/assets/data-stores-walkthrough-5.png)

1. Adicione um filtro após o roteador para criar uma empresa somente se ele ainda não estiver no Workfront. Nomeie de &quot;Não na Workfront&quot;.
1. Defina a condição para a ID do módulo Pesquisa do Workfront e não exista.

   ![Armazenamento de dados Imagem 6](../12-exercises/assets/data-stores-walkthrough-6.png)

   **Prepare-se para atualizar o armazenamento de dados no próximo caminho.**

1. Adicione um módulo Definir variável ao final do caminho superior.
1. Defina o nome da variável como &quot;Workfront ID&quot;.
1. Defina o valor Variable como a ID do módulo Create company .
1. Renomeie este módulo como &quot;Definir Workfront ID&quot;.

   **Caminho de roteamento 2 - Atualize o armazenamento de dados.**

1. Crie um filtro no caminho de roteamento 2. Nomeie de &quot;Não no armazenamento de dados&quot;.

1. Defina a Condição para a Chave no módulo do Armazenamento de dados e não exista.

   ![Armazenamento de dados Imagem 7](../12-exercises/assets/data-stores-walkthrough-7.png)

1. O primeiro módulo neste caminho é o módulo de variável Get.
1. Defina o nome da variável como &quot;Workfront ID&quot;.
1. Renomeie este módulo como &quot;Obter Workfront ID&quot;.
1. Adicione outro módulo do aplicativo da Data Store, Adicione/substitua um registro.
1. No campo Data store , escolha Company sync (Sincronização da empresa). Esse é o armazenamento de dados criado anteriormente.
1. Deixe o campo Key em branco.
1. Mapeie o campo CID da Coluna 1 no módulo CSV de análise.
1. Mapeie o campo de nome da empresa da Coluna 2 no módulo CSV de análise.
1. Mapeie o campo WFID do módulo Obter Workfront ID.
1. Para o campo Created date , use a função formatDate da guia Date and time para formatar a data atual como MM/DD/AAAA.

   ![Armazenamento de dados Imagem 8](../12-exercises/assets/data-stores-walkthrough-8.png)

1. Clique em OK e renomeie este módulo como &quot;Criar entrada de empresa&quot;.

   **Caminho de roteamento 3 - Sincronize o armazenamento de dados entre sistemas.**

1. Comece criando um filtro no caminho de roteamento 3. Nomeie como &quot;Empresa existe, não em armazenamento de dados&quot;.
1. Defina a Condição como a Chave no módulo de registros de Pesquisa do armazenamento de dados e não exista.
1. Clique no botão Adicionar e regra e designe que o nome da empresa no arquivo CSV (Coluna 2) é igual ao nome da empresa encontrada no módulo Pesquisa do Workfront.

   ![Armazenamento de dados Imagem 9](../12-exercises/assets/data-stores-walkthrough-9.png)

1. Agora, adicione outro módulo Adicionar/substituir um registro clonando o módulo no final do caminho de roteamento 2.
1. Arraste o módulo clonado para o local no final do caminho de roteamento 3. Exclua o módulo vazio que estava lá.
1. Clique no módulo clonado. Todos os campos devem permanecer os mesmos, exceto o campo WFID. Mapeie a partir do módulo Pesquisa de empresas correspondentes.

   ![Armazenamento de dados Imagem 10](../12-exercises/assets/data-stores-walkthrough-10.png)

1. Clique em OK e renomeie este módulo como &quot;Criar entrada de empresa&quot;.
