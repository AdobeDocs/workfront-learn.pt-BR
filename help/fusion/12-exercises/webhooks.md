---
title: Webhooks
description: Saiba como criar, acionar e gerenciar cenários iniciados pelo webhook.
feature: Workfront Fusion
role: User
level: Beginner
kt: 11053
thumbnail: KT11053.png
source-git-commit: 1f7a4da813805691fc0e52d3ad1ea708f9e07a9a
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---


# Webhooks

Saiba como criar, acionar e gerenciar cenários iniciados pelo webhook.

## Visão geral do exercício

A finalidade deste cenário é criar um aplicativo para vender para lojas de conveniência para que possam determinar facilmente se um cliente é ou não velho o suficiente para comprar álcool. O caixa simplesmente precisa publicar o nome e a data de nascimento do cliente em um URL fornecido. Essa publicação acionará o cenário que calculará a resposta e a retornará ao solicitante.

1. O cenário consiste em três webhooks.
1. O módulo acionador é um webhook personalizado que escuta uma publicação.
1. Quando receber uma publicação, ela será emitida para um dos módulos seguintes.
1. O próximo módulo retorna uma resposta ao solicitante.

   ![Imagem do Webhooks 1](../12-exercises/assets/webhooks-walkthrough-1.png)

## Etapas a seguir

**Configure o webhook do acionador.**

1. Crie um novo cenário e o nomeie como &quot;Usando webhooks&quot;.
1. Para o acionador , adicione o módulo Webhook personalizado do aplicativo Webhooks.
1. Clique em Adicionar para criar um novo Webhook.
1. Insira o nome do Webhook de &quot;Aplicativo de página de bebida&quot;.
1. Deixe as restrições de IP em branco, o que significa que qualquer pessoa pode enviar dados para ele.
1. Clique em Salvar.


   ![Imagem 2 dos Webhooks](../12-exercises/assets/webhooks-walkthrough-2.png)

1. De volta ao painel de mapeamento Webhooks, um URL foi criado para este webhook específico. Clique em &quot;Copiar endereço para a área de transferência&quot; para copiar esse URL.
1. Clique em OK.
1. Clique em Executar uma vez.
1. Use o URL no Postman para enviar um nome e uma data de nascimento para seu webhook personalizado. Para obter instruções sobre como configurar o Postman, consulte o [Apresentação dos Webhooks](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/beyond-basic-modules/webhooks-walkthrough.html?lang=en) tutorial.

   **O painel do módulo Webhooks deve ter esta aparência:**

   ![Imagem do Webhooks 3](../12-exercises/assets/webhooks-walkthrough-3.png)

   **O webhook agora está em um estado em que está escutando dados para determinar a estrutura de dados.**

1. Você pode definir a estrutura de dados da carga que espera obter (as estruturas de dados serão discutidas posteriormente). Se você não definir uma estrutura de dados, o Fusion determinará a estrutura de dados automaticamente quando a publicação for enviada.
1. No lado do Postman, você deseja enviar para o URL copiado. A publicação deve incluir dados básicos de formulário. Neste exemplo, você precisa de três campos: Nome, Birthdate e clientToken.

   ![Imagem 4 dos Webhooks](../12-exercises/assets/webhooks-walkthrough-4.png)

1. Depois de clicar em Enviar do Postman , você deve obter uma indicação de que a publicação foi aceita.
1. Este é o ponto em que seu cenário mostrará que a estrutura de dados foi determinada com sucesso.
1. Você pode ver que os dados foram recebidos abrindo o inspetor de execução.

   ![Imagem de Webhooks 5](../12-exercises/assets/webhooks-walkthrough-5.png)

   **Configurar roteamento para tokens de cliente.**

1. Adicione um roteador ao módulo de acionador.
1. No caminho superior, adicione um módulo de resposta do Webhook. Esse será o nosso caminho para quando o token de cliente não corresponder.
1. Defina o status como 401.
1. Defina o Corpo como {&quot;erro&quot;: &quot;Falha ao autenticar solicitação. Verifique seu clientToken&quot;}.

   ![Imagem 6 dos Webhooks](../12-exercises/assets/webhooks-walkthrough-6.png)

1. Crie um filtro entre o roteador e o módulo de resposta do Webhook. Nomeie-o como &quot;O token do cliente não corresponde&quot;.
1. Para a Condição, use o campo clientToken do módulo de acionador e faça uma comparação numérica &quot;Not equal to&quot; com o número 5121933.

   ![Imagem de Webhooks 7](../12-exercises/assets/webhooks-walkthrough-7.png)

1. No caminho inferior, adicione outro módulo de resposta do Webhook. Esse será o nosso caminho para quando o token do cliente corresponder.
1. Defina o status como 200.
1. Ao configurar o Corpo, use as funções do painel de mapeamento para testar se a pessoa tem 21 anos ou mais. Se estiverem, retorne &quot;Você é velho o suficiente para beber!&quot;, caso contrário retorne &quot;Você está sem sorte...&quot;

   ![Imagem do Webhooks 9](../12-exercises/assets/webhooks-walkthrough-9.png)

1. Crie um filtro entre o roteador e o módulo de resposta do Webhook no caminho inferior. Nomeie-o como &quot;O token do cliente não corresponde&quot;.
1. Para a Condição, use o campo clientToken do módulo de acionador e faça uma comparação numérica &quot;Equal to&quot; com o número 5121933.


   ![Imagem do Webhooks 8](../12-exercises/assets/webhooks-walkthrough-8.png)

1. Clique no botão Agendamento em Executar uma vez para ativar seu cenário de forma que, a qualquer momento, uma nova publicação seja recebida, desça qualquer um dos caminhos e gere uma resposta.
