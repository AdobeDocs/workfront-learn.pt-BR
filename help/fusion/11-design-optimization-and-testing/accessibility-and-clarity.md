---
title: Acessibilidade e clareza
description: Aprenda algumas práticas recomendadas básicas para facilitar a leitura, o compartilhamento e a compreensão de cenários.
activity: use
type: Tutorial
team: Technical Marketing
kt: 11037
exl-id: ba2c5c64-ab4d-42d3-8a69-6b9df1373b29
source-git-commit: a64b29632b502af42d366ce543e5a71e9901e99c
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 0%

---

# Acessibilidade e clareza

No início do treinamento do Workfront Fusion, você aprendeu algumas práticas recomendadas básicas para facilitar a leitura, o compartilhamento e a compreensão dos cenários. Essas práticas ajudam a facilitar as coisas para futuros usuários do Workfront Fusion ou qualquer pessoa que solucione problemas ou suporte à sua instância do Workfront Fusion. Realize o pagamento seguindo as diretrizes abaixo ao projetar cenários.

## Rótulos e notas

Como regra geral, um objetivo principal no Workfront Fusion é sempre ter designs de cenário simples. Estas são algumas maneiras de fazer designs de interpretação simples.

* Certifique-se de nomear todos os módulos. Clique com o botão direito do mouse em um módulo e selecione Renomear. As etiquetas do módulo devem ser curtas, mas compreensíveis, para o que o módulo está executando. Por Exemplo, &quot;Criar Mktg Proj c/ Modelo Ch&quot;.
   ![Uma imagem de um cenário com tratamento de erros](assets/design-optimization-and-testing-1.png)
* Os caminhos de roteamento de etiquetas também. Mesmo que um caminho não use um filtro diretamente após um roteador, você pode aplicar um rótulo sem preencher a lógica do filtro. Fazer isso permite que outros entendam quais pacotes passam por quais caminhos e por quê. Para criar um rótulo para um caminho de roteador sem filtro, clique com o botão direito do mouse no caminho, adicione um rótulo e salve.
   ![Uma imagem de um cenário com tratamento de erros](assets/design-optimization-and-testing-2.png)
* Adicione observações, onde aplicável, em um cenário, se um rótulo de módulo ou rótulo de caminho de roteamento for muito curto para esclarecer o que está realmente acontecendo. Você pode adicionar notas sempre que desejar durante todo o processo de criação e iteração.

No entanto, pode ser mais fácil ler e entender se você adicionar observações ao final do design do cenário, quando estiver pronto para iniciar. Trabalhe a partir do fim do design do cenário (o canto inferior ou direito) para trás. Dessa forma, as notas que se aplicam ao início do seu cenário ficam no topo da lista ao abrir o painel de notas.

Depois de salvar ou fechar o painel de notas, as notas são classificadas com as últimas criadas na parte superior. Na imagem abaixo, a primeira nota criada aparece na parte inferior da lista. As notas foram intencionalmente criadas da parte inferior direita para o caminho acima e finalmente para o acionador— essencialmente a ordem inversa que um pacote de dados passaria pelo cenário. Isso faz com que as notas apareçam na ordem em que o cenário realmente é executado no pacote de dados.

![Uma imagem de um cenário com tratamento de erros](assets/design-optimization-and-testing-3.png)

## Templates Workfront Fusion

Uma ótima maneira de simplificar a rotulagem de módulos e caminhos de roteamento é usando modelos. Os modelos de práticas recomendadas podem acelerar a criação de cenários para casos de uso comuns.

### Exemplo de modelo

Ao iniciar um cenário, primeiro verifique se há um template disponível que ajudará. Por exemplo, você deseja criar um cenário que começa baixando um documento CSV do Workfront e depois o analisa.

Clique na seção Modelos para ver se algum modelo público atende às suas necessidades.

![Uma imagem de um cenário com tratamento de erros](assets/design-optimization-and-testing-4.png)

Clique na guia Modelos de equipe para ver se alguém em sua equipe criou um modelo que pode ser útil.

Se você encontrar um modelo que deseja usar, clique no nome para abri-lo.

![Uma imagem de um cenário com tratamento de erros](assets/design-optimization-and-testing-5.png)

Em seguida, vá para o canto superior direito, clique em Opções e selecione Criar cenário.

![Uma imagem de um cenário com tratamento de erros](assets/design-optimization-and-testing-6.png)

### Criar um modelo

Você pode criar um modelo na seção Modelos de Equipe . O modelo criado está disponível para você e sua equipe, mas ao clicar no botão Publicar , é possível compartilhá-lo com pessoas fora da equipe.

![Uma imagem de um cenário com tratamento de erros](assets/design-optimization-and-testing-7.png)

Ao criar o modelo, você pode incluir um assistente para orientar as pessoas que o usam para criar seus cenários, alterar as conexões, dados mapeados e outros campos do painel, conforme apropriado.

Marque a caixa de seleção &quot;Usar no Assistente&quot; para adicionar instruções que estarão disponíveis quando alguém criar um cenário usando seu modelo. Essas informações serão exibidas no campo Ajuda . Para permitir que os usuários vejam este texto ao usar o modelo, habilite Usar como valor padrão.

![Uma imagem de um cenário com tratamento de erros](assets/design-optimization-and-testing-8.png)

## Quer saber mais? Recomendamos o seguinte:

[Documentação do Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
