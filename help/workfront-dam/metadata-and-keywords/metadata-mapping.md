---
title: Configurar o mapeamento de metadados para [!UICONTROL Workfront DAM]
description: Saiba como configurar o mapeamento de metadados para [!UICONTROL Workfront DAM].
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
kt: 10088
exl-id: 3869db93-9fbc-4689-b838-0f4400a436c3
source-git-commit: a0aa8328842d2db1235edc42664eb0b18f4038e4
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---

# Mapeamento de metadados

[!DNL Workfront]Informações relacionadas sobre um ativo podem ser transferidas de [!DNL Workfront] em [!UICONTROL Workfront DAM] com o ativo. A opção de mapeamento de metadados no [!DNL Workfront] [!UICONTROL Configuração] permite essa transferência de informações.

Fale com o seu [!DNL Workfront] consultor para recomendações de práticas recomendadas sobre como configurar o mapeamento de metadados.

Você deve ser um [!DNL Workfront] administrador e um [!UICONTROL Workfront DAM] administrador para configurar o mapeamento de metadados. Antes de começar, você deve conectar [!DNL Workfront] e [!UICONTROL Workfront DAM] contas.

## Conexão de contas

1. Faça logon em [!DNL Workfront].
1. Abra um projeto, tarefa ou problema e clique no botão **[!UICONTROL Documentos]** guia .
1. Clique no botão **[!UICONTROL Adicionar novo]** e selecione **[!UICONTROL Do Workfront DAM]** no menu suspenso.
1. Digite seu nome de logon e senha no [!UICONTROL Workfront DAM] caixa de autorização exibida.
1. Em seguida, clique em **[!UICONTROL Sim]** para [!DNL Workfront] acesso ao [!UICONTROL DAM] conta.
1. Se necessário, atualize a página para atualizar o acesso ao [!UICONTROL Workfront DAM].

Com essa conexão estabelecida, agora você pode começar a mapear metadados entre os dois sistemas. Verifique se você já criou os campos de metadados necessários em [!UICONTROL Workfront DAM] antes de começar a mapear.

## Configurar o mapeamento

1. Faça logon em [!DNL Workfront].
1. Selecionar **[!UICONTROL Configuração]** do [!UICONTROL Menu principal].
1. Expanda o **[!UICONTROL Documentos]** no menu do painel esquerdo.
1. Em seguida, clique em **[!UICONTROL Mapeamento de metadados]**.
1. No campo Workfront , digite a fonte do campo da variável [!DNL Workfront] campo a ser mapeado.
1. Em seguida, selecione o target ou correspondente **[!UICONTROL Workfront DAM]** campo de metadados.
1. Clique no botão **[!UICONTROL Adicionar mapeamento]** botão.
1. Você verá o [!UICONTROL Origem de campo do Workfront] e [!UICONTROL Campo de destino DAM do Workfront] no gráfico na parte inferior da janela.
1. Repita o procedimento para todos os campos de metadados desejados.

![Uma captura de tela do [!UICONTROL Mapeamento de metadados] na tela [!DNL Workfront]](assets/01-metadata-mapping.png)
