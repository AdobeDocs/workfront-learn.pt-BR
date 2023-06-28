---
title: Prática recomendada - Filtros, exibições e agrupamentos
description: Explore as recomendações de práticas recomendadas dos especialistas do Adobe Workfront sobre a configuração, o gerenciamento e o uso de filtros, visualizações e agrupamentos do Workfront.
feature: Reports and Dashboards
role: Admin, Leader, User
level: Beginner
jira: KT-10911
exl-id: 845aa0b4-3fe9-4bc1-9dde-2f22c537e758
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 0%

---

# Prática recomendada - Filtros, exibições e agrupamentos

## O que é uma &quot;prática recomendada&quot; do Adobe Workfront?

As práticas recomendadas são diretrizes que representam um curso de ação eficaz e eficiente; são facilmente adotadas por você e pelos usuários em sua empresa; e podem ser replicadas com sucesso em toda a organização.

Ao revisar essas recomendações, lembre-se de que algumas práticas recomendadas do Workfront são universais, enquanto outras podem ser mais específicas ao tópico. Use essas práticas recomendadas como uma estrutura para ajudar a orientar as configurações e o uso do sistema Workfront.

## Navegando nesta página

Ao percorrer essa página, primeiro você encontrará uma lista de alto nível de todas as práticas recomendadas para o tópico. Isso permite analisar as recomendações sem mergulhar nos detalhes do &quot;por quê&quot;.

O &quot;Por que essas práticas recomendadas?&quot; A área, localizada após a lista de alto nível, fornece mais detalhes sobre algumas das práticas recomendadas e por que elas são consideradas um processo, ferramenta, etc. Você deve considerar a implementação com sua instância do Workfront.

</br>
</br>

## Práticas recomendadas de filtros, visualizações e agrupamentos

* Reduza o número de relatórios personalizados que você cria utilizando filtros, visualizações e agrupamentos em uma lista de objetos para obter os dados necessários.

* Use os controles de lista em modelos de layout para ocultar filtros, visualizações e agrupamentos desnecessários para objetos usados com frequência (projetos, tarefas, programas etc.).

* Compartilhe filtros, visualizações e agrupamentos personalizados relevantes para os fluxos de trabalho e processos de sua organização por meio dos controles de lista em modelos de layout.

* Ao criar filtros para status do projeto, status da tarefa ou status do problema, use (objeto)>>Status Igual à origem do campo/nome do campo com o modificador Igual, em vez da origem/nome do campo Projeto>>Status.

</br>
</br>

## Por que essas práticas recomendadas?

**Prática recomendada**

Reduza o número de relatórios personalizados que você cria utilizando filtros, visualizações e agrupamentos em uma lista de objetos para obter os dados necessários.

**Veja o porquê**

Criar relatórios de uso único para cada segmento de dados que você deseja ver é demorado e desorganiza o sistema do Workfront.

</br>
</br>

**Prática recomendada**

Use os controles de lista em modelos de layout para ocultar filtros, visualizações e agrupamentos desnecessários para objetos usados com frequência (projetos, tarefas, programas etc.).

**Veja o porquê**

Menos é mais. Ocultar as opções de filtro, visualização e lista de agrupamento não relevantes para os fluxos de trabalho diários dos usuários restringe as listas, facilitando aos usuários encontrar o que precisam mais rápido.

</br>
</br>

**Prática recomendada**

Compartilhe filtros, visualizações e agrupamentos personalizados relevantes para os fluxos de trabalho e processos de sua organização por meio dos controles de lista em modelos de layout.

**Veja o porquê**

Se você criou filtros, visualizações e agrupamentos que exibem informações específicas para os processos diários dos usuários, é fácil compartilhá-los por meio dos modelos de layout. Isso garante que todos os usuários atribuídos ao modelo de layout tenham opções de filtro, exibição e agrupamento relevantes para seus workflows.

Personalizar as informações que você deseja que fiquem visíveis para os usuários por meio dos modelos de layout também economiza tempo para os administradores de sistema e de grupo, pois eles não precisarão compartilhar cada filtro, visualização ou opção de agrupamento individualmente.

</br>
</br>

**Prática recomendada**

Ao criar filtros para status do projeto, status da tarefa ou status do problema, use (objeto)>>Status Igual à origem do campo/nome do campo com o modificador Igual, em vez da origem/nome do campo Projeto>>Status.

**Veja o porquê**

Ao usar (objeto)>>Igual a, você está incluindo todos os status personalizados que têm esse status específico atribuído no campo Igual a nas configurações de status. Ao passo que a configuração do filtro como (objeto)>>Status > Igual exige que você selecione estatutos específicos para o filtro. Isso pode apresentar um desafio de manutenção se você precisar levar em conta esses novos status em vários filtros. Cada filtro precisaria ser aberto e atualizado com o novo status.

Por exemplo, se quiser ver todos os projetos atuais, você pode configurar seu filtro para ler Projeto>>Status > Igual > Atual. Porém, se alguém adicionar um status personalizado chamado Ativo e equipará-lo a Atual, esse filtro não encontrará projetos com o status Ativo. No entanto, se você usar Projeto>>> Status igual a > Igual > Atual, o filtro localizará objetos com o status Atual ou Ativo, pois ambos têm o status Atual no campo Igual a.
