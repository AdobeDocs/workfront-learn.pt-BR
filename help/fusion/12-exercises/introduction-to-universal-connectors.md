---
title: Exercício de introdução a conectores universais
description: Amplie sua compreensão de trabalhar com conectores universais REST e com os dados retornados.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11042
thumbnail: KT11042.png
recommendations: noDisplay,noCatalog
exl-id: eb442c3e-26f3-44b7-9937-ed4eeba39fb1
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: ht
source-wordcount: '602'
ht-degree: 100%

---

# Exercício de introdução a conectores universais

Amplie sua compreensão de trabalhar com conectores universais REST e com os dados retornados.

## Visão geral do exercício

Usando um caractere Pokemon em uma planilha, chame a API Poke por meio de um conector HTTP para coletar e publicar mais informações sobre esse caractere.

![Introdução aos conectores universais Imagem 1](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-1.png)

## Etapas a serem seguidas

**Baixe o arquivo CSV do Workfront.**

1. Na pasta “Arquivos de exercício do Fusion” no Workfront, selecione “_Fusion2020_Shipping Manifest.csv” e clique em Detalhes do documento.
1. Copie o primeiro número de ID do endereço URL.
1. Crie um novo cenário no Workfront Fusion. Nomeie como “Utilização de conectores universais”.
1. Comece com o módulo Baixar documento do aplicativo Workfront.
1. Configure sua conexão com o Workfront e inclua a ID do documento copiada do URL do Workfront.
1. Renomeie esse módulo como “Baixar manifesto de envio”.

   ![Introdução aos conectores universais Imagem 9](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-9.png)

   **Analise os dados do manifesto de envio.**

1. Adicione outro módulo, selecionando Analisar CSV.
1. Configure Analisar CSV para 11 colunas. Marque a caixa CSV contém cabeçalhos. Escolha o tipo de delimitador como Vírgula e coloque os dados do módulo Baixar documento no campo CSV.

   ![Introdução aos conectores universais Imagem 2](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-2.png)

1. Renomeie este módulo como “Analisar manifesto de envio”.
1. Salve o cenário e clique em Executar uma vez para que você possa ver os dados do arquivo CSV nas próximas etapas.

   **Obtenha os dados de Pokemon usando o conector universal.**

1. Adicione um módulo HTTP Fazer uma solicitação.
1. No campo URL, use `https://pokeapi.co/api/v2/pokemon/[Character]`, onde [Caractere] é mapeado para a Coluna 3 do módulo Analisar CSV.
1. Marque a caixa de seleção Analisar resposta.
1. Selecione Mostrar configurações avançadas e marque a caixa ao lado de “Avaliar todos os estados como erros”.
1. Clique em OK e renomeie o módulo “Obter informações de Pokemon”.

   **Seu painel de mapeamento deve ter esta aparência:**

   ![Introdução aos conectores universais Imagem 3](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-3.png)

   **Nesta parte do exercício, você só deseja processar a linha 1 no arquivo CSV.**

1. Adicione um filtro antes do módulo Obter informações de Pokemon. Nomeie-o como “Somente a linha 1”.
1. Defina a condição para permitir apenas a passagem da ID número 1. A ID número 1 está na linha 1, e o campo ID está na Coluna 1 no arquivo CSV.

   ![Introdução aos conectores universais Imagem 4](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-4.png)

1. Salve o cenário.
1. Clique em Executar uma vez e observe a mensagem de erro que você recebe no módulo HTTP Fazer uma solicitação.

   >[!IMPORTANT]
   >
   >Observe no campo URL dos dados de entrada que o nome do caractere está em maiúscula. Isso não funcionará para fazer essa chamada de API porque os nomes dos caracteres precisam estar em minúsculas.

   ![Introdução aos conectores universais Imagem 5](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-5.png)

1. Use o painel de mapeamento no campo URL HTTP Fazer uma solicitação para deixar campo [Caractere] todo em minúsculas usando a função **minúscula**.

   ![Introdução aos conectores universais Imagem 6](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-6.png)

   **Mapeie as informações de volta da API usando o módulo Definir variáveis múltiplas.**

1. Adicione o módulo Definir variáveis múltiplas após Obter informações de Pokemon. Mapeie nome, altura, peso e habilidades.
1. Como o campo Habilidades é uma matriz, lembre-se de usar a função de mapa para acessar o nome de cada habilidade na matriz.

   ![Introdução aos conectores universais Imagem 7](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-7.png)

   **Execute o cenário sem o filtro para descobrir outro erro.**

1. Para processar todas as linhas no arquivo CSV, exclua o filtro chamado Somente linha 1:

   + Clique no ícone de filtro para editá-lo.
   + Exclua o rótulo do filtro.
   + Exclua a Condição.
   + Clique em OK.

1. Salve o cenário e clique em Executar uma vez.
1. Ocorre um erro no módulo Obter informações do Pokemon. Você vê que um caractere super-herói foi passado para a API Pokemon.

   >[!NOTE]
   >
   >Na apresentação dos Roteadores, você verá como resolver esse erro criando um caminho separado para processar super-heróis.

   ![Introdução aos conectores universais Imagem 8](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-8.png)
