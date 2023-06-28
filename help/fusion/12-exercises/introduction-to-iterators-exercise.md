---
title: Introdução ao exercício de iteradores
description: Saiba como usar aplicativos do tipo iteração e executar ações em cada pacote de informações.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11046
thumbnail: KT11046.png
exl-id: 8d751885-372a-4716-9542-079cc3d36caf
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# Introdução aos iteradores

Saiba como usar aplicativos do tipo iteração e executar ações em cada pacote de informações.

## Visão geral do exercício

Examine um projeto específico no Workfront e todas as tarefas nesse projeto. Você usará o módulo de ferramenta de incremento para contar o número de tarefas no projeto. Finalmente, você usará o módulo Set variable para subtrair o Número de Filhos do Número de Problemas Abertos para produzir um valor numérico para cada um dos conjuntos de tarefas.

![Introdução aos iteradores Imagem 1](../12-exercises/assets/introduction-to-iterators-walkthrough-1.png)

## Etapas a serem seguidas

**Leia um projeto e tarefas relacionadas.**

1. Inicie um novo cenário. Nomeie-o como &quot;Introdução à iteração&quot;.
1. Escolha Workfront como módulo acionador e Leia um registro.
1. Para Tipo de Registro, escolha Projeto.
1. Para Saídas, escolha ID, Nome e Descrição.
1. No campo ID, coloque a ID do projeto Northstar Fashion Exhibitors Booth da sua instância da unidade de teste Workfront.
1. Renomeie este módulo como &quot;Localizar projetos do WF&quot;.
1. Adicione outro módulo Workfront para ler as tarefas relacionadas a este projeto. Escolha o módulo Ler registros relacionados.
1. Para Tipo de Registro, escolha Projeto.
1. Para o ID do Registro pai, escolha o ID no módulo Ler um registro.
1. Para Coleções, selecione Tarefas.
1. Para Saídas, selecione ID, Nome, Descrição, Número de Filhos, Número de Problemas Abertos e Trabalho.
1. Renomeie este módulo como &quot;Ler tarefas do projeto&quot;.
1. Salve o cenário e clique em Executar uma vez para ver as saídas.

   + Clique no inspetor de execução e você verá um pacote como entrada (o projeto) e 28 pacotes como saída (as tarefas).

   **Contar e processar pacotes iterados.**

1. Adicione outro módulo após Read Related Records (Ler registros relacionados). Escolha um módulo de ferramentas da função Incremento.

   + Deixe o campo Redefinir um valor como Nunca e clique em OK.

1. Renomeie esse módulo como &quot;Count the # of tasks&quot;.
1. Adicione um módulo Set variable. Defina o nome da variável como &quot;Random Math&quot;.
1. No campo Variable value, subtraia o número de filhos abertos do número de opTasks abertas.

   **Deve ter esta aparência:**

   ![Introdução aos iteradores Imagem 2](../12-exercises/assets/introduction-to-iterators-walkthrough-2.png)

1. Renomeie este módulo como &quot;Matemática aleatória&quot;.
1. Salve o cenário e clique em Executar uma vez.

Para cada uma das tarefas produzidas pelo módulo do iterador de Registros Relacionados de Leitura, o Workfront Fusion executou 28 execuções. Esses 28 pacotes continuarão a ser processados durante todo o cenário, a menos que um agregador seja adicionado para fechar o loop.
