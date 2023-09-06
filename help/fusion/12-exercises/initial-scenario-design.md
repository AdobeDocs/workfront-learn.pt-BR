---
title: Design do cenário inicial
description: Saiba mais sobre algumas dicas básicas de navegação para quando você faz logon pela primeira vez no Workfront Fusion, bem como a criação do primeiro cenário.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11038
thumbnail: KT11038.png
exl-id: 8ecf4979-f291-4788-bdaa-ab5485fb0849
source-git-commit: e639d3391ea6a8b46592dd18cf57b9eed50fbf8c
workflow-type: tm+mt
source-wordcount: '978'
ht-degree: 0%

---

# Design do cenário inicial

Saiba mais sobre algumas dicas básicas de navegação para quando você faz logon pela primeira vez no Workfront Fusion, bem como a criação do primeiro cenário.

## Pré-requisitos

1. Este exercício requer uma unidade de teste do Workfront. Você pode solicitar um preenchendo [este formulário](https://forms.office.com/r/f1J8HRGrNY). Caso não seja possível acessar o formulário, envie seu nome, endereço de email e nome da empresa para wfttstdr@adobe.com.
1. Exercícios de fusão presumem que você assistiu ao vídeo de apresentação que corresponde ao exercício. Nesse caso, é [Apresentação do design do cenário inicial](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/understand-the-basics/initial-scenario-design-walkthrough.html?lang=en).


## Visão geral do exercício

Crie um novo projeto no Workfront para cada linha no arquivo CSV da Lista de projetos.

![Imagem 1 do design do cenário inicial](../12-exercises/assets/initial-scenario-design-1.png)

## Etapas a serem seguidas

1. Crie uma pasta na seção Cenário chamada &quot;Exercícios de ativação do Fusion&quot;.
1. Clique em na pasta e em Criar um novo cenário.

   ![Imagem 2 do design do cenário inicial](../12-exercises/assets/initial-scenario-design-2.png)

1. Na próxima página, pesquise por Workfront e selecione esse aplicativo. Em seguida, clique em Continue.
1. Na parte superior esquerda da tela do designer de cenários, renomeie o cenário como &quot;Design de cenário inicial&quot;
1. Clique no módulo acionador vazio no centro da tela, selecione o aplicativo Workfront e o módulo Baixar documento.

   **Autentique a conexão do módulo com sua conta do Workfront.**

1. Para criar uma conexão pela primeira vez, clique no botão Add.

   ![Imagem 3 do design do cenário inicial](../12-exercises/assets/initial-scenario-design-3.png)

1. Nomeie a conexão, como &quot;My Workfront 2020&quot;

   ![Imagem 4 do design do cenário inicial](../12-exercises/assets/initial-scenario-design-4.png)

1. Insira o URL de **sua instância do Workfront** e, em seguida, clique em Next.

   ![Imagem 5 do design do cenário inicial](../12-exercises/assets/initial-scenario-design-5.png)

1. Digite sua senha e clique em Logon.

   **A conexão é estabelecida. Em seguida, insira a ID do documento que deseja baixar do Workfront.**

   ![Imagem 7 do design do cenário inicial](../12-exercises/assets/initial-scenario-design-7.png)

1. Volte para o Workfront. Na pasta &quot;Arquivos do Fusion Exercise&quot;, selecione &quot;_Fusion2020_Project List.csv&quot; e clique em Detalhes do Documento no painel esquerdo. Copie o número de ID do documento do endereço URL (esse é o primeiro número longo no URL).

   ![Imagem 8 do design do cenário inicial](../12-exercises/assets/initial-scenario-design-8.png)

1. Volte para o Fusion, cole o número no campo ID do documento e clique em OK.
1. A prática recomendada é renomear os módulos à medida que são criados. Clique com o botão direito do mouse no módulo Workfront e escolha Renomear. Nomeie o módulo como &quot;Obter lista de projetos&quot;.

   **Em seguida, você analisará o arquivo CSV que acabou de baixar para poder acessar cada linha no arquivo. Você usará essas informações ao criar um projeto a partir de cada linha.**

1. Clique no lado direito do módulo Workfront para adicionar outro módulo. Procure o aplicativo CSV e selecione o módulo Analisar CSV.
1. Configure o CSV de análise para 6 colunas, o CSV contém cabeçalhos, o tipo delimitador de vírgula e coloque os dados no campo CSV. Em seguida, clique em OK.

   ![Imagem 9 do design do cenário inicial](../12-exercises/assets/initial-scenario-design-9.png)

1. Renomeie este módulo como &quot;Lista de projetos de análise&quot;.
1. Na parte inferior do designer de cenário, clique em Salvar para salvar seu cenário.
1. Clique em Executar uma vez para exibir a saída.

   >[!NOTE]
   >
   >Ignore o aviso de que um transformador não deve ser o último módulo (isso é verdadeiro, mas não importa para este teste). Clique em Executar assim mesmo.

   ![Imagem 10 do projeto do cenário inicial](../12-exercises/assets/initial-scenario-design-10.png)

1. Abra o inspetor de execução no módulo Parse CSV para ver as entradas e saídas do módulo. Há um pacote (um arquivo CSV) como entrada e vários pacotes como saídas (um pacote para cada linha no arquivo CSV). Deve ser semelhante a:

   ![Imagem 11 do projeto do cenário inicial](../12-exercises/assets/initial-scenario-design-11.png)

   **Adicione um módulo para criar um projeto para cada linha no arquivo CSV.**

1. Adicione outro módulo. Selecione o aplicativo Workfront e escolha o módulo Criar registro.
1. Defina o Tipo de registro como Projeto.

   >[!TIP]
   >
   >Procure-o começando a digitar algumas letras, como *proj*, para ir diretamente para ele.

1. Em seguida, use Cmd/Ctrl+G para localizar Nome (nome do projeto). Marque a caixa ao lado de Nome; o campo aparece abaixo de.
1. Agora marque as caixas ao lado de Data de início planejada e Prioridade.
1. Clique no campo Nome para que o painel de mapeamento apareça. Clique no campo Coluna 1 do módulo Analisar CSV para adicioná-lo ao campo Nome. Este é o nome do projeto do arquivo CSV.
1. Para a Data de início planejada, clique na Coluna 5 do módulo Analisar CSV.
1. Em Prioridade, escolha Normal no menu suspenso.

   **Seu painel de mapeamento deve ter esta aparência:**

   ![Imagem 12 do projeto do cenário inicial](../12-exercises/assets/initial-scenario-design-12.png)

1. Clique em OK.

   >[!NOTE]
   >
   >Se você não clicar em OK e, acidentalmente, clicar novamente no designer, seu trabalho não será salvo e você terá que mapear novamente.

1. Clique com o botão direito do mouse no módulo Workfront e renomeie-o como &quot;Criar projetos Workfront&quot;.
1. Salve o cenário e clique no botão Executar uma vez.
1. Clique no inspetor de execução na parte superior direita do último módulo.

   + Você verá que 20 operações foram realizadas. Cada operação retirava um pacote, ou seja, uma linha, do arquivo CSV como entrada e saída e um pacote, que era um projeto criado no Workfront. A ID do projeto criado aparece com o pacote de saída.

   ![Imagem 13 do projeto do cenário inicial](../12-exercises/assets/initial-scenario-design-13.png)

   **Uso de notas**

1. As notas ajudam a criar mais visibilidade sobre o design do cenário. Para adicionar uma nota ao módulo Criar projetos Workfront, clique com o botão direito do mouse e selecione Adicionar uma nota. Um painel à direita da janela do designer aparece para que você possa adicionar uma nota ao módulo. Digite em &quot;Criar um projeto com o nome, a data de início planejada e a prioridade mapeada do arquivo CSV&quot;.
1. Adicione outra observação para descrever o que o módulo de acionamento (o primeiro módulo do Workfront) está fazendo.
1. Feche o painel &#39;Notas&#39; clicando no X no canto superior direito.

   + Acesse as notas novamente clicando no botão notas na barra de ferramentas inferior ou clicando com o botão direito do mouse em qualquer módulo e adicionando uma nova nota.
   + As notas são classificadas em ordem cronológica inversa.
   + Um ponto laranja é exibido no botão Notas quando as notas são adicionadas.

   ![Imagem 14 do projeto do cenário inicial](../12-exercises/assets/initial-scenario-design-14.png)

1. Salve o cenário clicando no botão Save na barra de ferramentas de controles.
1. É possível visualizar os projetos criados na instância do Workfront.
