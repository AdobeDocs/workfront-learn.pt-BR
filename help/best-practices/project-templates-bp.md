---
title: Prática recomendada - Modelos de projeto
description: Explore as recomendações de práticas recomendadas dos especialistas da Adobe Workfront sobre a configuração, o gerenciamento e o uso de modelos de projeto do Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10919
exl-id: 17cd2e49-ee16-4b80-a8b2-ccc254fa8014
source-git-commit: d39151288d8b749940c5183063392ee471769445
workflow-type: tm+mt
source-wordcount: '1743'
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

**Aqui está o porquê**

Os modelos de projeto eliminam as suposições para os gerentes de projeto (e outros que criam projetos) sobre quais tarefas um projeto deve conter, como estruturar a linha do tempo etc. Os modelos são a maneira mais eficaz de acelerar a criação de projetos.

É importante ressaltar que os modelos fornecem consistência entre projetos de tipos semelhantes, para que as pessoas, os processos e os pontos de dados sejam detalhados da mesma maneira todas as vezes. Mesmo projetos com mudanças rápidas (um ou dois dias) e tarefas mínimas podem se beneficiar de serem criados com modelos de projeto.

Essa consistência entre projetos resulta em dados mais precisos, que são essenciais ao tomar decisões para sua equipe, em seu departamento e em toda a organização.

</br>
</br>

**Prática recomendada**

Estabeleça uma convenção de nomenclatura para modelos de projeto.

**Aqui está o porquê**

A nomenclatura consistente facilita a localização dos modelos. Também ajuda os gerentes de projeto e outros que criam projetos a selecionarem o modelo certo quando houver modelos com nomes semelhantes em várias equipes ou departamentos.

</br>
</br>

**Prática recomendada**

Estabeleça um grupo selecionado de usuários que possam criar e atualizar modelos de projeto.

**Aqui está o porquê**

Ter modelos de projeto consistentes e bem construídos é fundamental para um bom gerenciamento do trabalho e relatórios precisos. Limite o número de usuários que podem editar modelos para evitar alterações acidentais ou não aprovadas.

</br>
</br>

**Prática recomendada**

Use o Compartilhamento de projetos em um modelo de projeto para conceder acesso automaticamente aos projetos criados usando esse modelo.

**Aqui está o porquê**

O acesso a projetos específicos é concedido através do próprio projeto. Se o mesmo grupo de pessoas sempre precisar de acesso aos projetos criados com um modelo específico, adicione-o na opção Compartilhamento de projeto no modelo. Você não só pode controlar o acesso aos projetos assim que eles são criados, como também facilita os esforços de escalabilidade se as permissões precisarem mudar no futuro.

Para obter instruções sobre como compartilhar projetos criados usando um modelo, consulte o capítulo intitulado &quot;Como compartilhar projetos criados usando um modelo&quot; na [Compartilhar um modelo de projeto](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/create-and-manage-project-templates/share-a-project-template.html).

**Nota**: o compartilhamento de modelo concede acesso ao próprio modelo. Um usuário deve ter pelo menos permissões de Visualização para criar projetos com o modelo.

</br>
</br>

**Prática recomendada**

Atribua funções de trabalho ou equipes a tarefas, não a indivíduos.

**Aqui está o porquê**

Quando um usuário individual muda de cargo ou deixa a organização, você terá que atualizar manualmente os modelos de projeto que incluem essa pessoa. Isso leva tempo para parte dos administradores de sistema ou de grupo ou gerentes de projeto.

Se você usar funções de trabalho ou equipes nos modelos, as alterações na equipe não terão um efeito direto nos modelos do projeto, pois qualquer pessoa com essa função de trabalho ou equipe atribuída poderá receber o trabalho. Isso ajuda a garantir que o trabalho não seja perdido. As atribuições de funções de trabalho também facilitam a atribuição de trabalho a usuários individuais, já que o Workfront pode mostrar uma lista de pessoas com essa função de trabalho atribuída a você.

Além disso, as funções de trabalho são usadas pelas ferramentas de planejamento de recursos da Workfront para ajudá-lo a calcular os recursos necessários e planejar trabalhos futuros.

</br>
</br>

**Prática recomendada**

Evite ficar muito granular ao criar tarefas em um modelo de projeto. Limite o número de tarefas em um modelo de projeto para aquelas necessárias para concluir o trabalho.

**Aqui está o porquê**

Modelos de projeto muito complicados resultam em uma experiência ruim para os usuários — gerentes de projeto, gerentes de recursos, membros da equipe e muito mais. Muitas tarefas dificultam o gerenciamento da linha do tempo do projeto, com sobreposição de prazos de tarefa e várias tarefas atribuídas às mesmas funções de trabalho ou indivíduos.


</br>
</br>

**Prática recomendada**

Use a descrição da tarefa para capturar as pequenas etapas da tarefa, em vez de dividi-la em várias tarefas.

**Aqui está o porquê**

Se várias tarefas em uma linha forem atribuídas à mesma função de trabalho/indivíduo, isso indica que essas tarefas podem ser combinadas. Ter muitas tarefas atribuídas a um usuário pode fazer com que ele sinta que há mais trabalho a ser concluído, o que pode afetar a adoção do Workfront.

</br>
</br>

**Prática recomendada**

Verifique se as tarefas do modelo incluem durações de tarefas, horas planejadas e predecessores.

**Aqui está o porquê**

Esses três elementos (durações, horas planejadas e predecessores) são os blocos que formam a linha do tempo do projeto. Esses são os pontos-chave para saber quanto tempo levará o trabalho e quando ele precisa ser feito. As ferramentas de gerenciamento de recursos da Workfront usam durações e horas planejadas, além de atribuições de funções de trabalho, para calcular a capacidade, a disponibilidade e muito mais.

Se não tiver certeza de como estimar as durações ou as horas planejadas pela primeira vez, trabalhe com a equipe do projeto para definir algumas estimativas iniciais. Depois de usar o modelo, reúna-se com a equipe do projeto novamente para determinar onde as alterações podem ser feitas para tornar o modelo mais preciso. Se os usuários estiverem registrando horas no Workfront, é possível comparar as horas planejadas de um projeto com as horas reais para ver onde os ajustes são necessários.


</br>
</br>

**Prática recomendada**

Pré-configure os detalhes do projeto e anexe formulários personalizados ao modelo.

**Aqui está o porquê**

Verifique se as informações padrão para todos os projetos estão preenchidas no modelo do projeto. Isso não apenas ajuda a acelerar a criação de projetos, como também garante que as informações necessárias estejam lá e sejam consistentes em todos os projetos.

Anexe formulários de projeto personalizados que correspondam aos formulários de solicitação personalizados para obter informações enviadas ao converter a solicitação em um projeto usando o modelo.

Para obter instruções sobre como anexar um formulário personalizado a um objeto como um modelo de projeto, consulte [Anexar um formulário personalizado a um objeto](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/custom-data/custom-forms/custom-forms-using-a-custom-form.html).

</br>
</br>

**Prática recomendada**

Revise e atualize modelos de projeto regularmente.

**Aqui está o porquê**

Conforme os processos e as equipes mudam, os modelos de projeto devem ser atualizados. Estabeleça uma cadência regular, como trimestral, para verificar e ver quais modelos não estão sendo usados ativamente. Você pode desativá-los para que eles ainda estejam no Workfront, mas não apareçam nas listas de seleção de modelo.

Para obter instruções sobre como desativar um modelo de projeto, consulte [Desativar um modelo de projeto](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/create-and-manage-project-templates/deactivate-a-project-template.html).

</br>
</br>

**Prática recomendada**

Verifique os modelos para garantir que eles tenham todas as informações necessárias antes de você compartilhá-los e que outras pessoas comecem a usá-los.


**Aqui está o porquê**

Como os modelos serão usados várias vezes para criar projetos, você precisará verificar se tudo está configurado corretamente e completamente. Isso leva à consistência em todos os projetos e a dados precisos para a geração de relatórios.

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
* Verifique a equipe do projeto para garantir que não haja pessoas adicionais atribuídas

</br>
</br>

**Prática recomendada**

Ao ajustar a opção Modo de programação em um modelo, revise e atualize as restrições da tarefa.

**Aqui está o porquê**

Misturar diferentes restrições de tarefa em um projeto pode causar cálculos inesperados e confusos de datas planejadas. Por exemplo, quando a opção Data inicial é selecionada para a opção Modo de programação, todas as tarefas criadas nesse projeto recebem a restrição de tarefa O mais rápido possível por padrão. Se, posteriormente, você alternar a opção Modo de Programação para Data de Conclusão, quaisquer tarefas criadas terão uma restrição de tarefa O Mais Tarde Possível por padrão. Ter uma combinação não intencional de tarefas com cada uma dessas restrições pode resultar em datas planejadas confusas na linha do tempo do seu projeto.

Para entender melhor as restrições de tarefas e como usá-las, consulte [Entender e gerenciar tipos de duração e restrições de tarefa](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/intermediate-projects/understand-and-manage-duration-types-and-task-constraints.html).

</br>
</br>

**Prática recomendada**

Verifique a equipe do projeto no modelo e remova os usuários que não trabalharão com o projeto.

**Aqui está o porquê**

Ao criar um modelo a partir de um projeto existente, a menos que você escolha a opção Limpar atribuições durante a criação, o Workfront traz as pessoas às quais foram atribuídas tarefas/problemas no projeto na seção Pessoas. E enquanto estiver trabalhando com seu modelo, talvez você queira remover essas pessoas que foram anteriormente designadas para trabalhar ou alterar uma atribuição que você mesmo fez no modelo.

Todos esses usuários serão listados como parte da equipe do projeto, nas seções Pessoas e Agendamento do projeto. Como resultado, eles serão propagados para todos os projetos criados a partir desse modelo. Isso pode causar confusão para o usuário, pois, como parte da equipe do projeto, ele recebe notificações sobre a atividade no projeto, vê o projeto na lista Projetos em que estou e obtém permissões para o projeto e suas tarefas, problemas e documentos.

Para obter instruções sobre como editar a equipe do projeto em um modelo de projeto, consulte [Editar a equipe do projeto em um modelo de projeto](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/create-and-manage-project-templates/edit-the-project-team-in-a-project-template.html).
