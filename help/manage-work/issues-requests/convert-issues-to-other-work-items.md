---
title: Converter um problema/solicitação em uma tarefa
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
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# Converter um problema/solicitação em uma tarefa

Um problema pode ser suficientemente significativo para que o tempo e o esforço para resolvê-lo precisem ser contabilizados na linha do tempo do projeto e alocar os recursos apropriados. Nesse caso, o problema pode ser convertido em uma tarefa.

![Uma imagem do [!UICONTROL Converter em Tarefa] opção de um problema no [!UICONTROL Workfront].](assets/15-convert-issue-to-task-menu-option.png)

1. Navegue até a [!UICONTROL Problemas] seção do projeto ou tarefa na qual o problema está conectado. Ou encontre o problema em um relatório ao qual você tenha acesso.
1. Clique no nome do problema para abri-lo.
1. No menu de 3 pontos à direita do nome do problema, selecione **[!UICONTROL Converter em tarefa]**.
1. Preencha o [!UICONTROL Converter em tarefa] formulário. Comece dando um nome e uma descrição à nova tarefa.
1. Se a nova tarefa precisar fazer parte de um projeto diferente, altere a variável [!UICONTROL Projeto de destino] nome.
1. No [!UICONTROL Opções] marque as caixas para manter o problema original, permitir acesso à nova tarefa e manter a data de conclusão. Siga o fluxo de trabalho da sua organização ao fazer essas seleções.
1. Anexe um formulário personalizado se quiser transferir dados de formulário personalizados do problema para a tarefa. (Todos os campos existentes no formulário de problema e no formulário de tarefa serão transferidos automaticamente para o formulário de tarefa.)
1. Clique em **[!UICONTROL Converter em tarefa]** para terminar.

![Uma imagem do [!UICONTROL Converter em Tarefa] forma de um problema no [!UICONTROL Workfront].](assets/16-convert-to-task-options.png)

Dependendo da organização [!DNL Workfront] configurações do sistema, você pode ou não conseguir alterar as configurações na seção Opções quando estiver convertendo a tarefa. Essas opções afetam o problema original e a nova tarefa.

* **Conservar o problema original e vincular a sua resolução a esta tarefa** retém o problema original e informações relacionadas (horas, documentos, etc.). Com essa opção selecionada, quando a tarefa for concluída, o problema será marcado como resolvido. Se essa opção for **não** selecionado, o problema original será excluído na criação da tarefa. Isso pode afetar como sua organização rastreia e relata problemas.
* A variável **Permitir que (nome de usuário) tenha acesso a esta tarefa** Esta opção permitirá que a pessoa que criou o problema tenha acesso a esta nova tarefa.
* A variável **Manter a data de conclusão planejada do problema** permite manter a data de conclusão planejada já definida no problema. Isso define a restrição da tarefa como [!UICONTROL Não Terminar Depois De]. Se a caixa estiver desmarcada, as datas da tarefa serão definidas como se uma nova tarefa fosse criada dentro do projeto.

A nova tarefa é colocada na parte inferior da lista de tarefas do projeto. Mova a tarefa para o local desejado, atribua um usuário ou equipe ao trabalho, adicione horas e duração planejadas, etc.

>[!NOTE]
>
>Não é possível adicionar problemas à linha do tempo do projeto, pois eles representam &quot;trabalho não planejado&quot;. A linha do tempo do projeto é para &quot;trabalho planejado&quot;, o que significa tarefas.


