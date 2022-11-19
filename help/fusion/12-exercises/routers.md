---
title: Roteadores
description: Entenda a importância dos roteadores e como eles podem ser usados para processar condicionalmente módulos diferentes.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11043
thumbnail: KT11043.png
exl-id: f2a60273-c19b-4423-b354-8cff0dd7bd6b
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 0%

---

# Roteadores

Entenda a importância dos roteadores e como eles podem ser usados para processar condicionalmente módulos diferentes.

## Visão geral do exercício

Use um roteador para passar Pokemon vs. super-heróis para baixo no caminho correto e crie uma tarefa para cada caractere.

![Imagem de Roteadores 1](../12-exercises/assets/routers-walkthrough-1.png)

## Etapas a seguir

1. Clona o cenário Uso de conectores universais do exercício anterior. Nomeie-o como &quot;Criando caminhos diferentes usando roteadores&quot;.

   **Crie um novo caminho para super-heróis clonando módulos e adicionando um roteador.**

   ![Imagem de Roteadores 2](../12-exercises/assets/routers-walkthrough-2.png)

1. Clique com o botão direito do mouse no módulo Obter informações do Pokemon e escolha Clonar. Depois de clonado, arraste-o e conecte-o à linha entre o novo módulo HTTP e o módulo CSV de análise.

   >[!NOTE]
   >
   > Observe como ele adiciona automaticamente um roteador com dois caminhos.

1. Nomeie este módulo como &quot;Obter aparência de super-herói&quot;.
1. Clonar este módulo, mover o clone para a direita, e nomeá-lo como &quot;Capturar habilidades de super-heróis&quot;.
1. Clona o módulo Ferramentas e mova-o para o final do segundo caminho.
1. Clique no ícone da varinha - o botão Alinhamento automático - na barra de ferramentas.

   **O cenário deve ser semelhante a:**

   ![Imagem de Roteadores 3](../12-exercises/assets/routers-walkthrough-3.png)

   **Em seguida, você alterará os valores mapeados nos novos módulos clonados.**

1. Ir para <https://www.superheroapi.com/> e use sua conta do Facebook para obter um token de acesso.

   >[!NOTE]
   >
   >Se tiver problemas para acessar seu próprio token de super-herói, você pode usar este token compartilhado: 10110256647253588. Considere quantas vezes você chama a API de super-herói para que esse token compartilhado continue a funcionar para todos.

1. Abra as configurações para a aparência de superherói Get e altere o URL para `https://www.superheroapi.com/api/[access- token]/332/appearance`. Certifique-se de incluir o token de acesso no URL. Clique em OK.
1. Abra as configurações para as habilidades do super-herói Get e altere o URL para `https://www.superheroapi.com/api/[access- token]/332/powerstats`. Certifique-se de incluir o token de acesso no URL. Clique em OK.
1. Clique com o botão direito do mouse em cada módulo de super-herói e selecione Executar este módulo somente. Isso gerará a estrutura de dados que você precisa ver para mapeamento.
1. Depois de executar os dois, altere o número &quot;332&quot; em cada campo de URL para a Coluna 4 mapeada do módulo CSV de análise.

   ![Imagem de Roteadores 4](../12-exercises/assets/routers-walkthrough-4.png)

   **Agora você pode clicar no módulo Definir várias variáveis no caminho do super-herói e atualizar o nome, a altura, o peso e as capacidades.**

1. Atualize os campos Nome e Capacidades do módulo Obter habilidades de super-heróis — Módulo 8.

   ![Imagem de Roteadores 5](../12-exercises/assets/routers-walkthrough-5.png)

1. Atualize os campos Altura e Peso do módulo Obter aparência de superherói — Módulo 6.

   ![Imagem de Roteadores 6](../12-exercises/assets/routers-walkthrough-6.png)

   **Quando terminar, suas variáveis devem ficar assim. Observe que os números de módulo são exibidos nos valores de campo.**

   ![Imagem de Roteadores 7](../12-exercises/assets/routers-walkthrough-7.png)

1. Clique em OK e salve seu cenário.

   **Crie outro caminho para criar uma tarefa por caractere.**

1. No Workfront, crie um projeto vazio. Nomeie-o como &quot;Projeto de manifesto de entrega&quot; e copie a ID do projeto do URL.
1. Retorne ao Workfront Fusion e clique no centro do roteador para criar outro caminho.

   ![Imagem de Roteadores 8](../12-exercises/assets/routers-walkthrough-8.png)

1. Clique no centro do módulo vazio que aparece e adicione um módulo de registro Create do aplicativo Workfront.
1. Defina o Tipo de registro como Tarefa e selecione ID do projeto na seção Campos para mapa .
1. Cole a ID do projeto copiada do Workfront no campo ID do projeto .
1. Agora, selecione o campo Nome na seção Campos a serem mapeados.
1. Nomeie a tarefa &quot;[Caractere] from [franquia],&quot; utilizando o nome do caractere e o nome da franquia do arquivo CSV. A coluna 3 é o nome do caractere e a coluna 2 é o nome da franquia.

   ![Imagem de Roteadores 9](../12-exercises/assets/routers-walkthrough-9.png)

1. Clique em OK e renomeie este módulo para &quot;Criar uma tarefa para cada caractere&quot;.

   **Adicione filtros para que o cenário possa ser executado sem erros. Você deseja que somente caracteres Pokemon abram o caminho superior, somente caracteres de super-herói para descer pelo caminho do meio, e todos os caracteres para descer pelo caminho inferior.**

1. Clique na linha pontilhada à esquerda do módulo de informações Get Pokemon para criar o primeiro filtro. Nomeie de &quot;caractere Pokemon&quot;.
1. Para a condição, permita apenas registros em que a franquia (Coluna 2) seja igual a &quot;Pokemon&quot;. Escolha o operador &quot;Equal to&quot; de texto.
1. Clique na linha pontilhada à esquerda do módulo Get superhero appearance para criar o próximo filtro. Nomeie-o como &quot;personagem de super-herói&quot;.
1. Como os super-heróis podem vir de várias franquias, use o campo ID de Superherói (Coluna 4) para determinar se um caractere é ou não um super-herói.

   **Seus filtros devem ter esta aparência:**

   ![Imagem de Roteadores 11](../12-exercises/assets/routers-walkthrough-11.png)

   ![Imagem de Roteadores 10](../12-exercises/assets/routers-walkthrough-10.png)

1. Salve o cenário e clique em Executar uma vez. Use os inspetores de execução para verificar se todas as operações foram bem-sucedidas e verificar as tarefas que foram criadas no seu projeto do Workfront.

   ![Imagem de Roteadores 12](../12-exercises/assets/routers-walkthrough-12.png)
