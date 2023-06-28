---
title: Mostrar folga afeta os cronogramas do projeto
description: Veja o que acontece com a linha do tempo de um projeto quando a configuração de tempo livre está ativada ou desativada.
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
ht-degree: 4%

---

# Como a folga afeta as linhas do tempo do projeto

Se os fatores de folga de um usuário atribuído na linha do tempo do projeto dependem de uma configuração de projeto chamada [!UICONTROL Tempo de folga do usuário]. Esta configuração determina se o tempo de folga do responsável principal da tarefa ajusta as datas planejadas para essa tarefa no projeto.

Vamos ver o que acontece com uma linha do tempo de projeto quando cada uma das configurações é selecionada - C[!UICONTROL Considerar o tempo de folga do usuário nas durações de tarefas] ou [!UICONTROL Ignorar o tempo de folga do usuário nas durações de tarefas].

![Configuração de tempo de folga do usuário](assets/toapt_01.png)

## Leve em conta o tempo de folga do usuário nas durações de tarefas

Essa opção é a configuração padrão do Workfront.

Neste exemplo, o principal responsável pela tarefa tem dias de folga marcados em seu calendário pessoal.

![calendário pessoal](assets/toapt_02.png)

O gerente de projeto deseja atribuir essa pessoa a uma tarefa que tenha datas planejadas que se sobreponham ao tempo de folga do usuário.

![tarefa de projeto com datas](assets/toapt_03.png)

Quando este usuário é atribuído à tarefa, as datas planejadas se ajustam automaticamente. Agora, a data planejada de conclusão da tarefa foi estendida por vários dias para acomodar o tempo de folga do usuário. É importante observar que essa alteração pode afetar as datas planejadas de outras tarefas no projeto e, possivelmente, a data planejada de conclusão do projeto.

![tarefa de projeto com data de vencimento](assets/toapt_04.png)

## [!UICONTROL Ignorar o tempo de folga do usuário nas durações de tarefas]

Com essa opção, as datas planejadas da tarefa permanecem como planejadas originalmente, mesmo que o destinatário principal tenha uma folga durante a duração dessa tarefa.

O membro da equipe tem dias de folga marcados em seu calendário.

![calendário de fotos com datas marcadas](assets/toapt_05.png)

O gerente de projeto atribui a eles uma tarefa que se sobrepõe ao tempo de folga. Depois que o usuário é atribuído, as datas planejadas da tarefa permanecem como planejadas originalmente.

![ajustar datas de tarefas do projeto](assets/toapt_06.png)

Para garantir que o trabalho seja concluído a tempo, pode ser útil atribuir outra pessoa que possa trabalhar na tarefa enquanto o responsável original estiver fora do escritório.

## Ajustar a configuração no nível do projeto

Para alterar a configuração Tempo livre do usuário em um projeto:

* Abra o projeto clicando no seu nome na Workfront.

* Selecionar [!UICONTROL Editar] no menu de 3 pontos no cabeçalho da página, à direita do nome do projeto.

* Role para a [!UICONTROL Configurações do projeto] e localize a [!UICONTROL Tempo de folga do usuário] campo.

* Selecione a opção que deseja aplicar a esse projeto — [!UICONTROL Considerar o tempo de folga do usuário nas durações de tarefas] ou I[!UICONTROL ignorar o tempo de folga do usuário nas durações de tarefas].

* Clique em [!UICONTROL Salvar] no canto superior direito da janela.

![Leve em conta o tempo de folga do usuário nas durações de tarefas](assets/toapt_07.png)


**Nota**: essa configuração não está disponível ao selecionar [!UICONTROL Detalhes do projeto] no menu do painel esquerdo da página do projeto.

Existe uma configuração global para isso nas preferências do projeto no [!UICONTROL Configuração] menu. Essa configuração é gerenciada pelo administrador do sistema. Os administradores de grupo podem conseguir ajustar essa configuração para os grupos que gerenciam.

A Workfront recomenda que a configuração seja definida da maneira que você deseja que a maioria dos projetos trate o tempo livre em sua organização.

A configuração também pode ser incorporada a modelos de projeto, por meio dos detalhes do modelo.
