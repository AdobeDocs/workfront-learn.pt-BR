---
title: Armazenamentos de dados
description: Saiba como sincronizar nomes de empresa entre dois sistemas. (Deve ter entre 60 e 160 caracteres, mas tem 59 caracteres)
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11055
thumbnail: KT11055.png
exl-id: e4aa9a97-679a-4575-a2c6-b6ac304ce9c2
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 0%

---

# Armazenamentos de dados

Saiba como sincronizar nomes de empresa entre dois sistemas.

## Visão geral do exercício

Esta é a primeira parte de uma sincronização unidirecional de empresas no Workfront e em outro sistema. Por enquanto, só é sincronizado entre um armazenamento de dados do Fusion e o Workfront. Uma tabela em um armazenamento de dados rastreia a Workfront ID (WFID) e a ID da empresa no arquivo CSV (CID) de cada empresa. Isso permite uma sincronização bidirecional em algum ponto no futuro.

![Armazenamentos de dados Imagem 1](../12-exercises/assets/data-stores-walkthrough-1.png)

## Etapas a serem seguidas

**Baixe o arquivo do Workfront.**

1. Na pasta &quot;Arquivos de exercício de fusão&quot; do Workfront, selecione &quot;_Companies.csv&quot; e clique em Detalhes do documento.
1. Copie o primeiro número de ID do endereço do URL.
1. No Fusion, crie um novo cenário chamado &quot;Uso de armazenamentos de dados para sincronizar dados&quot;.
1. Para o módulo acionador, selecione o módulo Baixar documento do Workfront.
1. Configure sua conexão com o Workfront e inclua a ID do documento copiada do URL do Workfront.
1. Nomeie esse módulo como &quot;Obter arquivo de empresas&quot;.
1. Agora adicione um módulo Analisar CSV.
1. Para o campo Número de colunas, digite 2.
1. Mapeie os dados do módulo Baixar documento no campo CSV.
1. Nomeie esse módulo como &quot;Analisar arquivo de empresas&quot;.
1. Salve o cenário e clique em Executar uma vez.

   **Crie um armazenamento de dados e uma estrutura de dados.**

1. Adicione um módulo de armazenamento de dados Pesquisar registros.
1. Crie um novo armazenamento de dados chamado &quot;Sincronização da empresa&quot;.
1. No armazenamento de dados, crie uma estrutura de dados chamada &quot;Sincronização da empresa (estrutura)&quot;.
1. Crie quatro campos.

   + CID - A ID da empresa no arquivo CSV
   + Nome da empresa
   + WFID - A ID da empresa Workfront
   + Data de criação - Verifique se o tipo de dados é data

   ![Armazenamentos de dados Imagem 2](../12-exercises/assets/data-stores-walkthrough-2.png)

1. Clique em Salvar na estrutura de dados, defina o tamanho do armazenamento de dados como 1 e salve o armazenamento de dados.
1. Continuando no módulo Armazenamento de dados, configure um Filtro em que a CID seja igual à ID da empresa do módulo Analisar CSV (Coluna 1).
1. Clique em Show advanced settings e selecione a opção para &quot;continuar a execução do cenário ou da rota, mesmo se esse módulo retornar sem resultados&quot;.

   ![Armazenamento de dados Imagem 3](../12-exercises/assets/data-stores-walkthrough-3.png)

1. Renomeie este módulo como &quot;Empresas correspondentes&quot;.
1. Adicione um módulo Workfront Search records.
1. Escolha Empresa como o tipo de registro.
1. O critério de pesquisa é que o nome da empresa no Workfront é igual ao nome da empresa no arquivo CSV.
1. Para saídas, selecione o nome da empresa e a ID.

   ![Armazenamento de dados Imagem 4](../12-exercises/assets/data-stores-walkthrough-4.png)

1. Clique em OK e renomeie este módulo como &quot;Empresas correspondentes&quot;.

   **Crie caminhos diferentes com base no fato de a empresa existir na Workfront ou no armazenamento de dados.**

   **Caminho de roteamento 1 - Crie uma empresa.**

1. Adicione um módulo de roteador à direita do módulo Workfront Search records.
1. Adicione um módulo Criar registro do Workfront ao caminho superior.
1. Defina o tipo de registro como Empresa.
1. Selecione Nome em Campos para Mapear. Mapeie o campo de nome para a saída do módulo Analisar CSV (Coluna 2).
1. Renomeie este módulo como &quot;Criar empresa&quot;.

   ![Armazenamento de dados Imagem 5](../12-exercises/assets/data-stores-walkthrough-5.png)

1. Adicione um filtro depois do roteador para criar uma empresa apenas se ela ainda não estiver no Workfront. Nomeie de &quot;Não no Workfront&quot;.
1. Defina a Condição para a ID do módulo Workfront Search e não existe.

   ![Armazenamento de dados Imagem 6](../12-exercises/assets/data-stores-walkthrough-6.png)

   **Prepare-se para atualizar o armazenamento de dados no próximo caminho.**

1. Adicione um módulo Set variable ao final do caminho superior.
1. Defina o nome da variável como &quot;Workfront ID&quot;.
1. Defina o valor da Variável para a ID do módulo Criar empresa.
1. Renomeie esse módulo como &quot;Definir Workfront ID&quot;.

   **Caminho de roteamento 2 - atualize o armazenamento de dados.**

1. Crie um filtro no caminho de roteamento 2. Nomeie de &quot;Não está no armazenamento de dados&quot;.

1. Defina a Condição para a Chave do módulo de armazenamento de dados e não existe.

   ![Armazenamento de dados Imagem 7](../12-exercises/assets/data-stores-walkthrough-7.png)

1. O primeiro módulo neste caminho é o módulo Obter variável.
1. Defina o nome da variável como &quot;Workfront ID&quot;.
1. Renomeie este módulo como &quot;Obter Workfront ID&quot;.
1. Adicione outro módulo do aplicativo Data store, Adicione/substitua um registro.
1. No campo Data store, escolha Company sync. Este é o armazenamento de dados criado anteriormente.
1. Deixe o campo Chave em branco.
1. Mapeie o campo CID da Coluna 1 no módulo Analisar CSV.
1. Mapeie o campo de nome da empresa da Coluna 2 no módulo Analisar CSV.
1. Mapeie o campo WFID do módulo Obter Workfront ID.
1. Para o campo Data de criação, use a função formatDate da guia Data e hora para formatar a data atual como MM/DD/AAAA.

   ![Armazenamento de dados Imagem 8](../12-exercises/assets/data-stores-walkthrough-8.png)

1. Clique em OK e renomeie este módulo como &quot;Criar entrada da empresa&quot;.

   **Caminho de roteamento 3 - Sincronize o armazenamento de dados entre sistemas.**

1. Comece criando um filtro no caminho de roteamento 3. Nomeie-a como &quot;Empresa existe, não no armazenamento de dados&quot;.
1. Defina a Condição para a Chave no módulo de registros de Pesquisa do armazenamento de dados e ela não existe.
1. Clique no botão Adicionar regra AND e designe que o nome da empresa do arquivo CSV (Coluna 2) é igual ao nome da empresa encontrado no módulo Workfront Search.

   ![Armazenamento de dados Imagem 9](../12-exercises/assets/data-stores-walkthrough-9.png)

1. Agora, adicione outro módulo Adicionar/substituir um registro, clonando o módulo no final do caminho de roteamento 2.
1. Arraste o módulo clonado para o local no final do caminho de roteamento 3. Exclua o módulo vazio que estava lá.
1. Clique no módulo clonado. Todos os campos devem permanecer os mesmos, exceto o campo WFID. Mapeie-o a partir do módulo Pesquisa de empresas correspondentes.

   ![Armazenamento de dados Imagem 10](../12-exercises/assets/data-stores-walkthrough-10.png)

1. Clique em OK e renomeie este módulo como &quot;Criar entrada da empresa&quot;.
