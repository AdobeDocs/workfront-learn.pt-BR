---
title: Tutorial de como acessar versões anteriores
description: Descubra como restaurar versões anteriores após fazer alterações no cenário e salvá-las no  [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9009
exl-id: dd2cc2a2-e5af-41cc-bc0d-6be1efd996d9
last-substantial-update: '2026-08-12T00:00:00.000Z'
recommendations: noDisplay,catalog
doc-type: video
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:39:17.503Z'
source-git-commit: 4b419797e3014599bffd64f576d8eeb196c8c153
workflow-type: tm+mt
source-wordcount: 280
ht-degree: 78%

---

# Tutorial de como acessar versões anteriores

Neste vídeo, você:

* Descubra como restaurar versões anteriores após fazer alterações no seu cenário e salvá-lo diversas vezes.

## Tutorial de como acessar versões anteriores

O Workfront recomenda assistir ao tutorial em vídeo antes de tentar recriar o exercício em seu próprio ambiente.

>[!VIDEO](https://video.tv.adobe.com/v/335268/?quality=12&learn=on&enablevpops=1)

>[!NOTE]
>
>Depois de salvar o cenário, o Workfront Fusion mantém a versão anterior do cenário por 60 dias. O período de retenção de uma versão começa quando essa versão é substituída por uma versão mais recente, não quando a versão foi originalmente criada.
>Para manter o histórico de versões do cenário além de 60 dias para fins de auditoria, salve e arquive um blueprint do cenário em um local combinado.


## Adicionar à terminologia

![Imagem de um registro de observação e um módulo de webhook personalizado](assets/understand-the-basics-3.png)

### Módulos acionadores

Os módulos acionadores só podem ser usados como o primeiro módulo e podem retornar zero, um ou mais pacotes. Estes serão processados individualmente em módulos subsequentes, a menos que sejam agregados.

**Acionador de sondagem (ícone de relógio no acionador)** - Recursos especiais para monitorar o último registro processado.

**Acionador instantâneo (ícone de raio no acionador)** - Acionado imediatamente com base no webhook.

![Imagem de um registro de criação e um módulo de pesquisa](assets/understand-the-basics-4.png)

### Módulos de ações e pesquisa

**Ação** - Usado para executar operações CRUD (criar, ler, atualizar e excluir)

**Pesquisas** - Usado para procurar zero, um ou mais registros, retornando-os como pacotes que serão processados individualmente em módulos subsequentes, a menos que sejam agregados.

## Quer saber mais? Recomendamos o seguinte:

[Documentação do Workfront Fusion](https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)
