---
title: Prática recomendada - Licenças e níveis de acesso
description: Explore as sugestões de práticas recomendadas dos especialistas da Adobe Workfront sobre como configurar, gerenciar e usar licenças e níveis de acesso do Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10914
exl-id: 6be3fab9-16a1-4ab9-89ce-8c53f8358e62
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '1253'
ht-degree: 100%

---

# Prática recomendada - Licenças e níveis de acesso

## O que é uma “prática recomendada” do Adobe Workfront?

As práticas recomendadas são diretrizes para um curso de ação eficaz e eficiente; elas podem ser facilmente adotadas por qualquer usuário da empresa e replicadas com sucesso em toda a organização.

Ao revisar essas recomendações, lembre-se de que algumas práticas recomendadas do Workfront são universais, enquanto outras podem ser mais específicas para um determinado assunto. Use essas práticas recomendadas como uma base para orientar as configurações e o uso do sistema do Workfront.

## Navegar nesta página

Ao percorrer esta página, você encontrará primeiro uma lista resumida de todas as práticas recomendadas para o tópico. Isso permite revisar as recomendações sem se aprofundar nos detalhes e motivos por trás delas.

A seção “Por que essas práticas são recomendadas?” , encontrada após a lista resumida, fornece mais detalhes sobre algumas práticas recomendadas e por que elas são consideradas como um processo, ferramenta ou recurso que você deve considerar implementar na sua instância do Workfront.

</br>
</br>

## Práticas recomendadas para licenças e níveis de acesso

* Comece com menos acesso para os usuários ao configurar os níveis de acesso.

* Ao atribuir licenças de Revisão e Solicitação, normalmente, opte como padrão pela Revisão, pois ela fornece ao usuário mais permissões no Adobe Workfront.

* Desmarque a caixa de seleção “Compartilhar em todo o sistema” de cada objeto em todos os níveis de acesso, a menos que você deseje especificamente que esses usuários possam fazer isso.

* Considere ativar a configuração “Nunca permitir que os usuários excluam comentários” em Definir restrições adicionais em um nível de acesso.

* Limite o número de administradores do sistema a favor de administradores de grupo.

* Copie um nível de acesso já existente e faça modificações, em vez de criar um novo nível do zero.

* Documente o que cada nível de acesso pode fazer na caixa Descrição.

* Limite-se apenas aos níveis de acesso necessários para atingir suas metas de trabalho, idealmente quatro ou cinco, que atendam às necessidades da maioria dos usuários do sistema.

* Atribua pelo menos dois usuários ao nível de acesso de administrador global do sistema.

* Restrinja o que os usuários podem fazer com itens do Workfront por meio do compartilhamento, em vez de remover um recurso em um nível de acesso.

</br>
</br>


## Por que essas práticas são recomendadas?

**Prática recomendada**

Comece com menos acesso para os usuários ao configurar os níveis de acesso.



**Entenda o porquê**

Inicie os usuários com o acesso mínimo necessário para realizar seu trabalho. Se eles não conseguirem realizar seus trabalho devido a direitos de acesso insuficientes, geralmente solicitarão acesso adicional. Conceder muito acesso aos usuários de imediato pode levar a problemas de segurança. Além disso, é sempre melhor conceder aos usuários mais acesso do que remover.

</br>
</br>



**Prática recomendada**

Ao atribuir licenças de Revisão e Solicitação, normalmente, opte como padrão pela Revisão, pois ela fornece ao usuário mais permissões no Adobe Workfront.



**Entenda o porquê**

Embora as licenças Revisão e Solicitação possam ser atribuídas a um número ilimitado de usuários no Workfront, as licenças de Solicitação são limitadas a apenas fazer e atualizar solicitações. Uma licença de Revisão possui mais acesso a projetos e tarefas do que uma licença de Solicitação, bem como a possibilidade de visualizar portfólios e programas, editar documentos e acessar ferramentas de gerenciamento de recursos.

</br>
</br>

**Prática recomendada**

Desmarque a caixa de seleção “Compartilhar em todo o sistema” em cada objeto em todos os níveis de acesso, a menos que haja um motivo específico para que os usuários precisem compartilhar em todo o sistema.



**Entenda o porquê**

Compartilhar um objeto em todo o sistema costuma ser usado como uma muleta para permitir que determinados usuários vejam itens no Workfront. Isso acontece quando a estrutura de grupo do Workfront é insuficiente ou quando as permissões de compartilhamento não são totalmente compreendidas. Quando os itens são compartilhados em todo o sistema, significa que todos podem ver o item compartilhado. Dependendo do tipo de informação que está sendo mantida no sistema, isso pode levar a problemas de privacidade.



Por exemplo, você pode trabalhar com vários fornecedores dentro do Workfront para verificar o progresso, fornecer aprovações etc. Se a caixa de seleção “Compartilhar em todo o sistema” for uma opção, ela poderá ser selecionada ou definida como padrão, disponibilizando informações para todos os fornecedores.



Ao desmarcar a opção completamente, você faz com que um usuário, com permissão para compartilhar, deva determinar a pessoa ou pessoas específicas (seja por meio de uma empresa, grupo ou equipe) com as quais deseja compartilhar o objeto.

</br>
</br>

**Prática recomendada**

Considere ativar a configuração “Nunca permitir que os usuários excluam comentários” em Definir restrições adicionais em um nível de acesso.



**Entenda o porquê**

Ativar esta opção garante que as comunicações anteriores não sejam removidas do Workfront. Algumas organizações exigem que o histórico completo de comentários seja mantido para fins de auditoria.

</br>
</br>

**Prática recomendada**

Limite o número de administradores do sistema a favor de administradores de grupo.



**Entenda o porquê**

Os administradores do sistema têm acesso a tudo no Workfront, incluindo configurações globais do sistema. As configurações que os administradores de grupos podem acessar são controladas pelo administrador do sistema e se aplicam somente a esse grupo específico.



Quando a empresa conta com administradores de grupo, os administradores de sistema podem delegar várias responsabilidades, permitindo que eles se concentrem em itens mais amplos, em vez de na manutenção diária do Workfront. Os administradores de grupo podem manter contato com mais facilidade com as necessidades de seus grupos, o que proporciona um melhor serviço aos usuários.

</br>
</br>


**Prática recomendada**

Copie um nível de acesso já existente e faça modificações, em vez de criar um novo nível do zero.



**Entenda o porquê**

Copiar um nível de acesso já existente fornece uma base consistente para novos níveis de acesso, garantindo que as configurações iniciais sejam idênticas. Isso também economiza tempo, pois os administradores do sistema não precisarão configurar um nível de acesso totalmente do zero.

</br>
</br>

**Prática recomendada**

Documente o que cada nível de acesso pode fazer na caixa Descrição.



**Veja o porquê**

Seja detalhado com a descrição, listando quais são as configurações para cada tipo de objeto. Isso ajuda os administradores de sistemas, atuais e futuros, a saber exatamente o que cada nível de acesso faz sem precisar se aprofundar no próprio nível de acesso para analisar as configurações.



Isso também pode facilitar a comparação dos níveis de acesso ao analisá-los num relatório. O campo de descrição pode ser adicionado rapidamente à visualização para ver facilmente como eles diferem e, possivelmente, por que um nível de acesso diferente foi criado.

</br>
</br>

**Prática recomendada**

Limite-se apenas aos níveis de acesso necessários para atingir suas metas de trabalho, idealmente quatro ou cinco, que atendam às necessidades da maioria dos usuários do sistema.


**Veja o porquê**

O nível de acesso garante que quando um objeto do Workfront é compartilhado com um usuário, o usuário tenha os direitos necessários para editá-lo, excluí-lo etc. Você pode tornar os níveis de acesso mais gerais, pois o compartilhamento em itens individuais pode ser configurado de maneira mais específica.


Além disso, ter menos níveis de acesso pode facilitar a manutenção de um sistema organizado e a implementação de uma estratégia, o que também pode resultar em uma integração mais rápida quando as pessoas ingressarem na empresa ou mudarem de departamento.

</br>
</br>

**Prática recomendada**

Atribua pelo menos dois usuários ao nível de acesso de administrador global do sistema.

**Veja o porquê**

Mais de uma pessoa deve entender por que o Workfront foi configurado daquela maneira, como gerenciá-lo/mantê-lo e como oferecer suporte aos usuários. Se uma pessoa estiver ausente, sair da organização, estiver ocupada etc., isso garante que haja outra pessoa com as informações e o conhecimento necessários para gerenciar o sistema com êxito.

</br>
</br>

**Prática recomendada**

Restrinja o que os usuários podem fazer com itens do Workfront por meio do compartilhamento, em vez de remover um recurso em um nível de acesso.


**Veja o porquê**

Os níveis de acesso controlam o que os usuários podem fazer com itens específicos em nível global. As permissões de compartilhamento em cada projeto, tarefa, portfólio, documento etc. controlam o que um usuário individual pode fazer com aquele item específico. Em vez de remover um recurso para todos com um nível de acesso específico, ajuste as permissões de compartilhamento em itens específicos para que os usuários tenham controles limitados.
