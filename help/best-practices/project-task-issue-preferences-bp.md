---
title: 'Prática recomendada: preferências de projetos, tarefas e problemas'
description: Explore as práticas recomendadas de especialistas do Adobe Workfront para configurar, gerenciar e usar preferências de projetos, tarefas e problemas no Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10918
exl-id: 321af897-3791-4b06-a9dd-241b5246b2a0
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 100%

---

# Prática recomendada: preferências de projetos, tarefas e problemas

## O que é uma “prática recomendada” do Adobe Workfront?

As práticas recomendadas são diretrizes para um curso de ação eficaz e eficiente; elas podem ser facilmente adotadas por qualquer usuário da empresa e replicadas com sucesso em toda a organização.

Ao revisar essas recomendações, lembre-se de que algumas práticas recomendadas do Workfront são universais, enquanto outras podem ser mais específicas para um determinado assunto. Use essas práticas recomendadas como uma base para orientar as configurações e o uso do sistema do Workfront.

## Navegar nesta página

Ao percorrer esta página, você encontrará primeiro uma lista resumida de todas as práticas recomendadas para o tópico. Isso permite revisar as recomendações sem se aprofundar nos detalhes e motivos por trás delas.

A seção “Por que essas práticas são recomendadas?” , encontrada após a lista resumida, fornece mais detalhes sobre algumas práticas recomendadas e por que elas são consideradas como um processo, ferramenta ou recurso que você deve considerar implementar na sua instância do Workfront.

</br>
</br>

## Práticas recomendadas para preferências de projetos, tarefas e problemas

* Defina o tipo de duração da tarefa padrão como “Simples”.

* Defina a preferência do status de um novo projeto como “Em planejamento” ou “Ideia”, não como “Atual”.

* Habilite “Criar linhas de base automaticamente” nas preferências globais do projeto.

* Verifique todas as opções na seção “Business Cases” das preferências do projeto no sistema.

* Nas preferências de problemas, marque a opção “Atualizar automaticamente o status de um problema resolvível” quando o status do objeto de resolução for alterado.

</br>
</br>


## Por que essas práticas são recomendadas?

**Prática recomendada**

Defina o tipo de duração da tarefa padrão como “Simples”.

**Entenda o porquê**

Os tipos de duração definem a relação entre a duração da tarefa, as horas planejadas e a quantidade de pessoas atribuídas à tarefa.

Com “Simples” como padrão global do sistema, todas as tarefas criadas manualmente possuem esse tipo de duração. As horas planejadas são divididas igualmente entre os destinatários da tarefa ao longo da duração. O tipo de duração “Simples” pode simplificar o planejamento do projeto, pois permite fazer alterações nos destinatários da tarefa e nas horas planejadas sem afetar a duração da tarefa, a data inicial planejada ou a data de conclusão planejada.

</br>
</br>

**Prática recomendada**

Defina a preferência do status de um novo projeto como “Em planejamento” ou “Ideia”, não como “Atual”.

**Entenda o porquê**

O status “Atual” indica que um projeto está ativo e o trabalho está sendo realizado ativamente. É raro que um projeto precise ter esse status no momento da criação. Mesmo se você usar um modelo de projeto, há algum “planejamento” envolvido na realização das atribuições de tarefas, no ajuste da data de conclusão planejada do projeto etc. O status “Em planejamento” também suprime notificações aos responsáveis pelas tarefas e aos membros da equipe do projeto. Receber notificações antes que o projeto esteja ativo pode ser confuso para os envolvidos.

</br>
</br>

**Prática recomendada**

Habilite “Criar linhas de base automaticamente” nas preferências globais do projeto.

**Entenda o porquê**

Cada vez que você altera o status de um projeto para “Atual”, o Workfront registra automaticamente uma linha de base do projeto. Esse “instantâneo” do projeto fornece informações históricas de como o plano do projeto mudou ao longo do tempo. Por exemplo, você pode comparar o plano original do projeto com o plano atual ao mostrar à liderança como a mudança de prioridades ou a redução do alcance afetaram os prazos do projeto.

</br>
</br>

**Prática recomendada**

Verifique todas as opções na seção “Business Cases” das preferências do projeto no sistema.

**Entenda o porquê**

Ative todas as cinco opções para permitir que gerentes de projetos, planejadores e outros incluam qualquer uma destas seções no Business Case de um projeto. Se as opções não estiverem habilitadas, elas não aparecerão na janela do Business Case. Os usuários poderão deixar qualquer um dos campos em branco se não forem necessários para o projeto em questão, mas não poderão habilitar um campo na camada do projeto. Essas opções só podem ser habilitadas globalmente em “Configuração”.

</br>
</br>

**Prática recomendada**

Nas preferências de problemas, marque a opção “Atualizar automaticamente o status de um problema resolvível” quando o status do objeto de resolução for alterado.

**Entenda o porquê**

Quando um problema é convertido em um projeto, essa configuração de preferência “vincula” os status dos dois itens. Atualizar o status do projeto (o objeto de resolução) atualizará automaticamente o status do problema. Isso significa que o solicitante pode ver o progresso que está sendo feito em sua solicitação, mesmo que não tenha permissões para ver todo o projeto no Workfront.
