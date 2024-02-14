---
title: Exercício de armazenamento de dados
description: Aprenda a sincronizar nomes de empresas entre dois sistemas. (Deve ter entre 60 e 160 caracteres, mas tem 59 caracteres)
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11055
thumbnail: KT11055.png
recommendations: noDisplay,noCatalog
exl-id: e4aa9a97-679a-4575-a2c6-b6ac304ce9c2
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: tm+mt
source-wordcount: '904'
ht-degree: 99%

---

# Exercício de armazenamento de dados

Aprenda a sincronizar nomes de empresas entre dois sistemas.

## Visão geral do exercício

Esta é a primeira parte de uma sincronização unidirecional de empresas do Workfront e de outro sistema. Por enquanto, sincronizaremos apenas entre um armazenamento de dados do Fusion e o Workfront. Uma tabela em um armazenamento de dados monitora o ID do Workfront (WFID) e o ID da empresa no arquivo CSV (CID) de cada empresa. Isso permitirá uma sincronização bidirecional em algum momento no futuro.

![Armazenamentos de dados - Imagem 1](../12-exercises/assets/data-stores-walkthrough-1.png)

## Etapas a serem seguidas

**Baixe o arquivo do Workfront.**

1. Na pasta “Arquivos de exercícios do Fusion” do Workfront, selecione “_Companies.csv” e clique em “Detalhes do documento”.
1. Copie o primeiro número de ID do endereço URL.
1. No Fusion, crie um novo cenário chamado “Uso de armazenamentos de dados para sincronizar dados”.
1. Selecione o módulo acionador “Baixar documento do Workfront”.
1. Configure a sua conexão com o Workfront e inclua o ID do documento copiado do URL do Workfront.
1. Nomeie esse módulo como “Obter arquivo de empresas”.
1. Agora adicione um módulo “Analisar CSV”.
1. No campo “Número de colunas”, digite “2”.
1. Mapeie os dados do módulo “Baixar documento” no campo CSV.
1. Nomeie esse módulo como “Analisar arquivo de empresas”.
1. Salve o cenário e clique em Executar uma vez.

   **Crie um armazenamento de dados e uma estrutura de dados.**

1. Adicione um módulo “Pesquisar registros” no armazenamento de dados.
1. Crie um novo armazenamento de dados chamado “Sincronização de empresas”.
1. No armazenamento de dados, crie uma estrutura de dados chamada “Sincronização de empresas (estr.)”.
1. Crie quatro campos.

   + CID: o ID da empresa no arquivo CSV
   + Nome da empresa
   + WFID: o ID da empresa no Workfront
   + Data de criação: certifique-se de que o tipo de dados seja uma “data”

   ![Armazenamentos de dados - Imagem 2](../12-exercises/assets/data-stores-walkthrough-2.png)

1. Clique em “Salvar” na estrutura de dados, defina o tamanho do armazenamento de dados como “1” e salve-o.
1. A seguir, no módulo “Armazenamento de dados”, configure um filtro no qual o CID corresponda ao ID da empresa do módulo “Analisar CSV” (coluna 1).
1. Clique em “Mostrar configurações avançadas” e selecione a opção “Continuar a execução do cenário ou da rota mesmo que este módulo não retorne resultados”.

   ![Armazenamentos de dados - Imagem 3](../12-exercises/assets/data-stores-walkthrough-3.png)

1. Nomeie esse módulo como “Empresas correspondentes”.
1. Adicione um módulo “Pesquisar registros” do Workfront.
1. Escolha “Empresa” como o tipo de registro.
1. O critério de pesquisa exige que o nome da empresa no Workfront seja igual ao nome da empresa no arquivo CSV.
1. Para os resultados, selecione o nome da empresa e o ID.

   ![Armazenamentos de dados - Imagem 4](../12-exercises/assets/data-stores-walkthrough-4.png)

1. Clique em OK e nomeie esse módulo como “Empresas correspondentes”.

   **Crie caminhos diferentes dependendo de se a empresa se encontra no Workfront ou no armazenamento de dados.**

   **Caminho de roteamento 1: criar uma empresa.**

1. Adicione um módulo roteador à direita do módulo “Pesquisar registros” do Workfront.
1. Adicione um módulo “Criar registro do Workfront” no caminho superior.
1. Defina o tipo de registro como “Empresa”.
1. Selecione “Nome” em “Campos a serem mapeados”. Mapeie o campo de nome para a saída do módulo “Analisar CSV” (coluna 2).
1. Renomeie esse módulo como “Criar empresa”.

   ![Armazenamentos de dados - Imagem 5](../12-exercises/assets/data-stores-walkthrough-5.png)

1. Adicione um filtro após o roteador para criar uma empresa apenas se ela não existir no Workfront. Nomeie-o como “Não está no Workfront”.
1. Defina a condição como a ID do módulo de pesquisa do Workfront e como não existente.

   ![Armazenamentos de dados - Imagem 6](../12-exercises/assets/data-stores-walkthrough-6.png)

   **Prepare-se para atualizar o armazenamento de dados no próximo caminho.**

1. Adicione um módulo “Definir variável” no final do caminho superior.
1. Defina o nome da variável como “ID do Workfront”.
1. Defina o valor da variável como a ID do módulo “Criar empresa”.
1. Renomeie esse módulo como “Definir ID do Workfront”.

   **Caminho de roteamento 2: atualizar o armazenamento de dados.**

1. Crie um filtro no caminho de roteamento 2. Nomeie-o como “Não está no armazenamento de dados”.

1. Defina a condição como a chave do módulo de armazenamento de dados e como não existente.

   ![Armazenamentos de dados - Imagem 7](../12-exercises/assets/data-stores-walkthrough-7.png)

1. O primeiro módulo neste caminho é o módulo “Obter variável”.
1. Defina o nome da variável como “ID do Workfront”.
1. Renomeie esse módulo como “Obter ID do Workfront”.
1. Adicione outro módulo do aplicativo do armazenamento de dados e adicione ou substitua um registro.
1. No campo do armazenamento de dados, escolha “Sincronização de empresas”. Este é o armazenamento de dados criado anteriormente.
1. Deixe o campo “Chave” em branco.
1. Mapeie o campo CID da coluna 1 no módulo “Analisar CSV”.
1. Mapeie o campo de nome da empresa da coluna 2 no módulo “Analisar CSV”.
1. Mapeie o campo WFID do módulo “Obter ID do Workfront”.
1. No campo “Data de criação”, use a função formatDate da guia “Data e hora” para formatar a data atual como DD/MM/AAAA.

   ![Armazenamentos de dados - Imagem 8](../12-exercises/assets/data-stores-walkthrough-8.png)

1. Clique em OK e renomeie esse módulo como “Criar registro da empresa”.

   **Caminho de roteamento 3: sincronizar o armazenamento de dados entre sistemas.**

1. Comece criando um filtro no caminho de roteamento 3. Nomeie-o como “A empresa existe, mas não está no armazenamento de dados”.
1. Defina a condição como a chave do módulo “Pesquisar registros” do armazenamento de dados e como não existente.
1. Clique no botão “Adicionar regra E” e determine que o nome da empresa no arquivo CSV (coluna 2) seja igual ao nome da empresa encontrado no módulo de pesquisa do Workfront.

   ![Armazenamentos de dados - Imagem 9](../12-exercises/assets/data-stores-walkthrough-9.png)

1. Agora, adicione outro módulo “Adicionar ou substituir um registro”, clonando o módulo no final do caminho de roteamento 2.
1. Arraste o módulo clonado até o final do caminho de roteamento 3. Exclua o módulo em branco que estava lá.
1. Clique no módulo clonado. Todos os campos devem permanecer iguais, exceto o campo do WFID. Mapeie-o no módulo de pesquisa de empresas correspondentes.

   ![Armazenamentos de dados - Imagem 10](../12-exercises/assets/data-stores-walkthrough-10.png)

1. Clique em OK e renomeie esse módulo como “Criar registro da empresa”.
