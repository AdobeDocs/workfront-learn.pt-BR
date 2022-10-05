---
title: Prática recomendada - Filtros, exibições e agrupamentos
description: Explore as recomendações de práticas recomendadas dos especialistas do Adobe Workfront sobre como configurar, gerenciar e usar filtros, visualizações e agrupamentos do Workfront.
feature: Reports and Dashboards
role: Admin, Leader, User
level: Beginner
kt: 10911
exl-id: 845aa0b4-3fe9-4bc1-9dde-2f22c537e758
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 0%

---

# Prática recomendada - Filtros, exibições e agrupamentos

## O que é uma &quot;prática recomendada&quot; do Adobe Workfront?

As melhores práticas são orientações que representam uma linha de ação eficaz e eficiente; sejam adotados facilmente por você e pelos usuários em sua empresa; e podem ser replicados com êxito em toda a organização.

À medida que você revisa essas recomendações, lembre-se de que algumas práticas recomendadas do Workfront são universais, enquanto outras podem ser mais específicas para o tópico. Use essas práticas recomendadas como estrutura para ajudar a orientar as configurações e o uso do sistema Workfront.

## Navegar nesta página

Ao rolar por essa página, primeiro você encontrará uma lista de alto nível de todas as práticas recomendadas para o tópico. Isso permite que você revise as recomendações sem entrar nos detalhes de &quot;por quê&quot;.

O &quot;Por que essas práticas recomendadas estão sendo usadas?&quot; , encontrada após a lista de alto nível, fornece mais detalhes sobre algumas práticas recomendadas e por que elas são consideradas como um processo, ferramenta etc., você deve considerar a implementação com sua instância do Workfront.

</br>
</br>

## Filtros, visualizações e práticas recomendadas de agrupamento

* Reduza o número de relatórios personalizados criados por meio de filtros, exibições e agrupamentos em uma lista de objetos para obter os dados necessários.

* Use os controles de lista em modelos de layout para ocultar filtros, exibições e agrupamentos desnecessários para objetos usados com frequência (projetos, tarefas, programas, etc.).

* Compartilhe filtros, visualizações e agrupamentos personalizados relevantes para os fluxos de trabalho e processos de sua organização por meio dos controles de lista em modelos de layout.

* Ao criar filtros para status do projeto, status da tarefa ou status da emissão, use o campo (objeto)>>Status Equates With field source/field name com o modificador Equal, em vez do Project>>Status field source/field name.

</br>
</br>

## Por que essas práticas recomendadas estão presentes?

**Prática recomendada**

Reduza o número de relatórios personalizados criados por meio de filtros, exibições e agrupamentos em uma lista de objetos para obter os dados necessários.

**Veja o porquê**

Criar relatórios de uso único para cada segmento de dados que você deseja visualizar é demorado e desordena o sistema do Workfront.

</br>
</br>

**Prática recomendada**

Use os controles de lista em modelos de layout para ocultar filtros, exibições e agrupamentos desnecessários para objetos usados com frequência (projetos, tarefas, programas, etc.).

**Veja o porquê**

Menos é mais. Ocultar as opções de filtro, visualização e lista de agrupamento que não são relevantes para os fluxos de trabalho diários dos usuários restringe as listas, o que facilita que os usuários encontrem o que precisam mais rapidamente.

</br>
</br>

**Prática recomendada**

Compartilhe filtros, visualizações e agrupamentos personalizados relevantes para os fluxos de trabalho e processos de sua organização por meio dos controles de lista em modelos de layout.

**Veja o porquê**

Se você criou filtros, visualizações e agrupamentos que exibem informações específicas para os processos diários dos usuários, é fácil compartilhá-las nos modelos de layout. Isso garante que todos os usuários atribuídos a esse modelo de layout tenham opções de filtro, visualização e agrupamento relevantes para seus fluxos de trabalho.

Personalizar as informações que deseja que sejam visíveis para os usuários por meio dos modelos de layout também é uma economia de tempo para administradores de sistema e grupo, pois eles não precisarão compartilhar cada opção de filtro, visualização ou agrupamento individualmente.

</br>
</br>

**Prática recomendada**

Ao criar filtros para status do projeto, status da tarefa ou status da emissão, use o campo (objeto)>>Status Equates With field source/field name com o modificador Equal, em vez do Project>>Status field source/field name.

**Veja o porquê**

Ao usar (objeto)>>Equações com, você está incluindo todos os status personalizados que têm esse status específico atribuído no campo Equações com nas configurações de status. Enquanto a configuração do filtro como (objeto)>>Status > Igual requer a seleção de estatutos específicos para o filtro. Isso pode representar um desafio de manutenção se você precisar levar em conta esses novos status em vários filtros. Cada filtro precisaria ser aberto e atualizado com o novo status.

Por exemplo, se você quiser ver todos os projetos atuais, poderá configurar seu filtro para ler Projeto>>Status > Igual > Atual. Mas se alguém adicionar um status personalizado chamado Ativo e o equiparar a Atual, esse filtro não encontrará projetos com o status Ativo. No entanto, se você usar o Projeto>>Status equivale a com > Igual > Atual, o filtro localizará objetos com o status Atual ou Ativo porque ambos têm Atual no campo Equações com .
