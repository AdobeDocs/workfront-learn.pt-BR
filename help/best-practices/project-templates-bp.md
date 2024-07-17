---
title: Prática Recomendada – Modelos de Projeto
description: Explore as sugestões de práticas recomendadas de especialistas do Adobe Workfront sobre como configurar, gerenciar e usar modelos de projeto do Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10919
exl-id: 17cd2e49-ee16-4b80-a8b2-ccc254fa8014
source-git-commit: d39151288d8b749940c5183063392ee471769445
workflow-type: tm+mt
source-wordcount: '1743'
ht-degree: 100%

---

# Prática Recomendada – Modelos de Projeto

## O que é uma “prática recomendada” do Adobe Workfront?

As práticas recomendadas são diretrizes para um curso de ação eficaz e eficiente; elas podem ser facilmente adotadas por qualquer usuário da empresa e replicadas com sucesso em toda a organização.

Ao revisar essas recomendações, lembre-se de que algumas práticas recomendadas do Workfront são universais, enquanto outras podem ser mais específicas para um determinado assunto. Use essas práticas recomendadas como uma base para orientar as configurações e o uso do sistema do Workfront.

## Navegar nesta página

Ao percorrer esta página, primeiro você encontrará uma lista resumida de todas as práticas recomendadas para o tópico. Isso permite que você revise as recomendações sem se aprofundar nos detalhes do “porquê”.

A seção “Por que essas práticas recomendadas?” , encontrada após a lista resumida, fornece mais detalhes sobre algumas práticas recomendadas e por que elas são consideradas como um processo, ferramenta ou recurso que você deve considerar implementar na sua instância do Workfront.

</br>
</br>

## Práticas recomendadas do modelo de projeto

* Use modelos ao criar projetos.

* Estabeleça uma convenção de nomenclatura para modelos de projeto.

* Estabeleça um grupo selecionado de usuários que possam criar e atualizar modelos de projeto.

* Use o Compartilhamento de projetos em um modelo de projeto para conceder acesso automaticamente aos projetos criados usando esse modelo.

* Atribua funções de trabalho ou equipes a tarefas, não a indivíduos.

* Evite ser muito granular ao criar tarefas em um modelo de projeto. Limite o número de tarefas em um modelo de projeto para as que forem necessárias para concluir o trabalho.

* Use a descrição da tarefa para capturar as pequenas etapas da tarefa, em vez de dividi-la em várias.

* Verifique se as tarefas do modelo incluem duração, horas planejadas e predecessores.

* Pré-configure os detalhes do projeto e anexe formulários personalizados ao modelo.

* Revise e atualize modelos de projeto regularmente.

* Verifique os modelos para garantir que eles tenham todas as informações necessárias antes de compartilhá-los e que outras pessoas comecem a usá-los.

* Ao ajustar a opção “Agendar de” em um modelo, revise e atualize as restrições da tarefa.

* Verifique a equipe do projeto no modelo e remova os usuários e usuárias que não serão associados ao projeto.

</br>
</br>

## Por que essas práticas são recomendadas?

**Prática recomendada**

Use modelos ao criar projetos.

**Entenda o porquê**

Os modelos de projeto eliminam as suposições dos gerentes (e outros que criam projetos) sobre quais tarefas um projeto deve conter, como estruturar a linha do tempo etc. Os modelos são a maneira mais eficaz de acelerar a criação de projetos.

É importante ressaltar que os modelos fornecem consistência entre projetos semelhantes, para que pessoas, processos e pontos de dados sejam sempre detalhados da mesma maneira. Mesmo projetos com entregas rápidas (um ou dois dias) e tarefas mínimas podem se beneficiar ao serem criados com modelos de projeto.

Essa consistência entre projetos resulta em dados mais precisos, que são essenciais ao tomar decisões para sua equipe, em seu departamento e em toda a organização.

</br>
</br>

**Prática recomendada**

Estabeleça uma convenção de nomenclatura para modelos de projeto.

**Entenda o porquê**

A nomenclatura consistente torna os modelos mais fáceis de serem encontrados. Também ajuda os gerentes de projeto e outras pessoas que criam projetos a selecionar o modelo certo quando há modelos com nomes semelhantes em várias equipes ou departamentos.

</br>
</br>

**Prática recomendada**

Estabeleça um grupo selecionado de usuários que possam criar e atualizar modelos de projeto.

**Entenda o porquê**

Ter modelos de projeto consistentes e bem construídos é fundamental para um bom gerenciamento de trabalho e relatórios precisos. Limite o número de usuários que podem editar modelos para evitar alterações acidentais ou não aprovadas.

</br>
</br>

**Prática recomendada**

Use o Compartilhamento de projetos em um modelo de projeto para conceder acesso automaticamente aos projetos criados usando esse modelo.

**Entenda o porquê**

O acesso a projetos específicos é concedido através do próprio projeto. Se o mesmo grupo de pessoas sempre precisar de acesso a projetos criados com um modelo específico, adicione-as na opção Compartilhamento de Projeto no modelo. Você não só pode controlar o acesso aos projetos assim que são criados, como também agilizar os esforços de escalabilidade caso as permissões precisem ser alteradas no futuro.

Para obter instruções sobre como compartilhar projetos criados usando um modelo, consulte o capítulo intitulado &quot;Como compartilhar projetos criados usando um modelo&quot; em [Compartilhar um modelo de projeto](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/create-and-manage-project-templates/share-a-project-template.html?lang=pt-BR).

**Observação**: o compartilhamento de modelo concede acesso ao próprio modelo. Os usuários devem ter pelo menos permissões de Visualização para criar projetos com o modelo.

</br>
</br>

**Prática recomendada**

Atribua funções de trabalho ou equipes a tarefas, não a indivíduos.

**Entenda o porquê**

Quando alguém muda de cargo ou sai da organização, você terá que atualizar manualmente os modelos de projeto que incluem essa pessoa. Isso leva tempo por parte dos administradores do sistema ou do grupo ou gerentes de projeto.

Se você usar funções no trabalho ou equipes em modelos, as alterações de equipe não terão um efeito direto em seus modelos de projeto porque qualquer pessoa com essa função no trabalho ou dessa equipe poderá ser designada para o trabalho. Isso ajuda a garantir que o trabalho não fique para trás. As atribuições de funções no trabalho também facilitam a atribuição de trabalho a usuários individuais, pois o Workfront pode mostrar uma lista de pessoas atribuídas a essa função.

Além disso, as funções no trabalho são usadas pelas ferramentas de planejamento de recursos do Workfront para ajudar você a calcular os recursos necessários e planejar o trabalho futuro.

</br>
</br>

**Prática recomendada**

Evite ser muito granular ao criar tarefas em um modelo de projeto. Limite o número de tarefas em um modelo de projeto para as que forem necessárias para concluir o trabalho.

**Entenda o porquê**

Modelos de projeto excessivamente complicados resultam em uma experiência ruim para os usuários: gerentes de projeto, gerentes de recursos, membros da equipe e muito mais. Muitas tarefas dificultam o gerenciamento da linha do tempo do projeto, com sobreposição de prazos de tarefa e várias tarefas atribuídas às mesmas funções de trabalho ou indivíduos.


</br>
</br>

**Prática recomendada**

Use a descrição da tarefa para capturar as pequenas etapas da tarefa, em vez de dividi-la em várias.

**Entenda o porquê**

Se várias tarefas consecutivas forem atribuídas à mesma função no trabalho/pessoa, é uma indicação de que essas tarefas podem ser combinadas. Ter muitas tarefas atribuídas a uma pessoa pode fazer com que ela sinta que há mais trabalho a ser concluído, o que pode afetar a adoção do Workfront.

</br>
</br>

**Prática recomendada**

Verifique se as tarefas do modelo incluem duração, horas planejadas e predecessores.

**Entenda o porquê**

Essas três coisas – durações, horas planejadas e predecessores – são a base para a construção da linha do tempo do projeto. São fundamentais para saber quanto tempo o trabalho levará e quando precisa ser concluído. As ferramentas de gerenciamento de recursos do Workfront usam durações e horas planejadas, além de atribuições de funções no trabalho, para calcular a capacidade, a disponibilidade de recursos e muito mais.

Se você não tiver certeza de como estimar durações ou horas planejadas pela primeira vez, trabalhe com a equipe do projeto para definir algumas estimativas iniciais. Depois de usar o modelo, reúna-se novamente com a equipe do projeto para determinar onde fazer alterações para tornar o modelo mais preciso. Se os usuários ou usuárias estiverem registrando o tempo no Workfront, você poderá comparar as horas planejadas de um projeto com as horas reais para ver onde serão necessários ajustes.


</br>
</br>

**Prática recomendada**

Pré-configure os detalhes do projeto e anexe formulários personalizados ao modelo.

**Entenda o porquê**

Certifique-se de que as informações padrão para todos os projetos sejam preenchidas no modelo de projeto. Isso não apenas ajuda a acelerar a criação de projetos, como também garante que as informações necessárias estejam lá e sejam uniformes em todos os projetos.

Anexe formulários personalizados de projeto que correspondam aos formulários personalizados de solicitação para obter informações enviadas ao converter a solicitação em um projeto usando o modelo.

Para obter instruções sobre como anexar um formulário personalizado a um objeto como modelo de projeto, consulte [Anexar um formulário personalizado a um objeto](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/custom-data/custom-forms/custom-forms-using-a-custom-form.html?lang=pt-BR).

</br>
</br>

**Prática recomendada**

Revise e atualize modelos de projeto regularmente.

**Entenda o porquê**

À medida que os processos e as equipes mudam, os modelos de projeto devem ser atualizados. Estabeleça uma cadência regular, como trimestral, para verificar quais modelos não estão sendo usados ativamente. Você pode desativá-los para que ainda estejam no Workfront, mas não apareçam nas listas de seleção de modelo.

Para obter instruções sobre como desativar um modelo de projeto, consulte [Desativar um modelo de projeto](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/create-and-manage-project-templates/deactivate-a-project-template.html?lang=pt-BR).

</br>
</br>

**Prática recomendada**

Verifique os modelos para garantir que eles tenham todas as informações necessárias antes de compartilhá-los e que outras pessoas comecem a usá-los.


**Entenda o porquê**

Como os modelos serão usados repetidamente para criar projetos, é bom ter tudo configurado de maneira adequada e completa. Isso leva à consistência em todos os projetos e a dados precisos para a geração de relatórios.

Além das configurações de tarefa, como duração e horas planejadas, alguns itens a serem revisados antes de compartilhar modelos incluem:

* Configuração Agendar de
* Restrições de tarefa
* Proprietário do projeto, patrocinador, grupo e empresa
* Portfólio e programa
* Caminho de marcos e etapas
* Processos de aprovação
* Certifique-se de que os usuários atribuídos a tarefas em projetos tenham acesso de contribuição ao projeto
* Conjunto de recursos
* Notificações de lembrete
* Agendar
* Configuração de moeda (se aplicável)
* Anexar documentos padrão
* Anexar os formulários personalizados necessários
* Verifique a equipe do projeto para ter certeza de que não haja pessoas demais designadas

</br>
</br>

**Prática recomendada**

Ao ajustar a opção Modo cronograma em um modelo, revise e atualize as restrições de tarefa.

**Entenda o porquê**

A mistura de diferentes restrições de tarefas em um projeto pode causar cálculos inesperados e confusos de datas planejadas. Por exemplo, quando a Data inicial é selecionada para a opção Modo cronograma, todas as tarefas criadas nesse projeto recebem a restrição de tarefa “O mais breve possível” por padrão. Se você alterar posteriormente a opção Modo cronograma para Data de conclusão, todas as tarefas criadas terão uma restrição de tarefa “O mais tarde possível” por padrão. Ter uma combinação não intencional de tarefas com cada uma dessas restrições pode resultar em datas planejadas confusas na linha do tempo do projeto.

Para entender melhor as restrições de tarefas e como usá-las, consulte [Entender e gerenciar tipos de duração e restrições de tarefa](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/intermediate-projects/understand-and-manage-duration-types-and-task-constraints.html?lang=pt-BR).

</br>
</br>

**Prática recomendada**

Verifique a equipe do projeto no modelo e remova pessoas que não trabalharão com o projeto.

**Entenda o porquê**

Quando você cria um modelo a partir de um projeto existente, a menos que você escolha a opção Limpar atribuições durante a criação, o Workfront inclui as pessoas às quais foram atribuídas tarefas/problemas no projeto na seção Pessoas. Ao trabalhar com seu modelo, você pode remover pessoas a quem foi atribuído trabalho anteriormente ou alterar uma atribuição que você fez no modelo.

Todos esses usuários serão listados como parte da equipe do projeto, nas seções Pessoas e Agendamento do projeto. Como resultado, isso será propagado para todos os projetos criados a partir desse modelo. Isso pode causar confusão para o usuário ou usuária, pois, como parte da equipe do projeto, recebe notificações sobre a atividade, vê o projeto na lista “Projetos em que estou” e obtém permissões para o projeto e suas tarefas, problemas e documentos.

Para obter instruções sobre como editar a equipe do projeto em um modelo de projeto, consulte [Editar a equipe do projeto em um modelo de projeto](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/create-and-manage-project-templates/edit-the-project-team-in-a-project-template.html?lang=pt-BR).
