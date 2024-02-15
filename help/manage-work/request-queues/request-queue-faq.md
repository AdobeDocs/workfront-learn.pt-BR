---
title: Respostas a perguntas comuns sobre filas de solicitações
description: Obtenha respostas para perguntas comuns sobre filas de solicitações no [!DNL  Workfront].
feature: Work Management
type: Tutorial
role: Admin, User
level: Beginner
last-substantial-update: 2023-07-18T00:00:00Z
jira: KT-10101
exl-id: bfa3ae5f-9618-444c-9eb8-5d82db9a77c7
source-git-commit: ec82cd0aafb89df7b3c46eb716faf3a25cd438a2
workflow-type: ht
source-wordcount: '406'
ht-degree: 100%

---

# Respostas a perguntas comuns sobre filas de solicitações

**Por que posso ver uma fila de solicitações, mas meu usuário não?**

Na guia de [!UICONTROL Detalhes da fila] de solicitações ou projeto, certifique-se de que o usuário atenda aos critérios do campo “Quem pode adicionar solicitações a esta fila?”

**Forneci acesso à fila aos usuários, mas eles também podem ver o projeto da fila de solicitações. Porquê?**

Isso é devido à forma como você concedeu acesso à fila de solicitações.

Se você usou a ferramenta [!UICONTROL Compartilhamento] da fila de solicitações da página de destino do projeto, esses usuários poderão ver o projeto na lista de projetos.

No entanto, se você deseja apenas permitir que o usuário envie uma solicitação à fila, acesse as Configuração da fila e selecione a opção apropriada em “Quem pode adicionar solicitações neste projeto”.

**Posso transformar uma solicitação em um projeto?**

Sim. Você pode converter problemas em tarefas ou projetos, dependendo do que for necessário.

Consulte este artigo para obter mais informações: [Converter problemas](https://experienceleague.adobe.com/docs/workfront/using/manage-work/issues/convert-issues/convert-issues-overview.html?lang=pt-BR).

**Onde encontro uma fila de solicitações para fazer edições?**

Você pode usar o campo [!UICONTROL Pesquisar] na barra de navegação ou encontrá-la na área [!UICONTROL Projetos].

Se você abrir uma solicitação da fila de solicitações, poderá clicar no nome do projeto na área de navegação estrutural.

**Posso transferir as informações de um formulário de solicitação personalizado para um formulário de projeto personalizado?**

Sim. Ao criar um formulário personalizado, selecione ambos o [!UICONTROL Projeto] e o [!UICONTROL Problema] como tipos de objeto. Anexe o formulário personalizado à solicitação. Ao converter a solicitação em um projeto, o formulário personalizado será anexado automaticamente ao novo projeto e os valores de todos os campos aparecerão nos formulários da solicitação e do projeto.

**Estou vendo um relatório de projeto ou tarefa. Como posso descobrir de qual solicitação esse objeto se originou?**

Você pode acessar os campos nas origens de campo **[!UICONTROL Problema convertido]** e **[!UICONTROL Originador do problema convertido]** para adicionar essas informações aos seus relatórios de projetos e tarefas.

**Qual é a melhor maneira de filtrar filas de solicitações em um relatório?**

Se o filtro do projeto incluir **Fila>>É pública>>Igual>>Nenhum**, o relatório mostrará apenas projetos que **NÃO** são filas de solicitações.

Se o filtro do projeto incluir **Fila>>É pública>>Não é igual>>Nenhum**, o relatório mostrará apenas projetos que **SÃO** filas de solicitações.
