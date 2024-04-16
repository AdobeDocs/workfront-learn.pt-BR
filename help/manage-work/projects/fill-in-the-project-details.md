---
title: Preencha os detalhes do projeto
description: Saiba quais são os 12 campos de detalhes do projeto que o  [!DNL  Workfront]  recomenda que você preencha ao criar um projeto.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: fill-in-the-project-details.jpeg
type: Tutorial
role: User
level: Beginner
recommendations: noDisplay,noCatalog
jira: KT-10140
exl-id: a62b9421-627a-4f23-ab66-da1f29114225
source-git-commit: c2ba2ddfbbc642398a0136ecbf7c3613208080c4
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Preencha os detalhes do projeto

Não se preocupe. Você não precisa preencher todos os campos e caixas de seleção nos detalhes do projeto com cada projeto criado no [!DNL  Workfront]. Use modelos para preencher previamente as informações e, em seguida, dê atenção aos 12 campos de detalhes do projeto mais importantes listados abaixo.

1. **Nome**

   Um nome de projeto descritivo ajuda todos a identificar o propósito do projeto. Certifique-se de seguir a convenção de nomeação de projeto da sua organização, que pode exigir que determinadas informações sejam incluídas no nome do projeto (como número de referência, nome do departamento ou indicador de categoria).


1. **Descrição**

   Quando várias pessoas trabalham em um projeto, você, como gerente de projeto, precisa garantir que todos estejam atualizados com a finalidade e as expectativas do projeto.

   Faça isso com uma descrição do projeto que forneça informações básicas, responda a perguntas e permita que a equipe do projeto avance no trabalho. Por exemplo, “Uma campanha destinada a aumentar o trabalho gerador de receitas em 50%” ou “Nova atualização do sistema para melhorar a eficiência em todo o departamento”.

   Alguns clientes do Workfront incluem uma amostra de como dever ser uma descrição de projeto em seus modelos de projeto.

1. **Status**

   O status é usado no Workfront para indicar onde, ou em que estágio, do fluxo de trabalho um projeto está. O status é usado em muitos relatórios do Workfront para rastrear o progresso do trabalho.

   O Workfront recomenda que o status seja definido como Planejamento enquanto você desenvolve e finaliza o plano do projeto. O principal aspecto do status Planejamento é que as notificações do Workfront não são enviadas aos responsáveis pela tarefa do projeto enquanto ele estiver com esse status.

   Então, quando o projeto estiver pronto para entrar em operação, altere o status para Atual. Isso permite que o Workfront envie notificações às pessoas sobre novas tarefas às quais estão atribuídas, mas não as enviará aos usuários sobre as tarefas às quais foram atribuídos enquanto o projeto estava no status de Planejamento.

   >[!TIP]
   >
   >  Ao fazer alterações no projeto, como datas de vencimento, você pode reverter o status para Planejamento ou desativar o recurso Salvamento automático para evitar que notificações sejam enviadas até que as alterações sejam concluídas.

   O status de Planejamento pode ser definido como padrão global do Workfront para novos projetos pelo administrador do sistema.

1. **Modo de cronograma**

   Os projetos do Workfront podem ser agendados a partir de uma data inicial ou de conclusão. Essa seleção importante determina como as datas planejadas de cada tarefa são calculadas.

   A opção Data inicial utiliza a data de início do projeto (inserida por você) e a duração e os antecessores de cada tarefa para calcular quando o projeto será concluído. O Workfront recomenda usar essa opção, pois é a mais comum e facilita o planejamento das datas dos projetos.

   No entanto, você pode usar uma data de conclusão. O Workfront analisa a data final (inserida por você) e o trabalho a ser realizado (com base nas durações e antecessores) e, em seguida, trabalha de trás para frente para calcular a data de início do projeto. O Workfront recomenda aguardar para usar a data de conclusão após um determinado nível de proficiência no Workfront ter sido estabelecido.

   Seja qual for a opção escolhida, não se esqueça de selecionar uma data no calendário pop-up.

   A opção Modo Cronograma pode ser definida no modelo.

1. **Grupo**

   Um grupo é uma unidade organizacional do Workfront que geralmente se alinha a um departamento. Esse campo pode ser definido no modelo de projeto. Caso contrário, o campo será automaticamente definido como o Grupo local da pessoa que criou o projeto. Você pode alterar o grupo conforme necessário.

   Geralmente, a maioria das pessoas que trabalha no projeto vem desse grupo. Mas isso não impede que pessoas de outros grupos sejam designadas para trabalhar no projeto.

   O Grupo no projeto também determina quais preferências de projeto, tarefa e problemas o projeto usará. Essas preferências, como um status personalizado para um grupo específico, são definidas pelo administrador do sistema ou administrador de grupo.

   A configuração do grupo é uma maneira conveniente, por meio de relatórios, de mostrar todos os projetos em que um departamento está trabalhando.

1. **Proprietário do projeto**

   Proprietário do projeto é o termo do Workfront para gerente de projeto. Essa é a pessoa responsável pelo planejamento e/ou gerenciamento do projeto.

   Para que o Proprietário do projeto tenha permissões totais de gerenciamento do projeto, ele deve ter uma licença do Plano.

   Normalmente esse campo fica em branco no modelo e é preenchido automaticamente com o nome de quem cria o projeto. Se um nome for inserido no modelo, esse será o proprietário padrão do projeto.

1. **Patrocinador do projeto**

   O Patrocinador do projeto não é obrigatório, mas, quando usado, geralmente é a pessoa que solicitou o projeto. Muitas vezes, trata-se de uma parte interessada interna, como um gerente ou executivo, com responsabilidade geral pelo projeto.

   O patrocinador recebe automaticamente permissões de visualização do projeto e deve ser um usuário licenciado do Workfront.

   O Patrocinador do projeto pode ser definido no modelo.

1. **Gerenciador de Recursos**

   Os usuários do Workfront listados nesse campo podem usar as ferramentas de planejamento e gerenciamento de recursos do Workfront para os projetos específicos em que estão listados. Até 30 nomes podem ser listados no campo Gerenciador de recursos, e cada um deve ter uma licença de plano.

   O campo Gerenciador de recursos pode ser definido no modelo.

1. **Formulários personalizados**

   O Workfront fornece campos nativos para itens como nome do projeto e data inicial. Mas há informações adicionais de que você precisa como gerente de projeto ou que a equipe do projeto precisará. Seus dados exclusivos são igualmente importantes e podem ser facilmente armazenados nesses formulários. Detalhes como datas de publicação, tamanhos de ativos de impressão, canais de entrega etc.

   Os formulários personalizados podem capturar essas informações e ser incluídos em listas e relatórios no Workfront, facilitando a visualização e a edição das informações.

   Formulários personalizados podem ser anexados aos seus modelos antecipadamente.

1. **Agendar**

   O trabalho acontece 24 horas por dia, já que muitas empresas têm funcionários em todo o mundo.

   O Workfront permite que você aplique um cronograma comum aos projetos. Eles são criados pela pessoa responsável pela administração do sistema. Os cronogramas refletem os dias e horários de trabalho das suas equipes, além dos dias em que os funcionários não estarão trabalhando (como feriados).

   Como pessoa responsável pelo planejamento, certifique-se de aplicar o cronograma certo ao projeto certo. As configurações de cronograma afetam os cálculos da linha do tempo, levando em consideração as folgas e os fusos horários.

   O cronograma atribuído ao projeto deve ser aquele que se aplica à maioria dos destinatários das tarefas. Se não houver um cronograma especificado para o projeto, o cronograma marcado como Padrão será usado.

   O cronograma pode ser definido no modelo.

1. **Conjuntos de Recursos**

   Conjuntos de recursos são coleções de usuários do Workfront necessários ao mesmo tempo para a conclusão de projetos em sua organização. Um conjunto de recursos pode ser atribuído a vários projetos, o que significa que você tem projetos competindo por recursos.

   Ter conjuntos de recursos atribuídos a um projeto é um pré-requisito para a utilização do Planejador de recursos e outras ferramentas de gerenciamento de recursos no Workfront.

   Um conjunto de recursos padrão pode ser definido no modelo.

1. **Acesso ao projeto para visualizadores e colaboradores**

   Quando alguém recebe acesso a um projeto por meio de compartilhamento, há três níveis de permissões que podem ser concedidos: Visualizar, Contribuir e Gerenciar. Cada nível de permissão permite que o usuário veja e faça determinadas coisas no projeto.

   Por exemplo, há pessoas que podem ter acesso ao projeto, mas não deveriam ver as informações financeiras. Portanto, você pode desativar a opção Visualizar finanças para eles.

   As configurações de acesso podem ser definidas no modelo.

## Tutoriais recomendados sobre este tópico

* [Entender a criação básica de projetos](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/manage-work/projects/understand-basic-project-creation)
* [Navegar na página do projeto](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/manage-work/projects/navigate-the-project-page)
* [Aprenda quatro maneiras de criar um projeto](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/manage-work/projects/understand-other-ways-to-create-projects)
* [Introdução ao planejamento de um projeto](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/manage-work/projects/getting-started-plan-a-project)
