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
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Além do mapeamento básico

Saiba como usar as fórmulas do painel de mapeamento para manipular ou converter campos enviados para um módulo.

## Visão geral do exercício

Altere o nome do projeto, a data de início planejada e a prioridade dos exercícios de explicação Além do mapeamento básico, usando as fórmulas do painel de mapeamento.

![Além da imagem básica de mapeamento 1](../12-exercises/assets/beyond-basic-mapping-walkthrough-1.png)

## Etapas a serem seguidas

**Faça um clone de seu cenário de design de cenário inicial.**

1. Selecione a opção Clone à direita do design de cenário inicial na seção de cenário, conforme mostrado abaixo. Nomeie-o como &quot;Além do mapeamento básico&quot;.

   ![Além da imagem básica de mapeamento 2](../12-exercises/assets/beyond-basic-mapping-walkthrough-2.png)

   **Agora vamos usar o painel de mapeamento no módulo Criar projetos Workfront para configurar o nome do projeto, a data de início planejada e os campos de prioridade.**

1. Clique no módulo Criar projetos Workfront para editar as configurações. Usando o painel de mapeamento, altere o campo Nome para &quot;[Nome do Meu Projeto] por [Patrocinador].&quot;

   + A variável [Nome do Meu Projeto] é a coluna 1 do módulo Analisar CSV e [Patrocinador] é a coluna 6. A palavra &quot;by&quot; é simplesmente digitada entre os dois.

1. Em seguida, vá para a Data de início planejada e use a fórmula addDays para adicionar 15 dias ao campo, conforme descrito no vídeo detalhado Beyond basic mapping.
1. Localize o campo Prioridade e alterne o botão Mapa na parte superior direita do campo. O menu da lista de opções muda para um número. Crie uma declaração if para rotular um projeto como de alta prioridade (4) se a classificação de confiança do arquivo CSV for menor que 100, caso contrário, poderá ser Normal (2).

   + A classificação de confiança está na Coluna 4.

   **Neste ponto, o painel de mapeamento deve ter esta aparência:**

   ![Além da imagem básica de mapeamento 3](../12-exercises/assets/beyond-basic-mapping-walkthrough-3.png)

1. Clique em OK e, em seguida, clique em Executar uma vez.
1. Encontre o projeto na instância do Workfront para garantir que tudo foi mapeado corretamente.
1. Salve seu cenário.
