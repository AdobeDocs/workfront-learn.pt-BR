---
title: Entenda o acesso financeiro
description: Saiba como os direitos de acesso financeiro permitem que admins controlem quem pode ver e editar as informações financeiras registradas no Workfront.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-financial-access.png
type: Tutorial
role: User
level: Intermediate
jira: KT-10067
hide: true
exl-id: ded6b570-3e2a-4372-867d-a370de30dc31
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-05T19:01:54.624Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 415
ht-degree: 95%

---

# Entenda o acesso financeiro

Se sua organização estiver capturando dados financeiros com o [!DNL Workfront], como admin de sistema, é sua responsabilidade proteger o acesso a essas informações, definindo quem pode visualizá-las e editá-las.

São necessárias duas coisas para que um usuário visualize ou edite informações financeiras:

1. Os direitos de acesso devem ser habilitados no [!UICONTROL Nível de acesso].
2. A permissão para usar esses direitos de acesso deve ser concedida em cada objeto.

Por exemplo, um usuário pode receber direitos para visualizar dados financeiros em seu nível de acesso, mas só poderá visualizar dados financeiros de uma tarefa que seja compartilhada com ele e na qual a visualização de dados financeiros foi habilitada durante o compartilhamento dessa tarefa.

Portanto, é possível que um usuário que recebeu direitos de [!UICONTROL nível de acesso] para visualizar informações financeiras veja informações financeiras de alguns objetos e não de outros, pois isso dependerá das opções individuais de compartilhamento desses objetos. No entanto, nenhum usuário pode visualizar as informações financeiras de um objeto a menos que tenha recebido o direito para isso em seu [!UICONTROL Nível de acesso].

## Configurações de [!UICONTROL Nível de acesso]

O acesso geral aos dados financeiros é concedido primeiro pelo tipo de licença do [!DNL Workfront].

As licenças de **[!UICONTROL Plano] podem:**

* Gerenciar registros de cobrança
* Gerenciar e visualizar o faturamento de funções e as taxas de custo
* Gerenciar e visualizar o faturamento de usuários e as taxas de custo
* Gerenciar despesas
* Visualizar e editar informações financeiras

As licenças de **[!UICONTROL Trabalho] podem:**

* Gerenciar despesas
* Visualizar informações financeiras

As licenças de **[!UICONTROL Revisão] podem:**

* Visualizar informações financeiras

**As permissões podem ser modificadas pelo [!UICONTROL Nível de acesso]. As três opções de acesso a dados financeiros são:**

* [!UICONTROL Sem acesso] - O usuário não poderá ver informações financeiras.
* [!UICONTROL Visualizar] - O usuário pode analisar e compartilhar as informações.
* [!UICONTROL Editar] - O usuário pode criar, editar, excluir e compartilhar as informações. (Disponível somente para licenças de Plano.)

![Uma imagem que mostra as opções gerais de dados financeiros em um nível de acesso](assets/setting-up-finances-8.png)

É importante observar que as opções [!UICONTROL Exibir] e [!UICONTROL Editar] têm configurações adicionais para uma licença do [!UICONTROL Plano]. Clique no ícone de engrenagem do botão [!UICONTROL Visualizar] destas opções:

**[!UICONTROL Exibir]**

* Ver taxas de custo e cobrança de função
* Ver taxas de custo e cobrança de usuário

![Uma imagem que mostra as opções de visualização de dados financeiros em um nível de acesso](assets/setting-up-finances-9.png)

**[!UICONTROL Editar]**

Essas duas opções estão disponíveis para a opção [!UICONTROL Editar], além de:

* Editar taxas de custo e cobrança de função
* Editar taxas de custo e cobrança de usuário

![Uma imagem que mostra as opções de edição de dados financeiros em um nível de acesso](assets/setting-up-finances-10.png)

>[!NOTE]
>
>Usuário que têm permissão para adicionar despesas também podem visualizar as despesas adicionadas, bem como as despesas adicionadas por seus subordinados diretos.
