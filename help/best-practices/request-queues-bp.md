---
title: Prática recomendada - Filas de solicitação
description: Explore as recomendações de práticas recomendadas dos especialistas do Adobe Workfront sobre a configuração, o gerenciamento e o uso das filas de solicitações do Workfront.
feature: Resource Management
role: Admin, Leader, User
level: Beginner
jira: KT-10921
exl-id: dbb961f9-c207-49f1-9545-ec127f983c15
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1480'
ht-degree: 0%

---

# Prática recomendada - Filas de solicitação

## O que é uma &quot;prática recomendada&quot; do Adobe Workfront?

As práticas recomendadas são diretrizes que representam um curso de ação eficaz e eficiente; são facilmente adotadas por você e pelos usuários em sua empresa; e podem ser replicadas com sucesso em toda a organização.

Ao revisar essas recomendações, lembre-se de que algumas práticas recomendadas do Workfront são universais, enquanto outras podem ser mais específicas ao tópico. Use essas práticas recomendadas como uma estrutura para ajudar a orientar as configurações e o uso do sistema Workfront.

## Navegando nesta página

Ao percorrer essa página, primeiro você encontrará uma lista de alto nível de todas as práticas recomendadas para o tópico. Isso permite analisar as recomendações sem mergulhar nos detalhes do &quot;por quê&quot;.

O &quot;Por que essas práticas recomendadas?&quot; A área, localizada após a lista de alto nível, fornece mais detalhes sobre algumas das práticas recomendadas e por que elas são consideradas um processo, ferramenta, etc. Você deve considerar a implementação com sua instância do Workfront.

</br>
</br>

## Práticas recomendadas para a fila de solicitações

* Inclua uma descrição para cada elemento de uma fila de solicitações — o projeto da fila de solicitações, grupos de tópicos, tópicos da fila e regras de roteamento.

* Crie um status de projeto chamado &quot;Fila de solicitações&quot; ou &quot;Operacional&quot; que corresponda a &quot;Atual&quot; para distinguir projetos da fila de solicitações de outros projetos.

* Se você planeja usar aprovações de problemas com solicitações enviadas por meio de uma fila, crie um status de problema chamado Rejeitado.

* Atribua formulários personalizados &quot;universais&quot; às filas de solicitações para capturar o máximo possível de dados consistentes em toda a empresa.

* Evite compartilhar filas de solicitações com &quot;todos&quot;. Defina as configurações de detalhes da fila para que os usuários vejam apenas as filas relevantes às suas necessidades.

* Crie e atribua um painel contendo relatórios da fila de solicitações para que os gerenciadores de tráfego, administradores do sistema ou usuários atribuídos possam trabalhar nos problemas diretamente.

* Use modelos de layout para remover as opções de configuração da fila de solicitações do menu de projetos do painel esquerdo para usuários que não precisam criar filas.

* Crie uma fila de solicitações do administrador do sistema para que os usuários façam perguntas relacionadas ao Workfront, solicitações relacionadas às configurações do sistema, agendem treinamento de novos usuários etc.

* Auditoria de filas de solicitações regularmente para identificar e cancelar o compartilhamento de filas que não estão sendo usadas.

* Use grupos de tópicos para organizar mais de dez tópicos da fila em uma fila de solicitações para criar listas mais curtas e fáceis de gerenciar.

* Controlar o número total de filas de solicitações disponíveis aos usuários detalhando uma fila de solicitações usando grupos de tópicos e tópicos da fila, em vez de criar várias filas.

* Configurar regras de roteamento para cada tópico da fila. No mínimo, configure uma regra de roteamento padrão.

* Aproveite grupos de tópicos e tópicos de fila quando o roteamento seletivo for necessário.

* Encaminhar solicitações a uma equipe, em vez de a um indivíduo.


</br>
</br>


## Por que essas práticas recomendadas?


**Prática recomendada**

Inclua uma descrição para cada elemento de uma fila de solicitações — o projeto da fila de solicitações, grupos de tópicos, tópicos da fila e regras de roteamento.

**Veja o porquê**

As descrições permitem que administradores de grupos, futuros administradores do sistema ou outros que mantenham filas de solicitações saibam exatamente o que cada parte da fila de solicitações faz.

As informações de descrição também aparecem quando você passa o mouse sobre o ícone de informações no campo na nova janela de solicitação.

A descrição não precisa ser longa, apenas um breve comentário sobre o propósito ou o uso do elemento.

</br>
</br>

**Prática recomendada**

Crie um status de projeto chamado &quot;Fila de solicitações&quot; ou &quot;Operacional&quot; que corresponda a &quot;Atual&quot; para distinguir projetos da fila de solicitações de outros projetos.

**Veja o porquê**

Uma fila de solicitações &quot;vive&quot; em um projeto e deve estar em um status igual a Atual para que a fila fique ativa.

Para distinguir uma solicitação de projetos de trabalho reais com status &quot;Atual&quot;, crie um status para ser usado apenas em filas de solicitações chamadas &quot;Fila de solicitações&quot; ou &quot;Operacional&quot;. Você pode usar esse status para ajudar a excluir ou incluir projetos da fila de solicitações ao gravar relatórios.

</br>
</br>

**Prática recomendada**

Crie um status de problema chamado &quot;Rejeitado&quot; ao usar aprovações de problemas e defina a opção Se rejeitado para o status &quot;Rejeitado&quot;.

**Veja o porquê**

Ao usar o status &quot;Rejeitada&quot;, fica claro que a solicitação foi revisada e rejeitada.

</br>
</br>

**Prática recomendada**

Atribua formulários personalizados &quot;universais&quot; às filas de solicitações para capturar o máximo possível de dados consistentes em toda a empresa.

**Veja o porquê**

Um formulário personalizado &quot;universal&quot; coleta as informações padrão necessárias para a solicitação, independentemente do tipo de solicitação que está sendo enviada.

Ter um formulário personalizado &quot;universal&quot; ajuda a reduzir o número de formulários personalizados que você precisa criar e manter. Também garante que todas as solicitações estejam coletando as mesmas informações da mesma maneira, o que leva a relatórios e análises de dados consistentes.

</br>
</br>

**Prática recomendada**

Evite compartilhar filas de solicitações com &quot;todos&quot;.  Defina as configurações de detalhes da fila para que os usuários vejam apenas as filas relevantes às suas necessidades.

**Veja o porquê**

Na maioria dos casos, uma fila de solicitações só precisa ser compartilhada com um determinado conjunto de pessoas, como uma equipe, um fornecedor, clientes etc. Quando os solicitantes veem somente o que precisam na lista da fila de solicitações, facilita a localização e navegação.

</br>
</br>


**Prática recomendada**

Crie e atribua um painel contendo relatórios da fila de solicitações para que os gerenciadores de tráfego, administradores do sistema ou usuários atribuídos possam trabalhar nos problemas diretamente.

**Veja o porquê**

Fornecer aos usuários acesso rápido e fácil às solicitações recebidas significa que o trabalho não é perdido na ordem aleatória.

</br>
</br>

**Prática recomendada**

Use modelos de layout para remover as opções de configuração da fila de solicitações do menu de projetos do painel esquerdo para usuários que não precisam criar filas.


**Veja o porquê**

Isso garante que todas as filas de solicitações passem pelo processo adequado para criação (como serem revisadas por um comitê de governança) e sejam configuradas corretamente por um administrador de sistema ou de grupo.

Além disso, isso ajuda a manter a lista de filas organizada e focada nos tipos de solicitações de que sua organização precisa.

</br>
</br>

**Prática recomendada**

Crie uma fila de solicitações do administrador do sistema para que os usuários façam perguntas relacionadas ao Workfront, solicitações relacionadas às configurações do sistema, agendem treinamento de novos usuários etc.

**Veja o porquê**

Isso fornece um local centralizado para que os usuários enviem perguntas e para que os administradores coletem, monitorem e respondam a problemas relacionados ao Workfront.

Além disso, essas informações podem ser usadas para mostrar liderança, tempo, esforço e valor da função de administrador do sistema e como justificativa para um administrador de sistema adicional.

</br>
</br>


**Prática recomendada**

Auditoria de filas de solicitações regularmente para identificar e cancelar o compartilhamento de filas que não estão sendo usadas.

**Veja o porquê**

Uma auditoria regular das configurações e dos itens no sistema do Adobe Workfront ajuda a mantê-lo livre de itens desnecessários. Se uma fila não estiver mais sendo usada ou monitorada, certifique-se de que os usuários não possam mais acessá-la para que as solicitações de trabalho não se tornem nulas.

</br>
</br>


**Prática recomendada**

Use grupos de tópicos para organizar mais de dez tópicos da fila em uma fila de solicitações para criar listas mais curtas e fáceis de gerenciar.

**Veja o porquê**

Os grupos de tópicos aumentam a adoção de usuários e geram menos confusão ao diminuir a lista inicial de opções para seleção. Isso permite que os usuários encontrem facilmente o que estão procurando, sem sobrecarregá-los ao tentar enviar uma solicitação.

Além disso, permite que os administradores do sistema e/ou gerentes de fila de solicitações criem um caminho de navegação suave para os usuários e uma maneira melhor de organizar e gerar relatórios sobre os tipos de solicitações que estão sendo enviadas.

</br>
</br>

**Prática recomendada**

Controlar o número total de filas de solicitações disponíveis aos usuários detalhando uma fila de solicitações usando grupos de tópicos e tópicos da fila, em vez de criar várias filas.

**Veja o porquê**

Muitas filas de solicitações dificultam a localização do que os usuários precisam.

Menos filas também ajudam coordenadores de tráfego, administradores do sistema ou outras pessoas a gerenciar as filas, permitindo que encontrem as informações de que precisam mais rapidamente, sem precisar navegar para vários projetos de fila de solicitações.

Crie várias filas de solicitações se for necessário um acesso diferente para diferentes filas de solicitações ou se a consolidação de filas for confusa para os usuários.

</br>
</br>

**Prática recomendada**

Configurar regras de roteamento para cada tópico da fila. No mínimo, configure uma regra de roteamento padrão.

**Veja o porquê**

As regras de roteamento garantem que a solicitação recebida seja sempre atribuída a alguém para que o trabalho não seja interrompido.

</br>
</br>

**Prática recomendada**

Aproveite grupos de tópicos e tópicos de fila quando o roteamento seletivo for necessário.

**Veja o porquê**

As regras de roteamento não podem ser aplicadas a campos de um formulário personalizado. Portanto, se diferentes tipos de solicitações precisarem ser encaminhadas a diferentes equipes/indivíduos, faça de cada tipo de solicitação seu próprio tópico de grupo de tópicos/fila para que o trabalho possa ser encaminhado corretamente.

</br>
</br>

**Prática recomendada**

Encaminhar solicitações a uma equipe, em vez de a um indivíduo.

**Veja o porquê**

Quando as solicitações são enviadas à equipe, ela oferece visibilidade de toda a equipe sobre as solicitações que estão sendo feitas e o que pode envolver o trabalho futuro. Todos podem assistir à página Equipe em busca de novos itens ou acompanhar as novidades de um relatório em um painel.

Assegura igualmente que, quando o gestor de tráfego ou outra pessoa responsável pela análise ou atribuição dos pedidos recebidos não estiver disponível, um reserva esteja automaticamente disponível e tenha acesso às informações do pedido.
