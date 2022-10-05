---
title: Prática recomendada - Modelos de projeto
description: Explore as recomendações de práticas recomendadas dos especialistas do Adobe Workfront sobre como configurar, gerenciar e usar modelos de projeto do Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
kt: 10919
exl-id: 17cd2e49-ee16-4b80-a8b2-ccc254fa8014
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '1614'
ht-degree: 0%

---

# Prática recomendada - Modelos de projeto

## O que é uma &quot;prática recomendada&quot; do Adobe Workfront?

As melhores práticas são orientações que representam uma linha de ação eficaz e eficiente; sejam adotados facilmente por você e pelos usuários em sua empresa; e podem ser replicados com êxito em toda a organização.

À medida que você revisa essas recomendações, lembre-se de que algumas práticas recomendadas do Workfront são universais, enquanto outras podem ser mais específicas para o tópico. Use essas práticas recomendadas como estrutura para ajudar a orientar as configurações e o uso do sistema Workfront.

## Navegar nesta página

Ao rolar por essa página, primeiro você encontrará uma lista de alto nível de todas as práticas recomendadas para o tópico. Isso permite que você revise as recomendações sem entrar nos detalhes de &quot;por quê&quot;.

O &quot;Por que essas práticas recomendadas estão sendo usadas?&quot; , encontrada após a lista de alto nível, fornece mais detalhes sobre algumas práticas recomendadas e por que elas são consideradas como um processo, ferramenta etc., você deve considerar a implementação com sua instância do Workfront.

</br>
</br>

## Práticas recomendadas para o modelo de projeto

* Use modelos ao criar projetos.

* Estabeleça uma convenção de nomenclatura para modelos de projeto.

* Estabeleça um grupo selecionado de usuários que podem fazer e atualizar modelos de projeto.

* Use o Compartilhamento de projetos em um modelo de projeto para conceder acesso automaticamente aos projetos criados usando esse modelo.

* Atribuir funções ou equipes a tarefas, não a indivíduos.

* Evite ser muito granular ao criar tarefas em um modelo de projeto. Limite o número de tarefas em um modelo de projeto para as necessárias para concluir o trabalho.

* Use a descrição da tarefa para capturar as pequenas etapas da tarefa, em vez de dividi-la em várias tarefas.

* Certifique-se de que as tarefas do modelo incluam durações de tarefas, horas planejadas e antecessores.

* Pré-configurar os detalhes do projeto e anexar formulários personalizados ao modelo.

* Revise e atualize regularmente modelos de projeto.

* Verifique os modelos para garantir que eles tenham todas as informações necessárias antes de compartilhá-los e que outros comecem a usá-los.

* Ao ajustar a opção Programar de em um modelo, revise e atualize as restrições de tarefa.

* Verifique a equipe do projeto no modelo e remova os usuários que não serão associados ao projeto.

</br>
</br>

## Por que essas práticas recomendadas estão presentes?

**Prática recomendada**

Use modelos ao criar projetos.

**Veja o porquê**

Os modelos de projeto retiram a suposição dos gerentes de projeto (e outros criando projetos) sobre quais tarefas um projeto deve conter, como estruturar a linha do tempo etc. Os modelos são a maneira mais eficaz de acelerar a criação de projetos.

Importante: os modelos fornecem consistência em projetos de tipos semelhantes, para que pessoas, processos e pontos de dados sejam detalhados da mesma maneira todas as vezes. Até mesmo projetos com retornos rápidos (um ou dois dias) e tarefas mínimas podem se beneficiar de serem criados com modelos de projeto.

Essa consistência nos projetos resulta em dados mais precisos, que são essenciais ao tomar decisões para sua equipe, em seu departamento e em toda a organização.

</br>
</br>

**Prática recomendada**

Estabeleça uma convenção de nomenclatura para modelos de projeto.

**Veja o porquê**

A nomenclatura consistente facilita a localização de modelos. Também ajuda os gerentes de projeto e outros que criam projetos a selecionarem o modelo certo quando houver modelos com nomes semelhantes em várias equipes ou departamentos.

</br>
</br>

**Prática recomendada**

Estabeleça um grupo selecionado de usuários que podem fazer e atualizar modelos de projeto.

**Veja o porquê**

Ter modelos de projeto bem construídos e consistentes é fundamental para um bom gerenciamento de trabalho e relatórios precisos. Limite o número de usuários que podem editar modelos para evitar alterações acidentais ou não aprovadas.

</br>
</br>

**Prática recomendada**

Use o Compartilhamento de projetos em um modelo de projeto para conceder acesso automaticamente aos projetos criados usando esse modelo.

**Veja o porquê**

O acesso a projetos específicos é concedido através do próprio projeto. Se o mesmo grupo de pessoas sempre precisar acessar projetos criados com um modelo específico, adicione-os sob a opção Compartilhamento de projeto no modelo. Você não só pode controlar o acesso a projetos assim que eles são criados, como também simplifica os esforços de escalabilidade se as permissões precisarem ser alteradas no futuro.

**Observação**: O Compartilhamento de modelo concede acesso ao próprio modelo. Um usuário deve ter pelo menos permissões de Exibição para fazer projetos com o modelo.

</br>
</br>

**Prática recomendada**

Atribuir funções ou equipes a tarefas, não a indivíduos.

**Veja o porquê**

Quando um usuário individual alterar posições ou sair da organização, você terá que atualizar manualmente os modelos de projeto que incluem essa pessoa. Isso leva tempo em parte dos administradores de sistema ou grupo ou gerentes de projeto.

Se você usar funções de trabalho ou equipes em modelos, as alterações de pessoal não terão um efeito direto nos modelos do projeto porque qualquer pessoa que tenha atribuído essa função de trabalho ou nessa equipe poderá receber o trabalho. Isso ajuda a garantir que o trabalho não escorregue pelas fendas. As atribuições de função de trabalho também facilitam a atribuição de trabalho a usuários individuais, pois o Workfront pode mostrar uma lista de pessoas que atribuíram essa função de trabalho.

Além disso, as funções de trabalho são usadas pelas ferramentas de planejamento de recursos da Workfront para ajudar você a calcular os recursos necessários e a planejar o trabalho futuro.

</br>
</br>

**Prática recomendada**

Evite ser muito granular ao criar tarefas em um modelo de projeto. Limite o número de tarefas em um modelo de projeto para as necessárias para concluir o trabalho.

**Veja o porquê**

Modelos de projeto muito complicados resultam em uma experiência ruim para os usuários — gerentes de projeto, gerentes de recursos, membros da equipe e muito mais. Muitas tarefas dificultam o gerenciamento da linha do tempo do projeto, com prazos de tarefas sobrepostos e várias tarefas atribuídas às mesmas funções de trabalho ou indivíduos.


</br>
</br>

**Prática recomendada**

Use a descrição da tarefa para capturar as pequenas etapas da tarefa, em vez de dividi-la em várias tarefas.

**Veja o porquê**

Se várias tarefas em uma linha forem atribuídas à mesma função de trabalho/indivíduo, isso indica que essas tarefas podem ser combinadas. Ter muitas tarefas atribuídas a um usuário pode fazer com que ele sinta que há mais trabalho a ser concluído, o que pode afetar a adoção do Workfront.

</br>
</br>

**Prática recomendada**

Certifique-se de que as tarefas do modelo incluam durações de tarefas, horas planejadas e antecessores.

**Veja o porquê**

Essas três coisas — durações, horas planejadas e antecessores — são os elementos fundamentais da linha do tempo do projeto. Estas são as chaves para saber quanto tempo irá demorar e quando terá de ser feito. As ferramentas de gerenciamento de recursos da Workfront durações e horas planejadas, além de atribuições de funções de trabalho, para calcular a capacidade dos recursos, a disponibilidade e muito mais.

Se não tiver certeza sobre como estimar as durações ou as horas planejadas pela primeira vez, trabalhe com a equipe do projeto para definir algumas estimativas iniciais. Depois de usar o modelo, consulte a equipe do projeto novamente para determinar onde as alterações podem ser feitas para tornar o modelo mais preciso. Se os usuários estiverem fazendo logon no Workfront, você poderá comparar as horas planejadas de um projeto com as horas reais para ver onde os ajustes são necessários.


</br>
</br>

**Prática recomendada**

Pré-configurar os detalhes do projeto e anexar formulários personalizados ao modelo.

**Veja o porquê**

Verifique se as informações padrão para todos os projetos estão preenchidas no modelo do projeto. Isso não apenas ajuda a acelerar a criação de projetos, como também garante que as informações necessárias estejam lá e sejam consistentes em todos os projetos.

Anexe formulários personalizados de projeto que correspondem a formulários personalizados de solicitação para obter informações enviadas ao converter a solicitação em um projeto usando o modelo.

</br>
</br>

**Prática recomendada**

Revise e atualize regularmente modelos de projeto.

**Veja o porquê**

À medida que processos e equipes mudam, os modelos de projeto devem ser atualizados. Estabeleça uma cadência regular, como trimestral, para verificar quais modelos não estão sendo usados ativamente. Você pode desativá-los, portanto eles ainda estão no Workfront, mas não serão exibidos nas listas de seleção de modelo.

</br>
</br>

**Prática recomendada**

Verifique os modelos para garantir que eles tenham todas as informações necessárias antes de compartilhá-los e que outros comecem a usá-los.


**Veja o porquê**

Como os modelos serão usados repetidas vezes para criar projetos, você deve certificar-se de que tudo esteja configurado corretamente e completamente. Isso leva à consistência em todos os projetos e a dados precisos para relatórios.

Além das configurações de tarefa, como duração e horas planejadas, algumas coisas a serem revisadas antes de compartilhar modelos incluem:

* Configurar Agendar de
* Restrições de tarefa
* Proprietário do projeto, patrocinador, grupo e empresa
* Portfolio e programa
* Caminho e etapas do marco
* Processos de aprovação
* Certifique-se de que os usuários que atribuem tarefas aos projetos tenham acesso ao Contribute para o projeto
* Conjunto de recursos
* Notificações de lembrete
* Cronograma
* Configuração da moeda (se aplicável)
* Anexar documentos padrão
* Anexar os formulários aduaneiros necessários
* Verifique a equipe do projeto para garantir que não haja mais pessoas atribuídas

</br>
</br>

**Prática recomendada**

Ao ajustar a opção Programar de em um modelo, revise e atualize as restrições de tarefa.

**Veja o porquê**

Misturar diferentes restrições de tarefa em um projeto pode causar cálculos de data planejada inesperados e confusos. Por exemplo, quando a Data inicial é selecionada para a opção Agendar de , qualquer tarefa criada nesse projeto recebe a restrição de tarefa Assim que possível por padrão. Posteriormente, se você alternar a opção Agendar de para Data de conclusão, qualquer tarefa criada terá uma restrição de tarefa O Mais Tarde Possível por padrão. Ter uma combinação não intencional de tarefas com cada uma dessas restrições pode resultar em datas planejadas confusas na linha do tempo do projeto.


</br>
</br>

**Prática recomendada**

Verifique a equipe do projeto no modelo e remova os usuários que não estarão trabalhando com o projeto.

**Veja o porquê**

Ao criar um modelo a partir de um projeto existente, ele mostra as pessoas às quais foram atribuídas tarefas/problemas no projeto. E, à medida que trabalha com o modelo, você pode remover pessoas às quais foi atribuído anteriormente trabalho ou alterar uma atribuição que você fez no modelo.

Todos esses usuários serão listados como parte da equipe do projeto, nas seções Pessoas e Agendamento do projeto. Como resultado, eles serão propagados para todos os projetos criados a partir desse template. Isso pode causar confusão para o usuário, pois como parte da equipe do projeto, ele recebe notificações sobre a atividade no projeto, vê o projeto na lista Projetos em que estou, e obtém permissões para o projeto e suas tarefas, problemas e documentos.
