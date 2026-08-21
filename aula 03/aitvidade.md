# Requisitos Não Funcionais (RNF)

## 1. História de Usuário — Acompanhar o pedido

**História:**
Como cliente, quero acompanhar o status do meu pedido, para saber em que etapa da entrega ele está.

### RNF 1.1 — Atualização do status

O sistema deve atualizar o status do pedido em no máximo **5 segundos** após uma alteração realizada pelo restaurante ou entregador.

**Característica ISO/IEC 25010:** Eficiência de desempenho.

### RNF 1.2 — Clareza das informações

O sistema deve apresentar os status do pedido de forma clara e compreensível, permitindo que o cliente identifique facilmente a etapa atual da entrega.

**Característica ISO/IEC 25010:** Usabilidade.

### RNF 1.3 — Histórico do pedido

O sistema deve manter o histórico dos status do pedido disponível durante todo o período da entrega.

**Característica ISO/IEC 25010:** Confiabilidade.

---

## 2. História de Usuário — Item indisponível

**História:**
Como restaurante, quero marcar um item do cardápio como indisponível, para evitar que clientes façam pedidos de produtos que não estão disponíveis.

### RNF 2.1 — Atualização da disponibilidade

A alteração da disponibilidade de um item deve ser refletida no cardápio dos clientes em no máximo **5 segundos**.

**Característica ISO/IEC 25010:** Eficiência de desempenho.

### RNF 2.2 — Controle de acesso

Apenas usuários com permissão de restaurante poderão alterar a disponibilidade dos itens do cardápio.

**Característica ISO/IEC 25010:** Segurança.

### RNF 2.3 — Consistência da disponibilidade

O sistema deve manter a disponibilidade dos itens corretamente registrada, evitando que um item marcado como indisponível seja disponibilizado incorretamente.

**Característica ISO/IEC 25010:** Confiabilidade.

---

## 3. História de Usuário — Reportar problema na entrega

**História:**
Como entregador, quero reportar um problema durante a entrega, para informar o restaurante e o cliente sobre a situação do pedido.

### RNF 3.1 — Facilidade de uso

O entregador deve conseguir registrar um problema em no máximo **3 etapas** dentro do aplicativo.

**Característica ISO/IEC 25010:** Usabilidade.

### RNF 3.2 — Registro da ocorrência

Após o envio do problema, o sistema deve registrar a ocorrência e disponibilizá-la ao restaurante em no máximo **5 segundos**.

**Característica ISO/IEC 25010:** Eficiência de desempenho.

### RNF 3.3 — Segurança do registro

Somente o entregador responsável pelo pedido poderá registrar ou alterar uma ocorrência relacionada àquela entrega.

**Característica ISO/IEC 25010:** Segurança.

---

## Resumo

| História            | RNF     | Característica ISO/IEC 25010 |
| ------------------- | ------- | ---------------------------- |
| Acompanhar o pedido | RNF 1.1 | Eficiência de desempenho     |
| Acompanhar o pedido | RNF 1.2 | Usabilidade                  |
| Acompanhar o pedido | RNF 1.3 | Confiabilidade               |
| Item indisponível   | RNF 2.1 | Eficiência de desempenho     |
| Item indisponível   | RNF 2.2 | Segurança                    |
| Item indisponível   | RNF 2.3 | Confiabilidade               |
| Reportar problema   | RNF 3.1 | Usabilidade                  |
| Reportar problema   | RNF 3.2 | Eficiência de desempenho     |
| Reportar problema   | RNF 3.3 | Segurança                    |

**Total: 9 requisitos não funcionais (RNF), sendo 3 para cada história de usuário.**
