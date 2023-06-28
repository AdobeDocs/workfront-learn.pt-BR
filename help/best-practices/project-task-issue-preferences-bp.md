---
title: Prática recomendada - Preferências de projeto, tarefa e problema
description: Explore as recomendações de práticas recomendadas dos especialistas da Adobe Workfront sobre como configurar, gerenciar e usar as preferências de projeto, tarefa e problema do Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10918
exl-id: 321af897-3791-4b06-a9dd-241b5246b2a0
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 0%

---

# Prática recomendada - Preferências de projeto, tarefa e problema

## O que é uma &quot;prática recomendada&quot; do Adobe Workfront?

As práticas recomendadas são diretrizes que representam um curso de ação eficaz e eficiente; são facilmente adotadas por você e pelos usuários em sua empresa; e podem ser replicadas com sucesso em toda a organização.

Ao revisar essas recomendações, lembre-se de que algumas práticas recomendadas do Workfront são universais, enquanto outras podem ser mais específicas ao tópico. Use essas práticas recomendadas como uma estrutura para ajudar a orientar as configurações e o uso do sistema Workfront.

## Navegando nesta página

Ao percorrer essa página, primeiro você encontrará uma lista de alto nível de todas as práticas recomendadas para o tópico. Isso permite analisar as recomendações sem mergulhar nos detalhes do &quot;por quê&quot;.

O &quot;Por que essas práticas recomendadas?&quot; A área, localizada após a lista de alto nível, fornece mais detalhes sobre algumas das práticas recomendadas e por que elas são consideradas um processo, ferramenta, etc. Você deve considerar a implementação com sua instância do Workfront.

</br>
</br>

## Práticas recomendadas para preferências de projetos, tarefas e problemas

* Defina o tipo de duração padrão da tarefa como Simple.

* Defina a preferência do status de um novo projeto como Planejamento ou Ideia, Não Atual.

* Habilite Criar linhas de base Automaticamente nas preferências do projeto global.

* Marque todas as opções na seção Business Cases das preferências do projeto do sistema.

* Nas preferências de problemas, marque a opção Atualizar automaticamente o status de um problema resolvível quando o status do objeto de resolução for alterado.

</br>
</br>


## Por que essas práticas recomendadas?

**Prática recomendada**

Defina o tipo de duração padrão da tarefa como Simple.

**Veja o porquê**

Os tipos de duração definem a relação entre a duração da tarefa, as horas planejadas e o número de pessoas atribuídas à tarefa.

Com Simples como padrão do sistema global, todas as tarefas criadas manualmente têm esse tipo de duração. As horas planejadas são divididas uniformemente entre os atribuídos da tarefa na duração. O tipo de duração Simples pode simplificar o planejamento do projeto, pois permite fazer alterações nos designados da tarefa e nas horas planejadas sem afetar a duração da tarefa, a data de início planejada ou a data de conclusão planejada.

</br>
</br>

**Prática recomendada**

Defina a preferência do status de um novo projeto como Planejamento ou Ideia, Não Atual.

**Veja o porquê**

Um status Atual indica que um projeto está ativo e que o trabalho está sendo realizado ativamente. É raro um projeto precisar estar com esse status ao ser criado. Mesmo se você usar um modelo de projeto, há um &quot;planejamento&quot; envolvido na realização das atribuições de tarefas, no ajuste da data de conclusão planejada do projeto etc. O status do Planning também suprime notificações para os designados da tarefa e membros da equipe do projeto. Receber notificações antes que o projeto esteja ativo pode ser confuso para os envolvidos.

</br>
</br>

**Prática recomendada**

Habilite Criar linhas de base Automaticamente nas preferências do projeto global.

**Veja o porquê**

Toda vez que você altera o status de um projeto para Atual, o Workfront registra automaticamente uma linha de base do projeto. Esse &quot;instantâneo&quot; do projeto fornece informações históricas sobre como o plano do projeto mudou com o tempo. Por exemplo, você pode comparar o plano original do projeto com o plano atual ao mostrar à liderança como a mudança de prioridades ou a diminuição do escopo afetaram os prazos do projeto.

</br>
</br>

**Prática recomendada**

Marque todas as opções na seção Business Cases das preferências do projeto do sistema.

**Veja o porquê**

Ative todas as cinco opções para permitir que gerentes de projeto, planejadores e outros incluam qualquer uma dessas seções no business case de um projeto. Se as opções não estiverem ativadas, elas não aparecerão na janela business case. Os usuários podem deixar qualquer um dos campos em branco se não for necessário para esse projeto específico, mas não podem habilitar um campo no nível do projeto. Essas opções só podem ser ativadas globalmente na Configuração.

</br>
</br>

**Prática recomendada**

Nas preferências de problemas, marque a opção Atualizar automaticamente o status de um problema resolvível quando o status do objeto de resolução for alterado.

**Veja o porquê**

Quando um problema é convertido em um projeto, essa configuração de preferência &quot;vincula&quot; os status dos dois itens. Atualizar o status do projeto (o objeto de resolução) atualizará automaticamente o status do problema. Isso significa que o solicitante pode ver o progresso que está sendo feito em sua solicitação, mesmo que não tenha permissões para ver todo o projeto no Workfront.
