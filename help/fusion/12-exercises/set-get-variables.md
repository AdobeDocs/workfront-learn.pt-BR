---
title: Exercício para definir/obter variáveis
description: Saiba como usar os módulos Definir e Obter variáveis para utilizar os campos de um caminho em um caminho diferente.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11045
thumbnail: KT11045.png
recommendations: noDisplay,catalog
exl-id: 225f0090-0428-40e2-8a4b-9c6b18b205d2
source-git-commit: f033b210268e8979ee15abe812e6ad85673eeedb
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Exercício para definir/obter variáveis

Saiba como usar os módulos Definir e Obter variáveis para utilizar os campos de um caminho em um caminho diferente.

## Visão geral do exercício

Pesquise informações sobre um projeto no Workfront e envie um email com informações relacionadas.

![Definir e obter variáveis - Imagem 1](../12-exercises/assets/set-get-variables-walkthrough-1.png)

## Etapas a serem seguidas

1. Crie um novo cenário e nomeie-o como “Compartilhamento de variáveis entre caminhos de roteamento”.
1. Para o acionador, selecione o módulo Pesquisa no aplicativo do Workfront.

   + Defina o tipo de registro como Projeto.
   + Ao definir os resultados, escolha Todos os registros correspondentes.
   + Em Critérios de pesquisa, defina como Status igual a CUR.
   + Em Saídas, escolha ID, Nome, Descrição e ID do patrocinador.

   ![Definir e obter variáveis - Imagem 2](../12-exercises/assets/set-get-variables-walkthrough-2.png)

   ![Definir e obter variáveis - Imagem 3](../12-exercises/assets/set-get-variables-walkthrough-3.png)

1. Clique em OK e renomeie este módulo como “Encontrar projetos atuais”.
1. Adicione outro módulo e selecione o módulo Ler um registro do Workfront.

   + Defina o tipo de registro como Usuário.
   + Em Saídas, escolha Nome.
   + Defina a ID do patrocinador no módulo Pesquisar como o campo ID.

1. Clique em OK.
1. Renomeie o módulo como “Encontrar nome do patrocinador”.

   ![Definir e obter variáveis - Imagem 4](../12-exercises/assets/set-get-variables-walkthrough-4.png)

1. Salve o cenário e clique em Executar uma vez.

   Se você receber um erro no módulo Ler um registro, é provável que o módulo Pesquisar tenha encontrado um projeto sem um patrocinador listado.

   **Para evitar esse erro, crie dois caminhos: um para projetos que possuem uma ID de patrocinador e outro para projetos que não possuem a ID.**

1. Adicione um roteador entre os dois módulos clicando no ícone de chave inglesa entre o roteador e o módulo Ler um registro. Configure um filtro chamado “O patrocinador existe” e defina a condição como ID do patrocinador existe.

   ![Definir e obter variáveis - Imagem 5](../12-exercises/assets/set-get-variables-walkthrough-5.png)

1. Clique no roteador para criar outro caminho. Adicione um módulo Enviar um email no aplicativo de email.

   + Insira seu endereço de email no campo Para.
   + No campo Assunto, digite “Informações atuais do projeto”.
   + No campo Conteúdo, insira o nome do projeto, a descrição e o patrocinador.
   + Não é possível coletar a saída do nome do patrocinador com o módulo Ler um registro. Você só pode acessar a ID do patrocinador no módulo de pesquisa anterior ao roteador. Você precisará encontrar uma maneira de acessar o nome do patrocinador a partir do outro caminho do roteador.

   ![Definir e obter variáveis - Imagem 6](../12-exercises/assets/set-get-variables-walkthrough-6.png)

1. Clique em OK por enquanto e renomeie este módulo como “Enviar informações do projeto”

   **Use os recursos Definir e Obter variáveis para compartilhar dados entre diferentes caminhos.**

1. Após o módulo Encontrar nome do patrocinador, adicione um módulo de ferramenta Definir variável.

   + Utilize “Nome do patrocinador” como o nome da variável.
   + Defina o tempo de vida da variável como Um ciclo.
   + Mapeie o campo para a saída de nome do módulo Encontrar nome do patrocinador.

1. Clique em OK e renomeie o módulo como “Definir nome do patrocinador”.

   ![Definir e obter variáveis - Imagem 7](../12-exercises/assets/set-get-variables-walkthrough-7.png)

1. Em seguida, clique com o botão direito entre o roteador e o módulo Enviar um email para adicionar um módulo de ferramenta Obter variável. Insira “Nome do patrocinador” no campo de nome da variável.
1. Clique em OK. Renomeie o módulo como “Obter nome do patrocinador”.

   ![Definir e obter variáveis - Imagem 8](../12-exercises/assets/set-get-variables-walkthrough-8.png)

1. Volte para o módulo Enviar um email e mapeie o valor do módulo Obter nome do patrocinador para o campo do conteúdo. Clique em OK.

   ![Definir e obter variáveis - Imagem 8](../12-exercises/assets/set-get-variables-walkthrough-8.png)

   >[!IMPORTANT]
   >
   >Antes de testar o cenário, recomendamos restringir o número de projetos processados para evitar uma enxurrada de emails.

1. Acesse a unidade de teste do Workfront e localize o projeto Northstar Fashion Exhibitors Booth. Este é um projeto atual que conta com um patrocinador. Copie a ID do projeto contida no URL.

   ![Definir e obter variáveis - Imagem 10](../12-exercises/assets/set-get-variables-walkthrough-10.png)

1. No seu cenário, clique no módulo Encontrar projetos atuais. Adicione outra condição aos critérios de pesquisa clicando no botão verde “Adicionar regra E”. Especifique que a ID deve ser igual à ID do projeto que você copiou. Clique em OK.
1. Salve o cenário e clique em Executar uma vez.
1. Revise os inspetores de execução e o email que você recebeu.

   ![Definir e obter variáveis - Imagem 11](../12-exercises/assets/set-get-variables-walkthrough-11.png)
