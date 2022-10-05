---
title: Prática recomendada - Projeto, tarefa e preferências de emissão
description: Explore as recomendações de práticas recomendadas dos especialistas do Adobe Workfront sobre como configurar, gerenciar e usar o projeto, a tarefa e as preferências de emissão do Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
kt: 10918
exl-id: 321af897-3791-4b06-a9dd-241b5246b2a0
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 0%

---

# Prática recomendada - Projeto, tarefa e preferências de emissão

## O que é uma &quot;prática recomendada&quot; do Adobe Workfront?

As melhores práticas são orientações que representam uma linha de ação eficaz e eficiente; sejam adotados facilmente por você e pelos usuários em sua empresa; e podem ser replicados com êxito em toda a organização.

À medida que você revisa essas recomendações, lembre-se de que algumas práticas recomendadas do Workfront são universais, enquanto outras podem ser mais específicas para o tópico. Use essas práticas recomendadas como estrutura para ajudar a orientar as configurações e o uso do sistema Workfront.

## Navegar nesta página

Ao rolar por essa página, primeiro você encontrará uma lista de alto nível de todas as práticas recomendadas para o tópico. Isso permite que você revise as recomendações sem entrar nos detalhes de &quot;por quê&quot;.

O &quot;Por que essas práticas recomendadas estão sendo usadas?&quot; , encontrada após a lista de alto nível, fornece mais detalhes sobre algumas práticas recomendadas e por que elas são consideradas como um processo, ferramenta etc., você deve considerar a implementação com sua instância do Workfront.

</br>
</br>

## Práticas recomendadas de preferências de projeto, tarefa e emissão

* Defina o tipo padrão de duração da tarefa como Simples.

* Defina a preferência do status de um novo projeto como Planejamento ou Ideia, não Atual.

* Ative Criar linhas de base automaticamente nas preferências do projeto global.

* Marque todas as opções na seção Casos de negócios das preferências do projeto do sistema.

* Nas preferências de problemas, marque a opção para Atualizar automaticamente o status de problema resolvível quando o status do objeto de resolução for alterado.

</br>
</br>


## Por que essas práticas recomendadas estão presentes?

**Prática recomendada**

Defina o tipo padrão de duração da tarefa como Simples.

**Veja o porquê**

Os tipos de duração definem a relação entre a duração da tarefa, as horas planejadas e o número de pessoas atribuídas à tarefa.

Com Simples como padrão do sistema global, todas as tarefas criadas manualmente têm esse tipo de duração. As horas planejadas são divididas igualmente entre os designados de tarefa durante a duração. O tipo Simple duration pode simplificar o planejamento do projeto, pois permite fazer alterações nos destinatários da tarefa e nas horas planejadas sem afetar a duração da tarefa, a data de início planejada ou a data de conclusão planejada.

</br>
</br>

**Prática recomendada**

Defina a preferência do status de um novo projeto como Planejamento ou Ideia, não Atual.

**Veja o porquê**

Um status Atual indica que um projeto está ativo e o trabalho está sendo feito ativamente. É raro um projeto precisar estar nesse status ao criar. Mesmo que você use um modelo de projeto, há algum &quot;planejamento&quot; envolvido em obter atribuições de tarefa feitas, ajustando a data de conclusão planejada do projeto etc. O status do Planning também suprime notificações para os destinatários da tarefa e membros da equipe do projeto. Receber notificações antes que o projeto esteja ativo pode ser confuso para os envolvidos.

</br>
</br>

**Prática recomendada**

Ative Criar linhas de base automaticamente nas preferências do projeto global.

**Veja o porquê**

Toda vez que você altera o status de um projeto para Atual, o Workfront registra automaticamente a linha de base de um projeto. Este &quot;instantâneo&quot; do projeto fornece informações históricas sobre como o plano do projeto foi alterado ao longo do tempo. Por exemplo, você pode comparar o plano de projeto original com o plano atual ao mostrar à liderança como a mudança de prioridades ou o desnível de escopo afetaram os prazos do projeto.

</br>
</br>

**Prática recomendada**

Marque todas as opções na seção Casos de negócios das preferências do projeto do sistema.

**Veja o porquê**

Habilite todas as cinco opções para permitir que gerentes de projeto, planejadores e outras pessoas incluam qualquer uma dessas seções no caso comercial de um projeto. Se as opções não estiverem ativadas, então elas não aparecerão na janela do caso comercial. Os usuários podem deixar qualquer um dos campos em branco se não for necessário para esse projeto específico, mas não podem ativar um campo no nível do projeto. Essas opções só podem ser ativadas globalmente na Configuração.

</br>
</br>

**Prática recomendada**

Nas preferências de problemas, marque a opção para Atualizar automaticamente o status de problema resolvível quando o status do objeto de resolução for alterado.

**Veja o porquê**

Quando um problema é convertido em um projeto, essa configuração de preferência &quot;vincula&quot; os status dos dois itens. Atualizar o status do projeto (o objeto de resolução) atualizará automaticamente o status do problema. Isso significa que o solicitante pode ver o progresso sendo feito em sua solicitação, mesmo que ele não tenha permissões para ver todo o projeto no Workfront.
