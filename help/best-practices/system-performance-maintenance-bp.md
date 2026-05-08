---
title: Prática recomendada - Desempenho e manutenção do sistema
description: Explore sugestões de práticas recomendadas dos especialistas do Adobe Workfront sobre desempenho e manutenção do sistema Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10927
exl-id: c3f32975-96f4-4e62-8c3a-5b985b45bbbf
TQID: https://experienceleague.adobe.com/2tq7aNHE96fep1EFCPrjcCo13t5lQ24A6c-ORDUmlpY
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 638
ht-degree: 93%

---

# Prática recomendada - Desempenho e manutenção do sistema

## O que é uma “prática recomendada” do Adobe Workfront?

As práticas recomendadas são diretrizes para um curso de ação eficaz e eficiente; elas podem ser facilmente adotadas por qualquer usuário da empresa e replicadas com sucesso em toda a organização.

Ao revisar essas recomendações, lembre-se de que algumas práticas recomendadas do Workfront são universais, enquanto outras podem ser mais específicas para um determinado assunto. Use essas práticas recomendadas como uma base para orientar as configurações e o uso do sistema do Workfront.

## Navegar nesta página

Ao percorrer esta página, você encontrará primeiro uma lista resumida de todas as práticas recomendadas para o tópico. Isso permite revisar as recomendações sem se aprofundar nos detalhes e motivos por trás delas.

A área &quot;Por que essas práticas recomendadas?&quot;, encontrada após a lista de alto nível, fornece mais detalhes sobre algumas das práticas recomendadas e por que elas são consideradas um processo, ferramenta etc., você deve considerar a implementação com sua instância do Workfront.

</br>
</br>

## Práticas recomendadas de desempenho e manutenção do sistema

* Revise as notas de versão do produto antes da data de lançamento.

* Crie diferentes tipos de relatórios de exceções que destacam dados e configurações ausentes ou incorretos.

* Crie um processo de desativação de usuários que inclua uma revisão dos objetos que pertencem ou que são atribuídos a eles, para que os usuários que não fazem mais parte da empresa não permaneçam ativos no sistema criando confusão para outros usuários.

* Mantenha as configurações de fluxo de trabalho o mais simples possível para garantir que sejam escaláveis e possam ser mantidas na sua ausência.

* Use filtros em relatórios e listas de objetos para diminuir o número de linhas exibidas de uma vez e concentrar a equipe em informações importantes.

* Limpe regularmente o cache e os cookies do navegador para ajudar a melhorar o desempenho do Workfront.

* Comece a limpar seu sistema nas principais áreas do Adobe Workfront que tendem a ficar mais desorganizadas, como formulários personalizados, modelos, projetos e usuários.

* Saiba em qual cluster sua instância do Workfront está para que você possa ficar atento a atualizações, a janelas de manutenção etc.

* Mantenha os projetos curtos.

* Sempre que possível, mantenha os relatórios “leves”, com poucos filtros e descomplicados para melhorar o desempenho.

</br>
</br>

## Por que essas práticas são recomendadas?

**Prática recomendada**

Revise as notas de versão do produto antes da data de lançamento.



**Entenda o porquê**

As notas de versão informam quais novas funcionalidades e ferramentas estão chegando ao sistema Workfront. Ao revisar essas notas e experimentar a nova funcionalidade no ambiente Sandbox de Pré-visualização, você tem a oportunidade de aprender, praticar e corrigir quaisquer erros com os novos aprimoramentos antes de serem lançados para produção.

</br>
</br>

**Prática recomendada**

Crie diferentes tipos de relatórios de exceções que destacam dados e configurações ausentes ou incorretos.



**Entenda o porquê**

Esses relatórios incluem aqueles que informam quais usuários devem ser desativados, quais projetos apresentam percentual de conclusão de 100%, mas não estão marcados como concluídos, quais modelos nunca foram usados etc.



Coloque relatórios como esses e outros em um painel e conceda acesso a outros administradores de sistema e de grupo a esse painel para manter um sistema limpo em tempo hábil. Por exemplo, o painel Limpeza do Workfront e o painel Uso do Workfront incluem exemplos de relatórios que você pode criar.



Para ajudar você a lembrar de verificar esses relatórios, pelo menos trimestralmente, crie um projeto com tarefas trimestrais e atribua-as a você mesmo e aos administradores de sistema e de grupo. Verifique se essas tarefas têm horas planejadas associadas para que os atribuídos desses itens de trabalho possam alocar seu tempo corretamente.

</br>
</br>

**Prática recomendada**

Mantenha os projetos curtos.



**Entenda o porquê**

Cada vez que você salva um projeto ou uma tarefa dentro do projeto, um cálculo de linha do tempo é executado para atualizar todas as dependências. Dependendo do número de tarefas no seu projeto, o recálculo pode demorar muito para ser executado.
