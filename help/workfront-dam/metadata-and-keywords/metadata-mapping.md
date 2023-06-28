---
title: Configurar o mapeamento de metadados para [!UICONTROL DAM DO WORKFRONT]
description: Saiba como configurar o mapeamento de metadados para [!UICONTROL DAM DO WORKFRONT].
activity: use
team: Technical Marketing
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
jira: KT-10088
exl-id: 3869db93-9fbc-4689-b838-0f4400a436c3
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---

# Mapeamento de metadados

[!DNL Workfront]As informações relacionadas ao sobre um ativo podem ser transferidas do [!DNL Workfront] em [!UICONTROL DAM DO WORKFRONT] com o ativo. A opção de mapeamento de metadados no [!DNL Workfront] [!UICONTROL Configuração] permite essa transferência de informações.

Fale com o seu [!DNL Workfront] consultor do para práticas recomendadas de configuração do mapeamento de metadados.

Você deve ser um [!DNL Workfront] administrador e um [!UICONTROL DAM DO WORKFRONT] administrador para configurar o mapeamento de metadados. Antes de começar, você deve conectar seu [!DNL Workfront] e [!UICONTROL DAM DO WORKFRONT] contas.

## Conectar contas

1. Efetue logon no [!DNL Workfront].
1. Abra um projeto, tarefa ou problema e clique no botão **[!UICONTROL Documentos]** guia.
1. Clique em **[!UICONTROL Adicionar novo]** e selecione **[!UICONTROL Do DAM do Workfront]** no menu suspenso.
1. Insira seu nome de logon e senha na [!UICONTROL DAM DO WORKFRONT] que aparece.
1. Clique em **[!UICONTROL Sim]** para dar [!DNL Workfront] acesso à [!UICONTROL DAM] conta.
1. Se necessário, atualize a página para atualizar o acesso ao [!UICONTROL DAM DO WORKFRONT].

Com essa conexão estabelecida, agora é possível começar a mapear metadados entre os dois sistemas. Verifique se você já criou os campos de metadados necessários no [!UICONTROL DAM DO WORKFRONT] antes de iniciar o mapeamento.

## Configurar o mapeamento

1. Efetue logon no [!DNL Workfront].
1. Selecionar **[!UICONTROL Configuração]** do [!UICONTROL Menu principal].
1. Expanda a **[!UICONTROL Documentos]** no menu do painel esquerdo.
1. Depois clique em **[!UICONTROL Mapeamento de metadados]**.
1. No campo Workfront, digite a origem do campo do [!DNL Workfront] para mapear.
1. Em seguida, selecione o target ou correspondente **[!UICONTROL DAM DO WORKFRONT]** campo de metadados.
1. Clique em **[!UICONTROL Adicionar mapeamento]** botão.
1. Você verá o [!UICONTROL Origem do campo Workfront] e [!UICONTROL Campo alvo do Workfront DAM] no gráfico na parte inferior da janela.
1. Repita o procedimento para todos os campos de metadados desejados.

![Uma captura de tela do [!UICONTROL Mapeamento de metadados] tela em [!DNL Workfront]](assets/01-metadata-mapping.png)
