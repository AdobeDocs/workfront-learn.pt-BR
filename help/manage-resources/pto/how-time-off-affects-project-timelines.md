---
title: Mostrar como a folga afeta os cronogramas do projeto
description: Veja o que acontece com o cronograma de um projeto quando a configuração de folgas está ativada ou desativada.
feature: Resource Management
type: Tutorial
role: Leader, User
level: Intermediate, Experienced
activity: use
team: Technical Marketing
jira: KT-10180
exl-id: 0f79dd8d-b7ce-4ee9-b211-23c8ed5d497c
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 100%

---

# Como as folgas afetam os cronogramas do projeto

Se as folgas atribuídas a um usuário serão levadas em consideração no cronograma do projeto é algo que depende de uma configuração do projeto chamada [!UICONTROL Folgas do usuário]. Essa configuração determina se as folgas do responsável principal da tarefa ajustam as datas planejadas para essa tarefa no projeto.

Vamos ver o que acontece com o cronograma de um projeto quando cada uma das configurações é selecionada: [!UICONTROL Considerar as folgas do usuário nas durações das tarefas] ou [!UICONTROL Ignorar as folgas do usuário nas durações das tarefas].

![Configuração das folgas do usuário](assets/toapt_01.png)

## Leve em conta o tempo de folga do usuário nas durações de tarefas

Esta opção é a configuração padrão do Workfront.

Neste exemplo, o principal responsável pela tarefa tem dias de folga marcados em seu calendário pessoal.

![calendário pessoal](assets/toapt_02.png)

O gerente de projetos deseja atribuir essa pessoa a uma tarefa que tenha datas planejadas que se sobreponham às folgas do usuário.

![tarefa do projeto com datas](assets/toapt_03.png)

Quando este usuário for atribuído à tarefa, as datas planejadas serão ajustadas automaticamente. Agora, a data planejada de conclusão da tarefa foi prorrogada por vários dias para acomodar as folgas do usuário. É importante observar que essa alteração pode afetar as datas planejadas de outras tarefas do projeto e, potencialmente, a data planejada de conclusão do projeto.

![tarefa do projeto com data de vencimento](assets/toapt_04.png)

## [!UICONTROL Ignorar o tempo de folga do usuário nas durações de tarefas]

Com esta opção, as datas planejadas da tarefa permanecem conforme planejadas originalmente, mesmo que o responsável principal esteja de folga durante essa tarefa.

O membro da equipe tem dias de folga marcados no calendário.

![calendário de folgas com datas marcadas](assets/toapt_05.png)

A pessoa repsonsável pela gerência de projetos atribui a usuários tarefas que se sobrepõem às folgas. Depois que usuário são atribuídos, as datas planejadas da tarefa permanecem como planejadas originalmente.

![ajustar datas de tarefas do projeto](assets/toapt_06.png)

Para garantir que o trabalho seja concluído a tempo, pode ser útil atribuir outra pessoa que possa trabalhar na tarefa enquanto a pessoa responsável original estiver fora do escritório.

## Ajustar a configuração na camada do projeto

Para alterar a configuração das folgas do usuário em um projeto:

* Abra o projeto clicando no nome no Workfront.

* Selecione [!UICONTROL Editar] no menu de três pontos, no cabeçalho da página, à direita do nome do projeto.

* Role até a seção [!UICONTROL Configurações do projeto] e encontre o campo [!UICONTROL Folgas do usuário].

* Selecione a opção que deseja aplicar a este projeto: [!UICONTROL Considerar as folgas do usuário nas durações das tarefas] ou [!UICONTROL Ignorar as folgas do usuário nas durações das tarefas].

* Clique no botão [!UICONTROL Salvar], no canto superior direito da janela.

![Leve em conta o tempo de folga do usuário nas durações de tarefas](assets/toapt_07.png)


**Observação**: esta configuração não está disponível quando você seleciona [!UICONTROL Detalhes do projeto] no menu do painel esquerdo da página do projeto.

Existe uma configuração global para isso nas preferências do projeto, no menu [!UICONTROL  Configuração]. Esta configuração é gerenciada pelo administrador do sistema. Os administradores de grupos podem conseguir ajustar esta configuração para os grupos que gerenciam.

O Workfront recomenda que a configuração seja definida de acordo com a forma que você deseja que a maioria dos seus projetos lidem com as folgas na sua organização.

A configuração também pode ser incorporada a modelos de projeto por meio dos detalhes do modelo.
