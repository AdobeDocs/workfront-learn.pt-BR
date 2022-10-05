---
title: Prática recomendada - Desempenho e manutenção do sistema
description: Explore as recomendações de práticas recomendadas dos especialistas da Adobe Workfront sobre o desempenho e a manutenção do sistema Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
kt: 10927
exl-id: c3f32975-96f4-4e62-8c3a-5b985b45bbbf
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 0%

---

# Prática recomendada - Desempenho e manutenção do sistema

## O que é uma &quot;prática recomendada&quot; do Adobe Workfront?

As melhores práticas são orientações que representam uma linha de ação eficaz e eficiente; sejam adotados facilmente por você e pelos usuários em sua empresa; e podem ser replicados com êxito em toda a organização.

À medida que você revisa essas recomendações, lembre-se de que algumas práticas recomendadas do Workfront são universais, enquanto outras podem ser mais específicas para o tópico. Use essas práticas recomendadas como estrutura para ajudar a orientar as configurações e o uso do sistema Workfront.

## Navegar nesta página

Ao rolar por essa página, primeiro você encontrará uma lista de alto nível de todas as práticas recomendadas para o tópico. Isso permite que você revise as recomendações sem entrar nos detalhes de &quot;por quê&quot;.

O &quot;Por que essas práticas recomendadas estão sendo usadas?&quot; , encontrada após a lista de alto nível, fornece mais detalhes sobre algumas práticas recomendadas e por que elas são consideradas como um processo, ferramenta etc., você deve considerar a implementação com sua instância do Workfront.

</br>
</br>

## Práticas recomendadas de manutenção e desempenho do sistema

* Analise as notas de versão do produto antes da data de lançamento.

* Crie diferentes tipos de relatórios de exceções que destacam dados e configurações ausentes ou incorretos.

* Crie um processo de desativação do usuário que inclua uma análise dos objetos que são de sua propriedade ou atribuídos a eles para que os usuários que não fazem mais parte da empresa não permaneçam ativos no sistema e criem confusão para outros usuários.

* Mantenha as configurações do fluxo de trabalho o mais simples possível para garantir que elas sejam escaláveis e possam ser mantidas na sua ausência.

* Use filtros em relatórios e listas de objetos para diminuir o número de linhas exibidas de uma vez e concentrar a equipe em informações importantes.

* Limpe regularmente o cache do navegador e os cookies para ajudar a melhorar o desempenho no Workfront.

* Comece a limpar o sistema nas principais áreas do Adobe Workfront que tendem a ser as mais desordenadas, como formulários, modelos, projetos e usuários personalizados.

* Saiba em qual cluster sua instância do Workfront está, para que você possa ver as atualizações, estar ciente das janelas de manutenção, etc.

* Mantenha os projetos curtos.

* Sempre que possível, mantenha os relatórios &quot;leves&quot; com poucos filtros sem complicações para melhorar o desempenho.

</br>
</br>

## Por que essas práticas recomendadas estão presentes?

**Prática recomendada**

Analise as notas de versão do produto antes da data de lançamento.



**Veja o porquê**

As notas de versão informam quais novos recursos e ferramentas estão chegando ao sistema Workfront. Ao revisar essas notas e reproduzir com a nova funcionalidade no ambiente Preview Sandbox, você tem a chance de aprender, praticar e resolver quaisquer erros com novas melhorias antes de serem liberados para produção.

</br>
</br>

**Prática recomendada**

Crie diferentes tipos de relatórios de exceções que destacam dados e configurações ausentes ou incorretos.



**Veja o porquê**

Esses relatórios incluem aqueles que informam quais usuários devem ser desativados, quais projetos mostram a porcentagem de conclusão de 100%, mas não estão marcados como concluídos, quais modelos nunca foram usados etc.



Coloque esses relatórios como estes e outros em um painel e dê a outros administradores de sistema e grupo acesso a esse painel para manter um sistema limpo em tempo hábil. Por exemplo, o Painel de limpeza do Workfront e o Painel de uso do Workfront incluem exemplos de relatório que você pode criar.



Para ajudar você a se lembrar de verificar esses relatórios, pelo menos trimestralmente, crie um projeto com tarefas trimestrais e atribua-os a você mesmo, além de administradores de sistema e grupo. Certifique-se de que essas tarefas tenham horas planejadas associadas para que os destinatários desses itens de trabalho possam alocar seu tempo corretamente.

</br>
</br>

**Prática recomendada**

Mantenha os projetos curtos.



**Veja o porquê**

Toda vez que você salva um projeto ou uma tarefa dentro do projeto, há um cálculo de linha do tempo em execução para atualizar todas as dependências. Dependendo do número de tarefas em seu projeto, o recálculo pode levar muito tempo para ser executado.
