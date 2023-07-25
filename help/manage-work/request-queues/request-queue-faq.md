---
title: Respostas a perguntas comuns sobre filas de solicitações
description: Obtenha respostas para perguntas comuns sobre filas de solicitações no [!DNL  Workfront].
feature: Work Management
type: Tutorial
role: Admin, User
level: Beginner, Intermediate
last-substantial-update: 2023-07-18T00:00:00Z
jira: KT-10101
exl-id: bfa3ae5f-9618-444c-9eb8-5d82db9a77c7
source-git-commit: ce2aad1cd0ecb7d568ed9a01d97147cbd126ca05
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---

# Perguntas comuns sobre filas de solicitações

**Por que posso ver uma fila de solicitações, mas meu usuário não pode?**

No [!UICONTROL Detalhes da fila] da fila de solicitações/projeto, certifique-se de que o usuário se ajusta aos critérios de &quot;Quem pode adicionar solicitações a esta fila?&quot; campo.

**Concedi aos usuários acesso à fila, mas agora eles também podem ver o projeto da fila de solicitações. Porquê?**

Isso tem a ver com a maneira como você deu a eles acesso à fila de solicitações.

Se você usou o [!UICONTROL Compartilhamento] da página de aterrissagem do projeto da fila de solicitações, você deu a esses usuários acesso para ver o projeto na lista de projetos.

No entanto, se você quiser conceder acesso apenas para enviar uma solicitação para a fila, vá para Configuração da fila e selecione a opção apropriada em &quot;Quem pode adicionar solicitações a este projeto&quot;.

**Posso transformar uma solicitação em um projeto?**

Sim. Você pode converter problemas em tarefas ou projetos, dependendo do que é necessário.

Consulte este artigo para obter mais informações: [Converter problemas](https://experienceleague.adobe.com/docs/workfront/using/manage-work/issues/convert-issues/convert-issues-overview.html?lang=en).

**Onde encontro uma fila de solicitações para fazer edições?**

Você pode usar o [!UICONTROL Pesquisar] na barra de navegação ou localize-o listado no [!UICONTROL Projetos] área.

Se abrir uma solicitação da fila de solicitações, você pode clicar no nome do projeto na área de navegação estrutural.

**Posso transferir as informações de um formulário personalizado de solicitação para um formulário personalizado de projeto?**

Sim. Ao criar um formulário personalizado, selecione ambos [!UICONTROL Projeto] e [!UICONTROL Problema] como os tipos de objeto. Anexe o formulário personalizado à solicitação. Quando você converter a solicitação em um projeto, o formulário personalizado será anexado automaticamente ao novo projeto e os valores contidos em quaisquer campos aparecerão nos formulários de solicitação e de projeto personalizado.

**Estou vendo um relatório de projeto ou tarefa. Como posso descobrir de que solicitação esse objeto se originou?**

Você pode acessar campos na variável **[!UICONTROL Problema convertido]** e a variável **[!UICONTROL Originador de problema convertida]** fontes de campo para adicionar essas informações aos relatórios de projeto e tarefa.

**Qual é a melhor maneira de filtrar por filas de solicitações em um relatório?**

Se o filtro do seu projeto incluir **Fila>>É pública>>Igual>>Nenhuma** seu relatório mostrará apenas os projetos que estão **NOT** filas de solicitações.

Se o filtro do seu projeto incluir **Fila>>É Pública>>Não Igual>>Nenhuma** seu relatório mostrará somente projetos que **SÃO** filas de solicitações.
