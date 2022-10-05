---
title: Compreender o acesso financeiro
description: Os direitos de acesso financeiro permitem que os administradores controlem quem pode ver e editar as informações financeiras rastreadas no Workfront.
feature: Work Management
thumbnail: understand-financial-access.png
type: Tutorial
role: User
level: Intermediate
kt: 10067
exl-id: 1c3d724a-8ff0-466f-9416-cff3da59c8ea
source-git-commit: d0c842ad8bf6f52161f003a62237fbcd35d23176
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 5%

---

# Compreender o acesso financeiro

Se sua organização estiver capturando dados financeiros com [!DNL Workfront], como administrador do sistema, é sua responsabilidade proteger e gerenciar quem tem acesso para visualizar e editar essas informações.

Duas coisas são necessárias para que um usuário visualize ou edite informações financeiras:

1. Os direitos de acesso devem ser ativados no [!UICONTROL Nível de acesso].
2. A permissão para usar esses direitos de acesso deve ser concedida em uma base de objeto.

Por exemplo, um usuário pode receber direitos para exibir dados financeiros em seu nível de acesso, mas só pode visualizar dados financeiros em uma tarefa que é compartilhada com ele e a visualização financeira é ativada no compartilhamento dessa tarefa.

Portanto, é possível para um usuário com [!UICONTROL Nível de acesso] direitos de visualização de recursos financeiros para poder visualizar as finanças em alguns objetos e não em outros, dependendo das opções de compartilhamento individuais desses objetos. No entanto, nenhum usuário pode visualizar as finanças em qualquer objeto, a menos que tenha o direito concedido a elas em suas [!UICONTROL Nível de acesso].

## [!UICONTROL Nível de acesso] configurações

O acesso geral aos dados financeiros é concedido em primeiro lugar por [!DNL Workfront] tipo de licença.

**[!UICONTROL Plano] as licenças podem:**

* Gerenciar registros de faturamento
* Gerenciar e visualizar taxas de faturamento e custo de função
* Gerenciar e exibir taxas de faturamento e custo do usuário
* Gerenciar despesas
* Exibir e editar finanças

**[!UICONTROL Trabalho] as licenças podem:**

* Gerenciar despesas
* Exibir finanças

**[!UICONTROL Revisão] as licenças podem:**

* Exibir finanças

**As permissões podem ser modificadas pelo [!UICONTROL Nível de acesso]. As três opções para acesso a dados financeiros são:**

* [!UICONTROL Sem acesso] — O usuário não poderá ver informações financeiras.
* [!UICONTROL Exibir] — O usuário pode revisar e compartilhar as informações.
* [!UICONTROL Editar] — O usuário pode criar, editar, excluir e compartilhar as informações. (Disponível somente para uma licença do Plano.)

![Uma imagem que mostra as opções gerais de Dados Financeiros em um nível de acesso](assets/setting-up-finances-8.png)

É importante observar que a variável [!UICONTROL Exibir] e [!UICONTROL Editar] têm configurações adicionais para um [!UICONTROL Plano] licença. Clique na engrenagem na [!UICONTROL Exibir] para essas opções:

**[!UICONTROL Exibir]**

* Ver taxas de custo e cobrança de função
* Ver taxas de custo e cobrança de usuário

![Uma imagem que mostra as opções de visualização de Dados Financeiros em um nível de acesso](assets/setting-up-finances-9.png)

**[!UICONTROL Editar]**

Essas duas opções estão disponíveis no [!UICONTROL Editar] , juntamente com:

* Editar taxas de custo e cobrança de função
* Editar taxas de custo e cobrança de usuário

![Uma imagem que mostra as opções de edição de Dados Financeiros em um nível de acesso](assets/setting-up-finances-10.png)

>[!NOTE]
>
>Um usuário com acesso para adicionar despesas também pode visualizar as despesas adicionadas, bem como as despesas adicionadas pelos relatórios diretos.
