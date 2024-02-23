---
title: Exercício de roteadores
description: Entenda a importância dos roteadores e como eles podem ser usados para processar diferentes módulos condicionalmente.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11043
thumbnail: KT11043.png
recommendations: noDisplay,noCatalog
exl-id: f2a60273-c19b-4423-b354-8cff0dd7bd6b
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: ht
source-wordcount: '755'
ht-degree: 100%

---

# Exercício de roteadores

Entenda a importância dos roteadores e como eles podem ser usados para processar diferentes módulos condicionalmente.

## Visão geral do exercício

Use um roteador para transferir pacotes de “Pokémon vs. super-heróis” pelo caminho correto e, em seguida, crie uma tarefa para cada personagem.

![Roteadores - Imagem 1](../12-exercises/assets/routers-walkthrough-1.png)

## Etapas a serem seguidas

1. Clone o cenário “Uso de conectores universais” do exercício anterior. Nomeie-o como “Criar caminhos diferentes usando roteadores”.

   **Crie um novo caminho para os super-heróis, clonando módulos e adicionando um roteador.**

   ![Roteadores - Imagem 2](../12-exercises/assets/routers-walkthrough-2.png)

1. Clique com o botão direito no módulo “Obter informações do Pokémon” e escolha “Clonar”. Depois de clonado, arraste e conecte-o à linha entre o novo módulo HTTP e o módulo Analisar CSV.

   >[!NOTE]
   >
   > Observe que ele automaticamente adiciona um roteador com dois caminhos.

1. Nomeie esse módulo como “Obter aparência do super-herói”.
1. Clone esse módulo, mova o clone para a direita e nomeie-o como “Obter habilidades do super-herói”.
1. Clone o módulo “Ferramentas” e mova-o para o fim do segundo caminho.
1. Clique no ícone de varinha (o botão de alinhamento automático) na barra de ferramentas.

   **O seu cenário deve ter esta aparência:**

   ![Roteadores - Imagem 3](../12-exercises/assets/routers-walkthrough-3.png)

   **Em seguida, você alterará os valores mapeados nos novos módulos clonados.**

1. Acesse <https://www.superheroapi.com/> e use a sua conta do Facebook para obter um token de acesso.

   >[!NOTE]
   >
   >Se tiver problemas para acessar o seu próprio token de super-herói, você pode usar este token compartilhado: 10110256647253588. Leve em consideração quantas vezes você chama o “Superhero API”, para que esse token compartilhado continue funcionando para todos.

1. Abra as configurações “Obter aparência do super-herói” e altere o URL para `https://www.superheroapi.com/api/[access- token]/332/appearance`. Certifique-se de incluir o seu token de acesso no URL. Clique em OK.
1. Abra as configurações “Obter habilidades do super-herói” e altere o URL para `https://www.superheroapi.com/api/[access- token]/332/powerstats`. Certifique-se de incluir o seu token de acesso no URL. Clique em OK.
1. Clique com o botão direito em cada módulo de super-herói e selecione “Executar apenas este módulo”. Isso gerará a estrutura de dados que você precisa ver para o mapeamento.
1. Depois de executar ambos, altere o número “332” em cada campo de URL para a coluna 4 mapeada no módulo Analisar CSV.

   ![Roteadores - Imagem 4](../12-exercises/assets/routers-walkthrough-4.png)

   **Agora, clique no módulo “Definir múltiplas variáveis” no caminho do super-herói e atualize o nome, a altura, o peso e as habilidades.**

1. Atualize os campos de nome e habilidades do módulo 8: “Obter habilidades do super-herói”.

   ![Roteadores - Imagem 5](../12-exercises/assets/routers-walkthrough-5.png)

1. Atualize os campos de altura e peso do módulo 6: “Obter aparência do super-herói”.

   ![Roteadores - Imagem 6](../12-exercises/assets/routers-walkthrough-6.png)

   **Quando terminar, as suas variáveis deverão ter essa aparência. Observe que os números do módulo aparecem nos valores dos campos.**

   ![Roteadores - Imagem 7](../12-exercises/assets/routers-walkthrough-7.png)

1. Clique em OK e salve o cenário.

   **Crie outro caminho para gerar uma tarefa por personagem.**

1. No Workfront, crie um projeto vazio. Chame-o de “Projeto de manifesto de transporte” e copie a ID do projeto contida no URL.
1. Retorne ao Workfront Fusion e clique no centro do roteador para criar outro caminho.

   ![Roteadores - Imagem 8](../12-exercises/assets/routers-walkthrough-8.png)

1. Clique no centro do módulo vazio exibido e adicione um módulo “Criar registro” do aplicativo do Workfront.
1. Defina o tipo de registro como “Tarefa” e selecione “ID do projeto” na seção “Campos a mapear”.
1. Cole a ID do projeto copiada do Workfront no campo de ID do projeto.
1. Agora, selecione o campo “Nome” na seção “Campos a mapear”.
1. Nomeie a tarefa como “[Personagem] da [série]” e utilize o nome do personagem e o nome da série coletados do arquivo CSV. A coluna 3 é o nome do personagem e a coluna 2 é o nome da série.

   ![Roteadores - Imagem 9](../12-exercises/assets/routers-walkthrough-9.png)

1. Clique em OK e renomeie este módulo como “Criar uma tarefa para cada personagem”.

   **Adicione filtros para que o cenário possa ser executado sem erros. É recomendado enviar apenas personagens de Pokémon pelo caminho superior, apenas personagens super-heróis pelo caminho central e que todos os personagens percorram o caminho inferior.**

1. Clique na linha pontilhada à esquerda do módulo “Obter informações do Pokémon” para criar o primeiro filtro. Nomeie-o como “Personagem de Pokémon”.
1. Para a condição, permita apenas registros onde a série (Coluna 2) corresponda a “Pokémon”. Escolha o operador “Igual a”.
1. Clique na linha pontilhada à esquerda do módulo “Obter aparência do super-herói” para criar o próximo filtro. Nomeie-o como “Personagem super-herói”.
1. Como os super-heróis podem vir de várias séries, use o campo ID do super-herói (Coluna 4) para determinar se um personagem é um super-herói ou não.

   **Os filtros devem ter esta aparência:**

   ![Roteadores - Imagem 11](../12-exercises/assets/routers-walkthrough-11.png)

   ![Roteadores - Imagem 10](../12-exercises/assets/routers-walkthrough-10.png)

1. Salve o cenário e clique em Executar uma vez. Use os inspetores de execução para verificar se todas as operações foram bem-sucedidas e verifique as tarefas que foram criadas no seu projeto do Workfront.

   ![Roteadores - Imagem 12](../12-exercises/assets/routers-walkthrough-12.png)
