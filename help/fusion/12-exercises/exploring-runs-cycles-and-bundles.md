---
title: Explorar execuções, ciclos e pacotes
description: Entenda como execuções, ciclos e pacotes se comportam usando o histórico de execução de um cenário.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11050
thumbnail: KT1101.png
exl-id: f04c84b1-2a3c-418b-9db3-baa74cf364f3
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# Explorar execuções, ciclos e pacotes

Entenda como execuções, ciclos e pacotes se comportam usando o histórico de execução de um cenário.

## Visão geral do exercício

Pratique com diferentes configurações de cenário para explorar o uso de execuções e ciclos do.

![Explorando ciclos de execuções e pacotes Imagem 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)

## Etapas a serem seguidas

1. Clonar o cenário chamado &quot;Compartilhamento de variáveis entre caminhos de roteamento&quot;. Nomeie o novo cenário como &quot;Sharing variables between routing paths - Cycles test&quot; (Compartilhamento de variáveis entre caminhos de roteamento - Teste de ciclos).
1. Remova o módulo Enviar um email, pois ele não é necessário para esse teste.

   **Configure seu cenário para processar três ciclos por execução. Processe 5 projetos em cada ciclo.**

1. Clique no módulo Acionador e altere o campo Máximo para 5, para que apenas 5 projetos sejam processados em cada ciclo.
1. Nos critérios de Pesquisa, remova o segundo filtro que restringe a pesquisa a um único projeto.
1. Clique em OK.

1. Na barra de ferramentas do Fusion, abra as configurações de Cenário e altere o campo Número máximo de ciclos de 1 para 3.
1. Clique em OK.

   ![Explorando ciclos de execuções e pacotes Imagem 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)


   **Agende o cenário para ser executado a cada minuto.**

1. Clique no ícone do relógio ao lado do módulo de acionamento e altere o campo Minutos para 1 minuto.

   ![Explorar ciclos de execução e pacotes Imagem 2](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-2.png)

1. Em seguida, alterne a opção Scheduling (Agendamento) sob o botão Run once (Executar uma vez) para On (Ativado). Salve seu cenário.

   ![Explorando ciclos de execuções e pacotes Imagem 3](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-3.png)

1. Vá para o Histórico de execução do cenário e observe como um novo registro de histórico é exibido no próximo minuto. Talvez seja necessário atualizar a página.

   ![Explorando ciclos de execuções e pacotes Imagem 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-4.png)

1. Clique no botão Detalhes de uma execução. Clique no log Simples no painel direito, semelhante ao que você fez na parte do histórico de execução do treinamento do Workfront Fusion.
1. Os registros das operações processadas são divididos em ciclos.

   ![Explorando ciclos de execuções e pacotes Imagem 5](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-5.png)

1. Um menu suspenso na parte superior direita da janela permite selecionar qualquer um dos 3 ciclos configurados para serem executados todas as vezes.

   ![Explorando ciclos de execuções e pacotes Imagem 6](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-6.png)
