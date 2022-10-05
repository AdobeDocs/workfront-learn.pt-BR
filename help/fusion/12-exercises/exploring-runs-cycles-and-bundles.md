---
title: Explorar execuções, ciclos e pacotes
description: Entenda como execuções, ciclos e pacotes se comportam usando o histórico de execução de um cenário.
feature: Workfront Fusion
role: User
level: Beginner
kt: 11050
thumbnail: KT1101.png
source-git-commit: c348222464180e994e7b414d1b84e07f58b6b2ae
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---


# Explorar execuções, ciclos e pacotes

Entenda como execuções, ciclos e pacotes se comportam usando o histórico de execução de um cenário.

## Visão geral do exercício

Pratique com diferentes configurações de cenário para explorar o uso de execuções e ciclos.

![Explorar ciclos e pacotes Imagem 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)

## Etapas a seguir

1. Clona o cenário chamado &quot;Compartilhando variáveis entre caminhos de roteamento&quot;. Nomeie o novo cenário como &quot;Compartilhando variáveis entre caminhos de roteamento - Teste de ciclos&quot;.
1. Remova o módulo Enviar um email, pois ele não é necessário para esse teste.

   **Configure seu cenário para processar 3 ciclos por execução. Processar 5 projetos em cada ciclo.**

1. Clique no módulo de acionador e altere o campo Máximo para 5, para que apenas 5 projetos sejam processados em cada ciclo.
1. Nos critérios de Pesquisa, remova o segundo filtro que restringe a pesquisa a um único projeto.
1. Clique em OK.

1. Na barra de ferramentas Fusão, abra as Configurações de cenário e altere o campo Número máximo de ciclos de 1 para 3.
1. Clique em OK.

   ![Explorar ciclos e pacotes Imagem 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)


   **Programe o cenário para ser executado a cada minuto.**

1. Clique no ícone de relógio ao lado do módulo do acionador e altere o campo Minutes para 1 minuto.

   ![Explorar ciclos e pacotes Imagem 2](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-2.png)

1. Em seguida, alterne o botão Scheduling para On (Ativado), abaixo do botão Run once (Executar uma vez). Salve o cenário.

   ![Explorar ciclos e pacotes Imagem 3](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-3.png)

1. Vá para o Histórico de execução do cenário e observe como um novo registro de histórico aparece no próximo minuto. Talvez seja necessário atualizar a página.

   ![Explorar ciclos e pacotes Imagem 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-4.png)

1. Clique no botão Details de uma execução. Clique no log Simple no painel direito, semelhante ao que você fez na porção do histórico de execução do treinamento do Workfront Fusion.
1. Os registros das operações processadas são divididos em ciclos.

   ![Explorar ciclos e pacotes Imagem 5](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-5.png)

1. Um menu suspenso na parte superior direita da janela permite selecionar qualquer um dos três ciclos configurados para serem executados sempre.

   ![Explorar ciclos e pacotes Imagem 6](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-6.png)
