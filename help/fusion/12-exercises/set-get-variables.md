---
title: Definir/obter variáveis
description: Saiba como usar os módulos Definir e Obter variável para usar os campos disponíveis em um caminho em um caminho diferente.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11045
thumbnail: KT11045.png
exl-id: 225f0090-0428-40e2-8a4b-9c6b18b205d2
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 0%

---

# Definir/obter variáveis

Saiba como usar os módulos Definir e Obter variável para usar os campos disponíveis em um caminho em um caminho diferente.

## Visão geral do exercício

Pesquise informações sobre um projeto no Workfront e envie um email com informações relacionadas.

![Definir Obter variáveis Imagem 1](../12-exercises/assets/set-get-variables-walkthrough-1.png)

## Etapas a serem seguidas

1. Crie um novo cenário e nomeie-o como &quot;Compartilhamento de variáveis entre caminhos de roteamento&quot;.
1. Para o acionador, selecione o módulo Pesquisa no aplicativo Workfront.

   + Defina o Tipo de registro como Projeto.
   + Para o Conjunto de resultados, escolha Todos os registros correspondentes.
   + Para os critérios de Pesquisa, defina-o como Status Igual a CUR.
   + Para Saídas, escolha ID, Nome, Descrição e ID do Patrocinador.

   ![Definir Obter variáveis Imagem 2](../12-exercises/assets/set-get-variables-walkthrough-2.png)

   ![Definir Obter variáveis Imagem 3](../12-exercises/assets/set-get-variables-walkthrough-3.png)

1. Clique em OK e renomeie este módulo como &quot;Localizar projetos atuais&quot;.
1. Adicione outro módulo e selecione o módulo Workfront Read a record.

   + Para o Tipo de Registro, escolha Usuário.
   + Para Saídas, escolha Nome.
   + Mapeie a ID do Patrocinador do módulo de Pesquisa para o campo de ID.

1. Clique em OK.
1. Renomeie o módulo como &quot;Localizar nome do patrocinador&quot;.

   ![Definir Obter variáveis Imagem 4](../12-exercises/assets/set-get-variables-walkthrough-4.png)

1. Salve o cenário e clique em Executar uma vez.

   Se você receber um erro no módulo Ler um registro, provavelmente será devido ao módulo Pesquisar encontrar um projeto sem um patrocinador listado.

   **Para evitar esse erro, crie dois caminhos: um para projetos com uma ID de patrocinador e outro para projetos que não têm.**

1. Adicione um roteador entre os dois módulos clicando na chave inglesa entre o roteador e o módulo Read a record. Configure um filtro chamado &quot;Patrocinador existe&quot; e defina a Condição para ID do Patrocinador existe.

   ![Definir Obter variáveis Imagem 5](../12-exercises/assets/set-get-variables-walkthrough-5.png)

1. Clique no roteador para criar outro caminho. Adicionar um Módulo Enviar um email do aplicativo Email.

   + Coloque seu próprio endereço de email no campo Para.
   + No campo Assunto, digite &quot;Informações atuais do projeto&quot;.
   + No campo Conteúdo, coloque o nome do projeto, a descrição e o patrocinador.
   + Não é possível obter a saída do nome do patrocinador do módulo Read a record. Você só pode acessar a ID do patrocinador do módulo de pesquisa antes do roteador. Você precisará encontrar uma maneira de acessar o nome do patrocinador a partir do outro caminho do roteador.

   ![Definir Obter variáveis Imagem 6](../12-exercises/assets/set-get-variables-walkthrough-6.png)

1. Clique em OK por enquanto e renomeie este módulo como &quot;Enviar informações do projeto&quot;

   **Use as variáveis Set/Get para compartilhar dados entre caminhos diferentes.**

1. Após o módulo Find sponsor name, adicione um módulo Set variable tool.

   + Coloque &quot;Sponsor name&quot; como o nome da variável.
   + Deixe a Variable lifetime em Um ciclo.
   + Mapeie o campo para a saída do nome do módulo de nome Localizar patrocinador.

1. Clique em OK e renomeie o módulo como &quot;Definir nome do Patrocinador&quot;.

   ![Definir Obter variáveis Imagem 7](../12-exercises/assets/set-get-variables-walkthrough-7.png)

1. Em seguida, clique com o botão direito do mouse entre o roteador e o módulo Send an email para adicionar um módulo de ferramenta Get variable. Insira &quot;Sponsor name&quot; no campo Variable name.
1. Clique em OK. Renomeie o módulo como &quot;Obter nome do Patrocinador&quot;.

   ![Definir Obter variáveis Imagem 8](../12-exercises/assets/set-get-variables-walkthrough-8.png)

1. Volte para o módulo Enviar um email e mapeie o valor do módulo Obter nome do patrocinador no campo de conteúdo. Clique em OK.

   ![Definir Obter variáveis Imagem 8](../12-exercises/assets/set-get-variables-walkthrough-8.png)

   >[!IMPORTANT]
   >
   >Antes de testar o cenário, recomendamos restringir o número de projetos processados para evitar uma enxurrada de emails.

1. Vá para a sua unidade de teste do Workfront e localize o projeto Northstar Fashion Exhibitors Booth. Este é um projeto atual que tem um patrocinador. Copie a ID do projeto do URL.

   ![Definir Obter variáveis Imagem 10](../12-exercises/assets/set-get-variables-walkthrough-10.png)

1. Em seu cenário, clique no módulo Localizar projetos atuais. Adicione outra condição aos critérios de pesquisa clicando no botão verde &quot;Adicionar regra AND&quot;. Especifique que a ID deve ser igual à ID do projeto copiada. Clique em OK.
1. Salve o cenário e clique em Executar uma vez.
1. Revise os inspetores de execução e o email que você recebe.

   ![Definir variáveis Get Imagem 11](../12-exercises/assets/set-get-variables-walkthrough-11.png)
