---
title: Exercício de exploração de execuções, ciclos e pacotes
description: Entenda o comportamento das execuções, ciclos e pacotes utilizando o histórico de execução de um cenário.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11050
thumbnail: KT1101.png
recommendations: noDisplay,noCatalog
exl-id: f04c84b1-2a3c-418b-9db3-baa74cf364f3
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: ht
source-wordcount: '342'
ht-degree: 100%

---

# Exercício de exploração de execuções, ciclos e pacotes

Entenda o comportamento das execuções, ciclos e pacotes utilizando o histórico de execução de um cenário.

## Visão geral do exercício

Pratique com diferentes configurações de cenário para explorar o uso de execuções e ciclos.

![Explorar execuções, ciclos e pacotes - Imagem 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)

## Etapas a serem seguidas

1. Clone o cenário chamado “Compartilhar variáveis entre caminhos de roteamento”. Nomeie o novo cenário como “Compartilhar variáveis entre caminhos de roteamento - Teste de ciclos”.
1. Remova o módulo Enviar um email, pois ele não é necessário para esse teste.

   **Configure seu cenário para processar 3 ciclos por execução. Processe 5 projetos em cada ciclo.**

1. Clique no módulo acionador e defina o campo Máximo como 5, para que apenas 5 projetos sejam processados em cada ciclo.
1. Nos critérios de pesquisa, remova o segundo filtro que restringe a pesquisa a um único projeto.
1. Clique em OK.

1. Na barra de ferramentas do Fusion, abra as configurações do cenário e altere o campo “Número máximo de ciclos” de 1 para 3.
1. Clique em OK.

   ![Explorar execuções, ciclos e pacotes - Imagem 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)


   **Programe o cenário para ser executado a cada minuto.**

1. Clique no ícone de relógio ao lado do módulo acionador e altere o campo Minutos para 1 minuto.

   ![Explorar execuções, ciclos e pacotes - Imagem 2](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-2.png)

1. Em seguida, ative o botão Cronograma (localizado abaixo do botão Executar uma vez). Salve seu cenário.

   ![Explorar execuções, ciclos e pacotes - Imagem 3](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-3.png)

1. Acesse o histórico de execução do cenário e observe como um novo registro aparecerá no histórico no minuto seguinte. Talvez seja necessário atualizar a página.

   ![Explorar execuções, ciclos e pacotes - Imagem 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-4.png)

1. Clique no botão Detalhes de uma execução. Clique nos registros simples do painel direito, semelhante ao que você fez na parte relacionada ao histórico de execução do treinamento do Workfront Fusion.
1. Os registros das operações processadas são divididos em ciclos.

   ![Explorar execuções, ciclos e pacotes - Imagem 5](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-5.png)

1. Um menu suspenso na parte superior direita da janela permite selecionar qualquer um dos 3 ciclos configurados para ser executado todas as vezes.

   ![Explorar execuções, ciclos e pacotes - Imagem 6](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-6.png)
