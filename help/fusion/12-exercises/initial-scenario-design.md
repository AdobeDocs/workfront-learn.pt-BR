---
title: Exercício de design do cenário inicial
description: Aprenda algumas dicas básicas de navegação para quando fizer seu primeiro logon no Workfront Fusion, bem como para construir seu primeiro cenário.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11038
thumbnail: KT11038.png
last-substantial-update: 2026-02-19T00:00:00Z
recommendations: noDisplay,catalog
exl-id: 8ecf4979-f291-4788-bdaa-ab5485fb0849
source-git-commit: 248683cd98cd123c4af9f34380a932deb714c62b
workflow-type: tm+mt
source-wordcount: '1181'
ht-degree: 77%

---

# Exercício de design do cenário inicial

Aprenda algumas dicas básicas de navegação para quando fizer seu primeiro logon no Workfront Fusion, bem como para construir seu primeiro cenário.

## Pré-requisitos

1. Este exercício requer um teste do Workfront. Você pode solicitar um preenchendo [este formulário](https://forms.office.com/r/f1J8HRGrNY). Caso não seja possível acessar o formulário, envie seu nome, endereço de email e o nome da empresa para wfttstdr@adobe.com.
1. Os exercícios do Fusion pressupõem que você tenha assistido aos vídeos explicativos correspondentes. Neste caso, o vídeo [Tutorial de design do cenário inicial](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/understand-the-basics/initial-scenario-design-walkthrough.html?lang=pt-BR).


## Visão geral do exercício

Crie um novo projeto no Workfront para cada linha no arquivo CSV da lista de projetos.

![Design do cenário inicial - Imagem 1](../12-exercises/assets/initial-scenario-design-1.png)

## Etapas a serem seguidas

1. Crie uma pasta na seção Cenário chamada “Exercícios de habilitação do Fusion”.
1. Clique na pasta e depois em Criar um novo cenário.

   ![Design do cenário inicial - Imagem 2](../12-exercises/assets/initial-scenario-design-2.png)

1. Na próxima página, pesquise por Workfront e selecione esse aplicativo. Em seguida, clique em Continuar.
1. Na parte superior esquerda da tela do designer de cenários, renomeie o cenário como &quot;Design de cenário inicial&quot;
1. Clique no módulo acionador vazio no centro da tela e selecione o aplicativo Workfront e, em seguida, selecione o módulo Baixar documento.

   **Autentique a conexão do módulo com sua conta do Workfront.**

1. Antes de se conectar a uma instância do Workfront, é necessário criar primeiro um conector OAuth 2.0 nessa instância do Workfront. Para fazer este logon na instância do Workfront, vá para **Configuração > Sistema > Aplicativos OAuth2** e clique em **Criar integração de aplicativos**.

Preencha a primeira página do formulário conforme mostrado abaixo e clique em **Criar**.

![Imagem de Design de Cenário Inicial 3a](../12-exercises/assets/initial-scenario-design-3a.png)

Quando a próxima tela for exibida, preencha o campo **Redirecionar URLs** com a seguinte URL:

`https://app.workfrontfusion.com/oauth/cb/workfront-workfront`

![Imagem de Design do Cenário Inicial 3b](../12-exercises/assets/initial-scenario-design-3b.png)

Em seguida, clique no botão **Adicionar segredo do cliente**. O segredo do cliente será exibido. Copie-a e salve-a em um local onde você possa recuperá-la para uma etapa futura. Você precisará dele no cenário do Fusion. Copie e salve também a **ID do cliente** para uma etapa futura. Quando terminar de copiar estes itens, clique em **Salvar** na parte inferior do aplicativo.

![Imagem de Design de Cenário Inicial 3c](../12-exercises/assets/initial-scenario-design-3c.png)

1. De volta ao Fusion, clique no botão **Adicionar** para criar uma conexão com o Workfront.

   ![Imagem de Design de Cenário Inicial 3d](../12-exercises/assets/initial-scenario-design-3d.png)

1. Selecione **Adobe Workfront auth** como o tipo de conexão e marque a caixa **Mostrar configurações avançadas**. Depois clique em **Continuar**.

   ![Imagem de Design de Cenário Inicial 4a](../12-exercises/assets/initial-scenario-design-4a.png)

1. Use a **ID do Cliente** e o **Segredo do Cliente** que você salvou anteriormente para preencher aqui. Para o **URL de Autenticação**, é mais fácil copiar o URL de Autenticação padrão fornecido abaixo do campo, substituir `oauth.my` por `<domain name>.testdrive` e clicar em **Continuar**.

   ![Imagem de Design do Cenário Inicial 5a](../12-exercises/assets/initial-scenario-design-5a.png)

1. Sua conexão deve estar sendo autenticada. Talvez seja necessário fazer logon no Workfront. Clique em **Permitir acesso**.

   ![Imagem de Design de Cenário Inicial 5b](../12-exercises/assets/initial-scenario-design-5b.png)

   **A conexão será estabelecida. Agora insira a ID do documento que deseja baixar do Workfront.**

   ![Design do cenário inicial - Imagem 7](../12-exercises/assets/initial-scenario-design-7.png)

1. Retorne ao Workfront. Na pasta “Arquivos de exercícios do Fusion”, selecione “_Fusion2020_Project List.csv” e clique em Detalhes do documento no painel esquerdo. Copie o número de ID do documento do endereço URL (esse é o primeiro número longo na URL).

   ![Design do cenário inicial - Imagem 8](../12-exercises/assets/initial-scenario-design-8.png)

1. Volte para o Fusion, cole o número no campo ID do documento e clique em OK.
1. A prática recomendada é renomear os módulos à medida que são criados. Clique com o botão direito no módulo Workfront e escolha Renomear. Nomeie o módulo como “Obter lista de projetos”.

   **Em seguida, você analisará o arquivo CSV que acabou de baixar para poder acessar cada linha do arquivo. Você usará essas informações ao criar um projeto a partir de cada linha.**

1. Clique no lado direito do módulo Workfront para adicionar outro módulo. Procure o aplicativo de CSV e selecione o módulo Analisar CSV.
1. Configure o módulo Analisar CSV para 6 colunas, defina o CSV para conter cabeçalhos, use um delimitador do tipo vírgula e insira Dados no campo CSV. Em seguida, clique em OK.

   ![Design do cenário inicial - Imagem 9](../12-exercises/assets/initial-scenario-design-9.png)

1. Renomeie este módulo como “Analisar lista de projetos”.
1. Na parte inferior do designer de cenário, clique para Salvar o cenário.
1. Clique em Executar uma vez para ver o resultado.

   >[!NOTE]
   >
   >Ignore o aviso de que um transformador não deve ser o último módulo (isso é verdade, mas não é importante para este teste). Clique em Executar assim mesmo.

   ![Design do cenário inicial - Imagem 10](../12-exercises/assets/initial-scenario-design-10.png)

1. Abra o inspetor de execução no módulo Analisar CSV para ver as entradas e saídas do módulo. Há um pacote (um arquivo CSV) como entrada e vários pacotes como saídas (um pacote para cada linha no arquivo CSV). A aparência deve ser semelhante a esta:

   ![Imagem 11 do design do cenário inicial](../12-exercises/assets/initial-scenario-design-11.png)

   **Adicione um módulo para criar um projeto para cada linha do arquivo CSV.**

1. Adicione outro módulo. Selecione o aplicativo Workfront e escolha o módulo Criar registro.
1. Defina o tipo de Registro como Projeto.

   >[!TIP]
   >
   >Pesquise-o começando a digitar algumas letras, como *proj*, para ir direto a ele.

1. Em seguida, use Cmd/Ctrl+G para encontrar o Nome (nome do projeto). Marque a caixa ao lado de Nome; o campo aparece abaixo.
1. Agora marque as caixas ao lado de Data inicial planejada e Prioridade.
1. Clique no campo Nome para que o painel de mapeamento apareça. Clique no campo Coluna 1 do módulo Analisar CSV para adicioná-lo ao campo Nome. Este é o nome do projeto do arquivo CSV.
1. Para a Data inicial planejada, clique na Coluna 5 do módulo Analisar CSV.
1. Para Prioridade, escolha Normal no menu suspenso.

   **Seu painel de mapeamento deve aparecer assim:**

   ![Imagem 12 do design do cenário inicial](../12-exercises/assets/initial-scenario-design-12.png)

1. Clique em OK.

   >[!NOTE]
   >
   >Se você não clicar em OK e acidentalmente clicar novamente no designer, seu trabalho não será salvo e será necessário mapear novamente.

1. Clique com o botão direito no módulo Workfront e renomeie-o como “Criar projetos do Workfront”.
1. Salve o cenário e clique no botão Executar uma vez.
1. Clique no inspetor de execução na parte superior direita do último módulo.

   + Você verá que foram realizadas 20 operações. Cada operação pegou um pacote, ou seja, uma linha, do arquivo CSV como entrada e teve como saída um pacote, que era um projeto criado no Workfront. A ID do projeto criado aparece com o pacote de saída.

   ![Imagem 13 do desgin do cenário inicial](../12-exercises/assets/initial-scenario-design-13.png)

   **Utilização de notas**

1. As notas ajudam a criar mais visibilidade no design do cenário. Para adicionar uma nota ao módulo Criar projetos do Workfront, clique com o botão direito do mouse e selecione Adicionar uma nota. À direita da janela do designer, surge um painel para que você possa adicionar uma nota ao módulo. Digite “Criar um projeto com nome, data inicial planejada e prioridade mapeadas a partir do arquivo CSV”.
1. Adicione outra nota para descrever o que o módulo acionador (o primeiro módulo do Workfront) está fazendo.
1. Feche o painel de notas clicando no X no canto superior direito.

   + Acesse as notas novamente clicando no botão de notas na barra de ferramentas inferior ou clicando com o botão direito do mouse em qualquer módulo e adicionando uma nova nota.
   + As notas são classificadas em ordem cronológica inversa.
   + Um ponto laranja aparece no botão Notas quando as notas são adicionadas.

   ![Imagem 14 do design do cenário inicial](../12-exercises/assets/initial-scenario-design-14.png)

1. Salve o cenário clicando no botão Salvar na barra de ferramentas de controles.
1. É possível visualizar os projetos criados na instância do Workfront.
