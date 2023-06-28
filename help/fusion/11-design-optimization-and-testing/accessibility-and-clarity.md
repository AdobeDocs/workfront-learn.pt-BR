---
title: Acessibilidade e clareza
description: Conheça algumas práticas recomendadas básicas para facilitar a leitura, o compartilhamento e a compreensão de cenários.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11037
exl-id: ba2c5c64-ab4d-42d3-8a69-6b9df1373b29
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 0%

---

# Acessibilidade e clareza

No início do treinamento do Workfront Fusion, você aprendeu algumas práticas recomendadas básicas para facilitar a leitura, o compartilhamento e a compreensão de cenários. Essas práticas ajudam a facilitar as coisas para futuros usuários do Workfront Fusion ou para qualquer pessoa que esteja solucionando problemas ou oferecendo suporte à sua instância do Workfront Fusion. Pague-o seguindo as diretrizes abaixo ao criar os cenários.

## Rótulos e notas

Como regra geral, um objetivo principal no Workfront Fusion é sempre ter designs de cenário simples. Estas são algumas maneiras de criar designs simples de interpretar.

* Certifique-se de nomear todos os módulos. Clique com o botão direito em um módulo e selecione Renomear. Os rótulos do módulo devem ser curtos, mas ainda assim compreensíveis, para o desempenho do módulo. Por exemplo, &quot;Criar Proj Mktg Com Modelo Ch&quot;.
  ![Uma imagem de um cenário com manipulação de erros](assets/design-optimization-and-testing-1.png)
* Rotular caminhos de roteamento também. Mesmo que um caminho não use um filtro diretamente após um roteador, é possível aplicar um rótulo sem preencher a lógica do filtro. Fazer isso permite que outros entendam quais pacotes passam por quais caminhos e por quê. Para criar um rótulo para um caminho de roteador sem filtro, clique com o botão direito do mouse no caminho, adicione um rótulo e salve.
  ![Uma imagem de um cenário com manipulação de erros](assets/design-optimization-and-testing-2.png)
* Adicione observações, quando aplicável, em um cenário se um rótulo de módulo ou de caminho de roteamento for muito curto para esclarecer o que realmente está acontecendo. É possível adicionar observações sempre que desejar em todo o processo de design e iteração.

No entanto, pode ser mais fácil ler e entender se você adicionar observações no final do design do cenário quando estiver pronto para iniciar. Trabalhe do final do design do cenário (canto inferior direito distante) para trás. Dessa forma, as notas que se aplicam ao início do cenário estão no topo da lista ao abrir o painel de notas.

Depois de salvar ou fechar o painel &#39;Notas&#39;, as notas são classificadas com as criadas mais recentemente na parte superior. Na imagem abaixo, a primeira nota criada aparece na parte inferior da lista. As notas foram criadas intencionalmente do canto inferior direito para o caminho acima e, finalmente, para o acionador — basicamente, a ordem inversa pela qual um conjunto de dados passaria pelo cenário. Isso faz com que as notas apareçam na ordem em que o cenário realmente é executado no pacote de dados.

![Uma imagem de um cenário com manipulação de erros](assets/design-optimization-and-testing-3.png)

## Modelos do Workfront Fusion

Uma ótima maneira de simplificar a rotulagem de módulos e caminhos de roteamento é usando modelos. Os modelos de práticas recomendadas podem acelerar a criação de cenários para casos de uso comuns.

### Exemplo de modelo

Ao iniciar um cenário, verifique primeiro se há um modelo disponível que ajudará. Por exemplo, você deseja criar um cenário que começa baixando um documento CSV do Workfront e, em seguida, o analisa.

Clique na seção Modelos para ver se algum modelo público atende às suas necessidades.

![Uma imagem de um cenário com manipulação de erros](assets/design-optimization-and-testing-4.png)

Clique na guia Modelos de equipe para ver se alguém na sua equipe criou um modelo que pode ser útil.

Se você encontrar um modelo que deseja usar, clique no nome para abri-lo.

![Uma imagem de um cenário com manipulação de erros](assets/design-optimization-and-testing-5.png)

Em seguida, vá para o canto superior direito, clique em Opções e selecione Criar cenário.

![Uma imagem de um cenário com manipulação de erros](assets/design-optimization-and-testing-6.png)

### Criar um modelo

Você pode criar um modelo na seção Modelos de Equipe. O modelo criado está disponível para você e sua equipe, mas quando você clica no botão Publicar, pode compartilhá-lo com pessoas de fora da equipe.

![Uma imagem de um cenário com manipulação de erros](assets/design-optimization-and-testing-7.png)

Ao criar o modelo, você pode incluir um assistente para orientar as pessoas que o usam para criar seus cenários, alterando as conexões, os dados mapeados e outros campos de painel, conforme apropriado.

Marque a caixa de seleção &quot;Usar no assistente&quot; para adicionar instruções que estarão disponíveis quando alguém criar um cenário usando seu modelo. Essas informações aparecerão no campo Ajuda. Para permitir que os usuários vejam esse texto ao usar o modelo, habilite Usar como valor padrão.

![Uma imagem de um cenário com manipulação de erros](assets/design-optimization-and-testing-8.png)

## Quer saber mais? Recomendamos o seguinte:

[Documentação do Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
