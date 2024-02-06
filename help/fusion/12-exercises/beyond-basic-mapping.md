---
title: Além do mapeamento básico
description: Saiba como usar as fórmulas do painel de mapeamento para manipular ou converter campos enviados para um módulo.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11039
thumbnail: KT11039.png
exl-id: 979d794d-b936-402e-b07c-71e999f40780
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '302'
ht-degree: 100%

---

# Além do mapeamento básico

Saiba como usar as fórmulas do painel de mapeamento para manipular ou converter campos enviados para um módulo.

## Visão geral do exercício

Altere o nome do projeto, a data de início planejada e a prioridade a partir dos exercícios do tutorial Além do mapeamento básico, que utilizam as fórmulas do painel de mapeamento.

![Além do mapeamento básico - Imagem 1](../12-exercises/assets/beyond-basic-mapping-walkthrough-1.png)

## Etapas a serem seguidas

**Crie um design idêntico ao utilizado no cenário inicial.**

1. Selecione a opção Clonar à direita do design inicial na seção Cenário, conforme mostrado abaixo. Nomeie-o como “Além do mapeamento básico”.

   ![Além do mapeamento básico - Imagem 2](../12-exercises/assets/beyond-basic-mapping-walkthrough-2.png)

   **Agora vamos usar o painel de mapeamento no módulo Criar projetos do Workfront para configurar o nome do projeto, a data de início planejada e os campos prioritários.**

1. Clique no módulo Criar projetos do Workfront para editar as configurações. Usando o painel de mapeamento, altere o campo Nome para “[Nome do meu projeto] de [Patrocinador]”.

   + O [Nome do meu projeto] é a coluna 1 do módulo Analisar CSV e o[ Patrocinador] é a coluna 6. A palavra “de” é apenas inserida entre as duas.

1. Em seguida, vá para a data de início planejada e use a fórmula addDays para adicionar 15 dias ao campo, conforme descrito no tutorial em vídeo Além do mapeamento básico.
1. Encontre o campo Prioridade e alterne o botão Mapa no canto superior direito do campo. O menu da lista de opções muda para um número. Crie uma instrução SE para rotular um projeto com prioridade Alta (4) se a classificação de confiança do arquivo CSV for inferior a 100; caso contrário, a prioridade pode ser Normal (2).

   + A classificação de confiança está na coluna 4.

   **A essa altura, o painel de mapeamento deve ter esta aparência:**

   ![Além do mapeamento básico - Imagem 3](../12-exercises/assets/beyond-basic-mapping-walkthrough-3.png)

1. Clique em OK e selecione Executar uma vez.
1. Encontre o projeto na sua instância do Workfront para garantir que tudo foi mapeado corretamente.
1. Salve seu cenário.
