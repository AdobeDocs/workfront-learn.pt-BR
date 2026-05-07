---
title: Introdução ao exercício para iteradores
description: Saiba como usar aplicativos de iteração e executar ações em cada pacote de informações.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11046
thumbnail: KT11046.png
recommendations: noDisplay,catalog
exl-id: 8d751885-372a-4716-9542-079cc3d36caf
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:42:51.955Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 390
ht-degree: 100%

---

# Introdução ao exercício para iteradores

Saiba como usar aplicativos de iteração e executar ações em cada pacote de informações.

## Visão geral do exercício

Observe um projeto específico no Workfront e, em seguida, analise todas as tarefas desse projeto. Você usará o módulo de ferramenta de incremento para contar o número de tarefas no projeto. Por fim, você usará o módulo Definir variável para subtrair o Número de tarefas derivadas do Número de problemas em aberto, a fim de produzir um valor numérico para cada um dos pacotes de tarefas.

![Introdução aos iteradores - Imagem 1](../12-exercises/assets/introduction-to-iterators-walkthrough-1.png)

## Etapas a serem seguidas

**Leia o projeto e as tarefas relacionadas.**

1. Crie um novo cenário. Nomeie-o como “Introdução à iteração”.
1. Escolha o Workfront como o módulo acionador para a leitura do registro.
1. Em Tipo de registro, escolha Projeto.
1. Em Saídas, escolha ID, Nome e Descrição.
1. No campo ID, insira a ID do projeto Northstar Fashion Exhibitors Booth da sua instância de teste do Workfront.
1. Renomeie este módulo como “Localizar projetos do WF”.
1. Adicione outro módulo do Workfront para ler as tarefas relacionadas a este projeto. Escolha o módulo Ler registros relacionados.
1. Em Tipo de registro, escolha Projeto.
1. Em ID do registro principal, escolha a ID do módulo Ler um registro.
1. Em Coleções, selecione Tarefas.
1. Em Saídas, selecione ID, Nome, Descrição, Número de tarefas derivadas, Número de problemas em aberto e Trabalho.
1. Renomeie este módulo como “Ler tarefas do projeto”.
1. Salve o cenário e clique em Executar uma vez para ver as saídas.

   + Clique no inspetor de execução e você verá um pacote de entrada (o projeto) e 28 pacotes de saída (as tarefas).

   **Contar e processar pacotes iterados.**

1. Adicione outro módulo além de Ler registros relacionados. Escolha um módulo de ferramentas com a função de incremento.

   + Defina o campo Redefinir um valor como Nunca e clique em OK.

1. Renomeie este módulo como “Contar o número de tarefas”.
1. Adicione um módulo Definir variável. Defina o nome da variável como “Matemática aleatória”.
1. No campo Valor da variável, subtraia o número de tarefas derivadas abertas do número de tarefas abertas.

   **Ele deve ter a seguinte aparência:**

   ![Introdução aos iteradores - Imagem 2](../12-exercises/assets/introduction-to-iterators-walkthrough-2.png)

1. Renomeie este módulo como “Matemática aleatória”.
1. Salve o cenário e clique em Executar uma vez.

Para cada uma das tarefas produzidas pelo módulo iterador Ler registros relacionados, o Workfront Fusion realizou 28 execuções. Esses 28 pacotes continuarão a ser processados durante todo o cenário, a menos que um agregador seja adicionado para fechar o loop.
