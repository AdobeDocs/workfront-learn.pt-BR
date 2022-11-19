---
title: Além do mapeamento básico
description: Saiba como usar as fórmulas do painel de mapeamento para manipular ou converter campos enviados em um módulo.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11039
thumbnail: KT11039.png
exl-id: 979d794d-b936-402e-b07c-71e999f40780
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Além do mapeamento básico

Saiba como usar as fórmulas do painel de mapeamento para manipular ou converter campos enviados em um módulo.

## Visão geral do exercício

Altere o nome do projeto, a data de início planejada e a prioridade dos exercícios de explicação Além do Mapeamento Básico usando as fórmulas do painel de mapeamento.

![Além da imagem básica do mapeamento 1](../12-exercises/assets/beyond-basic-mapping-walkthrough-1.png)

## Etapas a seguir

**Faça um clone do cenário de design do cenário inicial.**

1. Selecione a opção Clone à direita do Initial scenario design na seção do cenário, conforme mostrado abaixo. Nomeie-o como &quot;Além do mapeamento básico&quot;.

   ![Além da imagem básica do mapeamento 2](../12-exercises/assets/beyond-basic-mapping-walkthrough-2.png)

   **Agora vamos usar o painel de mapeamento no módulo Criar projetos do Workfront para configurar o nome do projeto, a data de início planejada e os campos de prioridade.**

1. Clique no módulo Criar projetos do Workfront para editar as configurações. Usando o painel de mapeamento, altere o campo Nome para &quot;[Meu nome do projeto] por [Patrocinador].&quot;

   + O [Meu nome do projeto] é a coluna 1 do módulo CSV de análise e [Patrocinador] é a coluna 6. A palavra &quot;by&quot; é digitada entre os dois.

1. Em seguida, vá para a Data inicial planejada e use a fórmula addDays para adicionar 15 dias ao campo, conforme descrito no vídeo de explicação passo a passo do mapeamento básico Beyond.
1. Encontre o campo Priority e alterne o botão Map na parte superior direita do campo. O menu da lista de opções muda para um número. Crie uma declaração if para rotular um projeto como prioridade Alta(4) se a classificação de confiança do arquivo CSV for menor que 100, caso contrário poderá ser Normal(2).

   + A classificação de confiança está na coluna 4.

   **Neste ponto, o painel de mapeamento deve ter esta aparência:**

   ![Além da imagem básica do mapeamento 3](../12-exercises/assets/beyond-basic-mapping-walkthrough-3.png)

1. Clique em OK e depois em Executar uma vez.
1. Localize o projeto na instância do Workfront para verificar se tudo foi mapeado corretamente.
1. Salve o cenário.
