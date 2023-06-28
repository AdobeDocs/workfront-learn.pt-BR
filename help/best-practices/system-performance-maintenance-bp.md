---
title: Prática recomendada - Desempenho e manutenção do sistema
description: Explore as práticas recomendadas dos especialistas da Adobe Workfront sobre o desempenho e a manutenção do sistema Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10927
exl-id: c3f32975-96f4-4e62-8c3a-5b985b45bbbf
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 0%

---

# Prática recomendada - Desempenho e manutenção do sistema

## O que é uma &quot;prática recomendada&quot; do Adobe Workfront?

As práticas recomendadas são diretrizes que representam um curso de ação eficaz e eficiente; são facilmente adotadas por você e pelos usuários em sua empresa; e podem ser replicadas com sucesso em toda a organização.

Ao revisar essas recomendações, lembre-se de que algumas práticas recomendadas do Workfront são universais, enquanto outras podem ser mais específicas ao tópico. Use essas práticas recomendadas como uma estrutura para ajudar a orientar as configurações e o uso do sistema Workfront.

## Navegando nesta página

Ao percorrer essa página, primeiro você encontrará uma lista de alto nível de todas as práticas recomendadas para o tópico. Isso permite analisar as recomendações sem mergulhar nos detalhes do &quot;por quê&quot;.

O &quot;Por que essas práticas recomendadas?&quot; A área, localizada após a lista de alto nível, fornece mais detalhes sobre algumas das práticas recomendadas e por que elas são consideradas um processo, ferramenta, etc. Você deve considerar a implementação com sua instância do Workfront.

</br>
</br>

## Práticas recomendadas de desempenho e manutenção do sistema

* Revise as notas de versão do produto antes da data de lançamento.

* Crie diferentes tipos de relatórios de exceções que destacam dados e configurações ausentes ou incorretos.

* Crie um processo de desativação de usuário que inclua uma revisão dos objetos que são de sua propriedade ou que estão atribuídos a eles, para que os usuários que não fazem mais parte da empresa não permaneçam ativos no sistema e gerem confusão para outros usuários.

* Mantenha as configurações de fluxo de trabalho o mais simples possível para garantir que sejam escaláveis e possam ser mantidas em sua ausência.

* Use filtros em relatórios e listas de objetos para diminuir o número de linhas exibidas de uma vez e concentrar a equipe em informações importantes.

* Limpe regularmente o cache do navegador e os cookies para ajudar a melhorar o desempenho no Workfront.

* Comece a limpar seu sistema nas principais áreas do Adobe Workfront que tendem a ser as mais poluídas, como formulários personalizados, modelos, projetos e usuários.

* Saiba em qual cluster está sua instância do Workfront para que você possa assistir a atualizações, estar ciente das janelas de manutenção etc.

* Mantenha os projetos curtos.

* Sempre que possível, mantenha os relatórios &quot;leves&quot; com pouquíssimos filtros simples para melhorar o desempenho.

</br>
</br>

## Por que essas práticas recomendadas?

**Prática recomendada**

Revise as notas de versão do produto antes da data de lançamento.



**Veja o porquê**

As notas de versão informam quais novas funcionalidades e ferramentas estão chegando ao sistema do Workfront. Ao revisar essas notas e aproveitar a nova funcionalidade no ambiente Pré-visualização de sandbox, você tem a chance de aprender sobre, praticar e resolver bugs com novos aprimoramentos antes que sejam lançados para produção.

</br>
</br>

**Prática recomendada**

Crie diferentes tipos de relatórios de exceções que destacam dados e configurações ausentes ou incorretos.



**Veja o porquê**

Esses relatórios incluem aqueles que informam quais usuários devem ser desativados, quais projetos mostram uma porcentagem de conclusão de 100%, mas não estão marcados como concluídos, quais modelos nunca foram usados etc.



Coloque esses relatórios como estes e outros em um painel e dê a outros administradores de sistema e grupo acesso a esse painel para manter um sistema limpo em tempo hábil. Por exemplo, o Painel de limpeza do Workfront e o Painel de uso do Workfront incluem exemplos de relatório que você pode criar.



Para ajudá-lo a se lembrar de verificar esses relatórios, pelo menos trimestralmente, crie um projeto com tarefas trimestrais e atribua-as a si mesmo e a administradores de sistema e de grupo. Verifique se essas tarefas têm horas planejadas associadas para que os atribuídos desses itens de trabalho possam alocar seu tempo corretamente.

</br>
</br>

**Prática recomendada**

Mantenha os projetos curtos.



**Veja o porquê**

Toda vez que você salva um projeto, ou uma tarefa dentro do projeto, há um cálculo de linha do tempo em execução para atualizar todas as dependências. Dependendo do número de tarefas em seu projeto, o recálculo pode levar muito tempo para ser executado.
