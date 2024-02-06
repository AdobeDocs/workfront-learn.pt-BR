---
title: Converter um problema ou solicitação em uma tarefa
description: Saiba como converter problemas em outros itens de trabalho.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: convert-issues-to-other-work-items.jpeg
type: Tutorial
role: User
level: Intermediate
jira: KT-10069
exl-id: 1fd4d862-e44b-4c50-9663-70e727f6e9b7
source-git-commit: 060ceb14d274e8b2ad080c1f58290a2c5769e007
workflow-type: ht
source-wordcount: '485'
ht-degree: 100%

---

# Converter um problema ou solicitação em uma tarefa

Há casos onde um problema é relevante o suficiente para que o tempo e esforço necessário para resolvê-lo precisem ser considerados no cronograma do projeto e recursos apropriados precisem ser alocados. Nestes casos, o problema pode ser convertido em uma tarefa.

![Imagem da opção [!UICONTROL Converter em tarefa] de um problema no [!UICONTROL Workfront].](assets/15-convert-issue-to-task-menu-option.png)

1. Acesse a seção [!UICONTROL Problemas] do projeto ou tarefa no qual o problema está registrado. Ou encontre o problema em um relatório ao qual você tenha acesso.
1. Clique no nome do problema para abri-lo.
1. No menu de três pontos à direita do nome do problema, selecione **[!UICONTROL Converter em tarefa]**.
1. Preencha o formulário [!UICONTROL Converter em tarefa]. Comece fornecendo um nome e uma descrição à nova tarefa.
1. Se a nova tarefa precisar fazer parte de um projeto diferente, altere o nome do [!UICONTROL Projeto de destino].
1. Na seção [!UICONTROL Opções], marque as caixas para manter o problema original, permitir acesso à nova tarefa e manter a data de conclusão. Siga o fluxo de trabalho da sua organização ao fazer essas seleções.
1. Anexe um formulário personalizado se desejar transferir dados de formulário personalizado do problema para a tarefa. (Todos os campos existentes no formulário do problema e da tarefa serão transferidos automaticamente para o formulário da tarefa.)
1. Clique em **[!UICONTROL Converter em tarefa]** para terminar.

![Imagem do formulário [!UICONTROL Converter em Tarefa] de um problema no [!UICONTROL Workfront].](assets/16-convert-to-task-options.png)

Dependendo das configurações do [!DNL Workfront] da sua organização, você pode ou não conseguir alterar as configurações na seção Opções ao converter a tarefa. Essas opções afetam o problema original e a nova tarefa.

* A opção **Manter o problema original e vincular sua resolução a esta tarefa** retém o problema original e as informações relacionadas (horas, documentos etc.). Se esta opção estiver selecionada quando a tarefa for concluída, o problema será marcado como resolvido. Se esta opção **não** estiver selecionada, o problema original será excluído ao criar a tarefa. Isso pode afetar como sua organização acompanha e relata problemas.
* A opção **Permitir que (nome de usuário) tenha acesso a esta tarefa** autorizará a pessoa que criou o problema a acessar esta nova tarefa.
* A opção **Manter a data de conclusão planejada do problema** permite manter a data de conclusão planejada já definida no problema. Isso define a restrição da tarefa como [!UICONTROL Finalizar no máximo até]. Se a caixa estiver desmarcada, as datas da tarefa serão definidas como se uma nova tarefa fosse criada dentro do projeto.

A nova tarefa é colocada na parte inferior da lista de tarefas do projeto. Mova a tarefa para o local desejado, atribua um usuário ou equipe ao trabalho, adicione horas e duração planejadas etc.

>[!NOTE]
>
>Você não pode adicionar problemas à linha do tempo do projeto, pois eles representam um “trabalho não planejado”. A linha do tempo do projeto é destinada a “trabalhos planejados”, ou seja, tarefas.


