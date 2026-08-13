# Making History

## 1. Acompanhar o pedido

**História de usuário:**
Como **cliente**, quero **acompanhar o status do meu pedido**, para **saber em que etapa da entrega ele está**.

**Critérios de aceitação:**

* **Dado** que o cliente realizou um pedido, **quando** acessar a tela de acompanhamento, **então** deverá visualizar o status atual do pedido.
* **Dado** que o pedido está em preparação, **quando** o restaurante atualizar o status, **então** o cliente deverá visualizar a nova etapa.
* **Dado** que o pedido foi enviado para entrega, **quando** o entregador iniciar a entrega, **então** o status deverá ser atualizado para "Em entrega".

---

## 2. Avisar sobre item indisponível

**História de usuário:**
Como **restaurante**, quero **marcar um item do cardápio como indisponível**, para **evitar que clientes façam pedidos de produtos que não estão disponíveis**.

**Critérios de aceitação:**

* **Dado** que um item está disponível no cardápio, **quando** o restaurante marcá-lo como indisponível, **então** o item deverá aparecer como indisponível para os clientes.
* **Dado** que um item está marcado como indisponível, **quando** um cliente visualizar o cardápio, **então** ele não deverá conseguir adicionar esse item ao pedido.
* **Dado** que o item voltou a estar disponível, **quando** o restaurante alterar seu status, **então** o item deverá voltar a poder ser selecionado pelos clientes.

---

## 3. Reportar problema durante a entrega

**História de usuário:**
Como **entregador**, quero **reportar um problema durante a entrega**, para **informar o restaurante e o cliente sobre a situação do pedido**.

**Critérios de aceitação:**

* **Dado** que o entregador está realizando uma entrega, **quando** ocorrer um problema, **então** ele deverá conseguir acessar a opção de reportar problema.
* **Dado** que o entregador selecionou a opção de reportar problema, **quando** informar o motivo, **então** o sistema deverá registrar a ocorrência vinculada ao pedido.
* **Dado** que um problema foi registrado, **quando** o registro for concluído, **então** o restaurante deverá receber uma notificação sobre a ocorrência.

---

# Priorização — MoSCoW

## MUST HAVE — Deve ter

Funcionalidades indispensáveis para o aplicativo funcionar corretamente:

1. **Cliente acompanhar o status do pedido.**
2. **Restaurante marcar item como indisponível.**
3. **Entregador reportar problema durante a entrega.**
4. **Sistema atualizar o status do pedido.**
5. **Sistema registrar problemas vinculados ao pedido.**

## SHOULD HAVE — Deveria ter

Funcionalidades importantes, mas que não impedem o funcionamento básico:

1. **Notificar o cliente quando o status do pedido mudar.**
2. **Notificar o restaurante quando o entregador reportar um problema.**
3. **Permitir que o restaurante altere novamente um item para disponível.**

## COULD HAVE — Poderia ter

Funcionalidades que melhorariam a experiência, mas não são essenciais:

1. **Exibir uma estimativa de tempo para a entrega.**
2. **Permitir que o entregador adicione uma descrição detalhada ou foto do problema.**
3. **Exibir um histórico das ocorrências do pedido.**

## WON'T HAVE — Não terá neste momento

Funcionalidades que podem ficar para versões futuras:

1. **Rastreamento do entregador em tempo real pelo mapa.**
2. **Sistema automático de previsão de atrasos usando inteligência artificial.**
3. **Chat em tempo real entre cliente, restaurante e entregador.**

### Ordem final de prioridade

**1º — Acompanhar pedido → MUST**
**2º — Marcar item indisponível → MUST**
**3º — Reportar problema → MUST**
**4º — Notificações → SHOULD**
**5º — Recursos extras de acompanhamento e registro → COULD**
**6º — Rastreamento em tempo real, IA e chat → WON'T**
