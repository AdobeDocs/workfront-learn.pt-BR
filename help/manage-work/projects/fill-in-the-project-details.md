---
title: Preencha os detalhes do projeto
description: Saiba quais são os 12 campos de detalhes do projeto [!DNL  Workfront] A recomenda que você preencha ao criar um projeto.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: fill-in-the-project-details.jpeg
type: Tutorial
role: User
level: Intermediate
jira: KT-10140
exl-id: a62b9421-627a-4f23-ab66-da1f29114225
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1219'
ht-degree: 1%

---

# Preencha os detalhes do projeto

Não se preocupe... você não precisa preencher cada campo e caixa de seleção nos detalhes do projeto com cada projeto criado no [!DNL  Workfront]. Use modelos para preencher previamente as informações e, em seguida, vire sua atenção para os 12 campos de detalhes mais importantes do projeto listados abaixo.

1. **Nome**

   Um nome de projeto descritivo ajuda todos a identificar a finalidade do projeto. Siga a convenção de nomenclatura de projeto de sua organização, que pode exigir que determinadas informações sejam incluídas no nome do projeto (como um número de referência, nome de departamento ou indicador de categoria).


1. **Descrição**

   Quando várias pessoas trabalham em um projeto, você, como gerente de projeto, precisa garantir que todos estejam atualizados com a finalidade e as expectativas do projeto.

   Faça isso com uma descrição do projeto que forneça informações básicas, responda perguntas e permita que a equipe do projeto avance com seu trabalho. Por exemplo, &quot;Uma campanha com o objetivo de aumentar a receita gerando trabalho em 50%&quot; ou &quot;Nova atualização do sistema para melhorar a eficiência em todo o departamento&quot;.

   Alguns clientes do Workfront incluem uma amostra do que uma descrição de projeto deve parecer em seus modelos de projeto.

1. **Status**

   O status é usado no Workfront para indicar onde ou em que estágio um projeto está no fluxo de trabalho. O status é usado em muitos relatórios do Workfront para rastrear o progresso do trabalho.

   A Workfront recomenda que o status seja definido como Planejamento enquanto você estiver concluindo o plano do projeto. O ponto principal do status de Planejamento é que as notificações do Workfront não são enviadas para os atribuídos da tarefa sobre o projeto enquanto ele estiver nesse status.

   Em seguida, quando o projeto estiver pronto para entrar no ar, altere o status para Current (Atual). Isso permite que o Workfront envie notificações às pessoas sobre novas tarefas às quais estão atribuídas, mas não enviará notificações aos usuários sobre as tarefas às quais foram atribuídas enquanto o projeto estava no status de Planejamento.

   >[!TIP]
   >
   >  Ao fazer alterações no projeto, como alterar datas de vencimento, você pode reverter o status para o Planning ou desativar o recurso de Salvamento Automático para impedir que as notificações sejam enviadas até que as alterações sejam concluídas.

   O status do Planning pode ser definido como o padrão global do Workfront para novos projetos pelo administrador do sistema.

1. **Modo de Cronograma**

   Os projetos da Workfront podem ser agendados a partir de uma data de início ou de uma data de conclusão. Essa seleção importante determina como as datas planejadas de cada tarefa são calculadas.

   A opção Data inicial usa a data de início do projeto—inserida por você—e a duração de cada tarefa e predecessoras para calcular quando o projeto será concluído. A Workfront recomenda usar essa opção, pois é a mais comum e facilita o planejamento das datas do projeto.

   No entanto, você pode usar uma data de conclusão. O Workfront verifica a data de término (inserida por você) e o trabalho a ser concluído (com base nas durações e predecessores) e, em seguida, trabalha de forma retroativa para calcular a data de início do projeto. A Workfront recomenda aguardar a data de conclusão após o estabelecimento de um certo nível de proficiência no Workfront.

   Seja qual for a opção escolhida, não se esqueça de selecionar uma data no calendário pop-up.

   A opção Schedule Mode pode ser definida no template.

1. **Grupo**

   Um grupo é uma unidade organizacional da Workfront que geralmente se alinha a um departamento. Este campo pode ser definido no modelo de projeto. Caso contrário, o campo é automaticamente definido para o Grupo inicial da pessoa que está criando o projeto. Você pode alterar o grupo conforme necessário.

   Geralmente, a maioria das pessoas que trabalham no projeto vem desse grupo. Mas isso não restringe as pessoas de outros grupos que recebem trabalho no projeto.

   O Grupo no projeto também determina quais preferências de projeto, tarefa e problema o projeto usará. Essas preferências, como um status personalizado para um grupo específico, são definidas pelo administrador do sistema ou de grupo.

   A configuração do grupo é uma maneira conveniente, por meio de relatórios, de mostrar todos os projetos em que um departamento está trabalhando.

1. **Proprietário do projeto**

   O Proprietário do projeto é o termo da Workfront para gerente de projeto. Essa é a pessoa responsável pelo planejamento e/ou gestão do projeto.

   Para que o Proprietário do Projeto tenha permissões de gerenciamento completas para o projeto, ele deve ter uma licença de Plano.

   Normalmente, esse campo é deixado em branco no modelo e é preenchido automaticamente com o nome da pessoa que cria o projeto. Se um nome for inserido no modelo, esse será o proprietário padrão do projeto.

1. **Patrocinador do projeto**

   O Patrocinador do projeto não é necessário, mas, quando usado, geralmente é a pessoa que solicitou o projeto. Muitas vezes, trata-se de uma parte interessada interna, como um gerente ou executivo, com responsabilidade geral pelo projeto.

   O patrocinador recebe automaticamente permissões de exibição para o projeto e deve ser um usuário licenciado pela Workfront.

   O Patrocinador do projeto pode ser definido no modelo.

1. **Gerenciador de Recursos**

   Os usuários do Workfront listados neste campo podem usar as ferramentas de planejamento e gerenciamento de recursos do Workfront para o(s) projeto(s) específico(s) no(s) qual(is) estão listados. Até 30 nomes podem ser listados no campo Gerenciador de recursos, e cada um deve ter uma licença de plano.

   O campo Gerenciador de recursos pode ser definido no modelo.

1. **Formulários personalizados**

   O Workfront fornece campos nativos para itens como nome do projeto e data de início. Mas há informações adicionais que você precisa como gerente de projeto ou que a equipe de projeto precisará. Seus dados exclusivos são igualmente importantes e podem ser facilmente armazenados nesses formulários. Detalhes como datas de publicação, tamanhos de ativos de impressão, canais de entrega etc.

   Os formulários personalizados podem capturar essas informações e podem ser incluídos em listas e relatórios no Workfront, facilitando a visualização e a edição das informações.

   Formulários personalizados podem ser anexados aos seus modelos antecipadamente.

1. **Agendar**

   O trabalho acontece 24 horas por dia, à medida que muitas empresas têm funcionários em todo o mundo.

   O Workfront permite aplicar um agendamento comum aos projetos. Eles são criados pelo administrador do sistema. Os cronogramas refletem os dias e horas de trabalho de suas equipes, além de dias em que os funcionários não estarão trabalhando (como feriados).

   Como planejador, certifique-se de aplicar o cronograma correto ao projeto correto. As configurações de programação afetam os cálculos da linha do tempo, levando em conta as folgas e os fusos horários.

   O cronograma atribuído ao projeto deve ser o que se aplica à maioria dos atribuídos da tarefa. Se não houver cronograma especificado para o projeto, o cronograma marcado como Padrão será usado.

   O agendamento pode ser definido no template.

1. **Conjuntos de Recursos**

   Conjuntos de recursos são coleções de usuários do Workfront que são necessárias ao mesmo tempo para a conclusão de projetos em sua organização. Um conjunto de recursos pode ser atribuído a vários projetos, o que significa que você tem projetos competindo por recursos.

   Ter conjuntos de recursos atribuídos a um projeto é um pré-requisito para o uso do Planejador de recursos e outras ferramentas de gerenciamento de recursos no Workfront.

   Um conjunto de recursos padrão pode ser definido no modelo.

1. **Acesso ao projeto para visualizadores e colaboradores**

   Quando alguém recebe acesso a um projeto por meio do Compartilhamento, há três níveis de permissões que eles podem receber — Exibir, Contribute e Gerenciar. Cada nível de permissão permite que o usuário veja e faça determinadas coisas com o projeto.

   Por exemplo, há pessoas que podem ter acesso ao projeto, mas não devem ver as informações financeiras. Para que você possa desativar a opção Exibir finanças para eles.

   As configurações de acesso podem ser definidas no template.
