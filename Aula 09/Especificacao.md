# Aula 9 — Especificação de caso de uso

## Caso de uso: Solicitar férias

- **Ator principal:** Colaborador.
- **Descrição:** O colaborador informa quando pretende tirar férias e envia o pedido para o gestor analisar.
- **Gatilho:** O colaborador decide solicitar férias.
- **Pré-condição:** O colaborador está autenticado no sistema.
- **Pós-condição:** O pedido fica registrado como aguardando análise e o gestor é avisado.

### Fluxo principal

1. O colaborador escolhe solicitar férias.
2. O sistema mostra o saldo disponível.
3. O colaborador informa a data de início e a quantidade de dias.
4. O sistema verifica se há saldo suficiente.
5. O sistema mostra um resumo do pedido.
6. O colaborador confirma a solicitação.
7. O sistema registra o pedido e avisa o gestor.

### Fluxo alternativo — Vender um terço das férias

No passo 3, o colaborador seleciona a opção de vender um terço das férias. O sistema calcula os dias de férias e os dias vendidos e retorna ao passo 4.

### Fluxo de exceção — Saldo insuficiente

No passo 4, se o colaborador não tiver dias suficientes, o sistema informa quantos dias estão disponíveis e retorna ao passo 3 para ajustar a solicitação.
