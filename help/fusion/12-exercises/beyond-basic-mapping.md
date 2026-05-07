---
title: Além do exercício básico de mapeamento
description: Saiba como usar as fórmulas do painel de mapeamento para manipular ou converter campos enviados para um módulo.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11039
thumbnail: KT11039.png
recommendations: noDisplay,catalog
exl-id: 979d794d-b936-402e-b07c-71e999f40780
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:44:57.573Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 314
ht-degree: 100%

---

# Além do exercício básico de mapeamento

Saiba como usar as fórmulas do painel de mapeamento para manipular ou converter campos enviados para um módulo.

## Visão geral do exercício

Altere o nome do projeto, a data inicial planejada e a prioridade a partir dos exercícios do tutorial Além do mapeamento básico, que utilizam as fórmulas do painel de mapeamento.

![Além do mapeamento básico - Imagem 1](../12-exercises/assets/beyond-basic-mapping-walkthrough-1.png)

## Etapas a serem seguidas

**Crie um design idêntico ao utilizado no cenário inicial.**

1. Selecione a opção Clonar à direita do design inicial na seção Cenário, conforme mostrado abaixo. Nomeie-o como “Além do mapeamento básico”.

   ![Além do mapeamento básico - Imagem 2](../12-exercises/assets/beyond-basic-mapping-walkthrough-2.png)

   **Agora vamos usar o painel de mapeamento no módulo Criar projetos do Workfront para configurar o nome do projeto, a data inicial planejada e os campos prioritários.**

1. Clique no módulo Criar projetos do Workfront para editar as configurações. Usando o painel de mapeamento, altere o campo Nome para “[Nome do meu projeto] de [Patrocinador]”.

   + O [Nome do meu projeto] é a coluna 1 do módulo Analisar CSV e o[ Patrocinador] é a coluna 6. A palavra “de” é apenas inserida entre as duas.

1. Em seguida, vá para a data inicial planejada e use a fórmula addDays para adicionar 15 dias ao campo, conforme descrito no tutorial em vídeo Além do mapeamento básico.
1. Encontre o campo Prioridade e alterne o botão Mapa no canto superior direito do campo. O menu da lista de opções muda para um número. Crie uma instrução SE para rotular um projeto com prioridade Alta (4) se a classificação de confiança do arquivo CSV for inferior a 100; caso contrário, a prioridade pode ser Normal (2).

   + A classificação de confiança está na coluna 4.

   **A essa altura, o painel de mapeamento deve ter esta aparência:**

   ![Além do mapeamento básico - Imagem 3](../12-exercises/assets/beyond-basic-mapping-walkthrough-3.png)

1. Clique em OK e selecione Executar uma vez.
1. Encontre o projeto na sua instância do Workfront para garantir que tudo foi mapeado corretamente.
1. Salve seu cenário.
