---
title: Prática recomendada - Modelos de projeto
description: Explore as recomendações de práticas recomendadas dos especialistas da Adobe Workfront sobre a configuração, o gerenciamento e o uso de modelos de projeto do Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10919
exl-id: 17cd2e49-ee16-4b80-a8b2-ccc254fa8014
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1614'
ht-degree: 0%

---

# Prática recomendada - Modelos de projeto

## O que é uma &quot;prática recomendada&quot; do Adobe Workfront?

As práticas recomendadas são diretrizes que representam um curso de ação eficaz e eficiente; são facilmente adotadas por você e pelos usuários em sua empresa; e podem ser replicadas com sucesso em toda a organização.

Ao revisar essas recomendações, lembre-se de que algumas práticas recomendadas do Workfront são universais, enquanto outras podem ser mais específicas ao tópico. Use essas práticas recomendadas como uma estrutura para ajudar a orientar as configurações e o uso do sistema Workfront.

## Navegando nesta página

Ao percorrer essa página, primeiro você encontrará uma lista de alto nível de todas as práticas recomendadas para o tópico. Isso permite analisar as recomendações sem mergulhar nos detalhes do &quot;por quê&quot;.

O &quot;Por que essas práticas recomendadas?&quot; A área, localizada após a lista de alto nível, fornece mais detalhes sobre algumas das práticas recomendadas e por que elas são consideradas um processo, ferramenta, etc. Você deve considerar a implementação com sua instância do Workfront.

</br>
</br>

## Práticas recomendadas do modelo de projeto

* Use modelos ao criar projetos.

* Estabeleça uma convenção de nomenclatura para modelos de projeto.

* Estabeleça um grupo selecionado de usuários que possam criar e atualizar modelos de projeto.

* Use o Compartilhamento de projetos em um modelo de projeto para conceder acesso automaticamente aos projetos criados usando esse modelo.

* Atribua funções de trabalho ou equipes a tarefas, não a indivíduos.

* Evite ficar muito granular ao criar tarefas em um modelo de projeto. Limite o número de tarefas em um modelo de projeto para aquelas necessárias para concluir o trabalho.

* Use a descrição da tarefa para capturar as pequenas etapas da tarefa, em vez de dividi-la em várias tarefas.

* Verifique se as tarefas do modelo incluem durações de tarefas, horas planejadas e predecessores.

* Pré-configure os detalhes do projeto e anexe formulários personalizados ao modelo.

* Revise e atualize modelos de projeto regularmente.

* Verifique os modelos para garantir que eles tenham todas as informações necessárias antes de você compartilhá-los e que outras pessoas comecem a usá-los.

* Ao ajustar a opção Agendar de em um modelo, revise e atualize as restrições da tarefa.

* Verifique a equipe do projeto no modelo e remova os usuários que não serão associados ao projeto.

</br>
</br>

## Por que essas práticas recomendadas?

**Prática recomendada**

Use modelos ao criar projetos.

**Veja o porquê**

Os modelos de projeto eliminam as suposições para os gerentes de projeto (e outros que criam projetos) sobre quais tarefas um projeto deve conter, como estruturar a linha do tempo etc. Os modelos são a maneira mais eficaz de acelerar a criação de projetos.

É importante ressaltar que os modelos fornecem consistência entre projetos de tipos semelhantes, para que as pessoas, os processos e os pontos de dados sejam detalhados da mesma maneira todas as vezes. Mesmo projetos com mudanças rápidas (um ou dois dias) e tarefas mínimas podem se beneficiar de serem criados com modelos de projeto.

Essa consistência entre projetos resulta em dados mais precisos, que são essenciais ao tomar decisões para sua equipe, em seu departamento e em toda a organização.

</br>
</br>

**Prática recomendada**

Estabeleça uma convenção de nomenclatura para modelos de projeto.

**Veja o porquê**

A nomenclatura consistente facilita a localização dos modelos. Também ajuda os gerentes de projeto e outros que criam projetos a selecionarem o modelo certo quando houver modelos com nomes semelhantes em várias equipes ou departamentos.

</br>
</br>

**Prática recomendada**

Estabeleça um grupo selecionado de usuários que possam criar e atualizar modelos de projeto.

**Veja o porquê**

Ter modelos de projeto consistentes e bem construídos é fundamental para um bom gerenciamento do trabalho e relatórios precisos. Limite o número de usuários que podem editar modelos para evitar alterações acidentais ou não aprovadas.

</br>
</br>

**Prática recomendada**

Use o Compartilhamento de projetos em um modelo de projeto para conceder acesso automaticamente aos projetos criados usando esse modelo.

**Veja o porquê**

O acesso a projetos específicos é concedido através do próprio projeto. Se o mesmo grupo de pessoas sempre precisar de acesso aos projetos criados com um modelo específico, adicione-o na opção Compartilhamento de projeto no modelo. Você não só pode controlar o acesso aos projetos assim que eles são criados, como também simplifica os esforços de escalabilidade se as permissões precisarem ser alteradas no futuro.

**Nota**: o compartilhamento de modelo concede acesso ao próprio modelo. Um usuário deve ter pelo menos permissões de Visualização para criar projetos com o modelo.

</br>
</br>

**Prática recomendada**

Atribua funções de trabalho ou equipes a tarefas, não a indivíduos.

**Veja o porquê**

Quando um usuário individual muda de cargo ou deixa a organização, você terá que atualizar manualmente os modelos de projeto que incluem essa pessoa. Isso leva tempo para parte dos administradores de sistema ou de grupo ou gerentes de projeto.

Se você usar funções de trabalho ou equipes nos modelos, as alterações na equipe não terão um efeito direto nos modelos do projeto, pois qualquer pessoa com essa função de trabalho ou equipe atribuída poderá receber o trabalho. Isso ajuda a garantir que o trabalho não escorra pelas fendas. As atribuições de funções de trabalho também facilitam a atribuição de trabalho a usuários individuais, já que o Workfront pode mostrar uma lista de pessoas com essa função de trabalho atribuída a você.

Além disso, as funções de trabalho são usadas pelas ferramentas de planejamento de recursos da Workfront para ajudar você a calcular os recursos necessários e planejar trabalhos futuros.

</br>
</br>

**Prática recomendada**

Evite ficar muito granular ao criar tarefas em um modelo de projeto. Limite o número de tarefas em um modelo de projeto para aquelas necessárias para concluir o trabalho.

**Veja o porquê**

Modelos de projeto muito complicados resultam em uma experiência ruim para os usuários — gerentes de projeto, gerentes de recursos, membros da equipe e muito mais. Muitas tarefas dificultam o gerenciamento da linha do tempo do projeto, com sobreposição de prazos de tarefa e várias tarefas atribuídas às mesmas funções de trabalho ou indivíduos.


</br>
</br>

**Prática recomendada**

Use a descrição da tarefa para capturar as pequenas etapas da tarefa, em vez de dividi-la em várias tarefas.

**Veja o porquê**

Se várias tarefas em uma linha forem atribuídas à mesma função de trabalho/indivíduo, isso indica que essas tarefas podem ser combinadas. Ter muitas tarefas atribuídas a um usuário pode fazer com que ele sinta que há mais trabalho a ser concluído, o que pode afetar a adoção do Workfront.

</br>
</br>

**Prática recomendada**

Verifique se as tarefas do modelo incluem durações de tarefas, horas planejadas e predecessores.

**Veja o porquê**

Essas três coisas — durações, horas planejadas e predecessores — são os blocos que formam a linha do tempo do projeto. Esses são os pontos-chave para saber quanto tempo levará o trabalho e quando ele precisa ser feito. As durações das ferramentas de gerenciamento de recursos da Workfront e as horas planejadas, além das atribuições de funções de trabalho, para calcular a capacidade, a disponibilidade e muito mais.

Se não tiver certeza de como estimar as durações ou as horas planejadas pela primeira vez, trabalhe com a equipe do projeto para definir algumas estimativas iniciais. Depois de usar o modelo, reúna-se com a equipe do projeto novamente para determinar onde as alterações podem ser feitas para tornar o modelo mais preciso. Se os usuários estiverem registrando o tempo no Workfront, é possível comparar as horas planejadas de um projeto com as horas reais para ver onde os ajustes são necessários.


</br>
</br>

**Prática recomendada**

Pré-configure os detalhes do projeto e anexe formulários personalizados ao modelo.

**Veja o porquê**

Verifique se as informações padrão para todos os projetos estão preenchidas no modelo do projeto. Isso não apenas ajuda a acelerar a criação de projetos, como também garante que as informações necessárias estejam lá e sejam consistentes em todos os projetos.

Anexe formulários de projeto personalizados que correspondam aos formulários de solicitação personalizados para obter informações enviadas ao converter a solicitação em um projeto usando o modelo.

</br>
</br>

**Prática recomendada**

Revise e atualize modelos de projeto regularmente.

**Veja o porquê**

Conforme os processos e as equipes mudam, os modelos de projeto devem ser atualizados. Estabeleça uma cadência regular, como trimestral, para verificar e ver quais modelos não estão sendo usados ativamente. Você pode desativá-los para que ainda estejam no Workfront, mas não apareçam nas listas de seleção de modelo.

</br>
</br>

**Prática recomendada**

Verifique os modelos para garantir que eles tenham todas as informações necessárias antes de você compartilhá-los e que outras pessoas comecem a usá-los.


**Veja o porquê**

Como os modelos serão usados várias vezes para criar projetos, você desejará garantir que tudo esteja configurado corretamente e completamente. Isso leva à consistência em todos os projetos e a dados precisos para a geração de relatórios.

Além das configurações de tarefa, como duração e horas planejadas, alguns itens a serem revisados antes de compartilhar modelos incluem:

* Configuração Agendar de
* Restrições de tarefa
* Proprietário do projeto, patrocinador, grupo e empresa
* Portfolio e programa
* Caminho e etapas da etapa
* Processos de aprovação
* Verificar se os usuários com tarefas atribuídas em projetos têm acesso ao Contribute
* Conjunto de recursos
* Notificações de lembrete
* Agendar
* Configuração de moeda (se aplicável)
* Anexar documentos padrão
* Anexar os formulários aduaneiros necessários
* Verifique a equipe do projeto para garantir que não haja pessoas extras atribuídas

</br>
</br>

**Prática recomendada**

Ao ajustar a opção Agendar de em um modelo, revise e atualize as restrições da tarefa.

**Veja o porquê**

Misturar diferentes restrições de tarefa em um projeto pode causar cálculos inesperados e confusos de datas planejadas. Por exemplo, quando Data Inicial é selecionada para a opção Agendar de, todas as tarefas criadas nesse projeto recebem a restrição de tarefa O Mais Breve Possível por padrão. Se você alternar posteriormente a opção Agendar de para Data de Conclusão, qualquer tarefa criada terá uma restrição de tarefa O Mais Tarde Possível por padrão. Ter uma combinação não intencional de tarefas com cada uma dessas restrições pode resultar em datas planejadas confusas na linha do tempo do seu projeto.


</br>
</br>

**Prática recomendada**

Verifique a equipe do projeto no modelo e remova os usuários que não trabalharão com o projeto.

**Veja o porquê**

Quando você cria um modelo a partir de um projeto existente, ele reúne as pessoas que receberam tarefas/problemas no projeto. E, ao trabalhar com seu modelo, você pode remover as pessoas às quais foram atribuídos trabalhos anteriormente ou alterar uma atribuição que você fez a si mesmo no modelo.

Todos esses usuários serão listados como parte da equipe do projeto, nas seções Pessoas e Agendamento do projeto. Como resultado, eles serão propagados para todos os projetos criados a partir desse modelo. Isso pode causar confusão para o usuário, pois, como parte da equipe do projeto, ele recebe notificações sobre a atividade no projeto, vê o projeto na lista Projetos em que estou e obtém permissões para o projeto e suas tarefas, problemas e documentos.
