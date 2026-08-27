# Aula 4 — Elicitação de Requisitos

## 1. Processo: Registro de Pedidos

### Requisito 1.1

**O sistema deve permitir que o vendedor registre um novo pedido informando o cliente, os produtos, as quantidades e a forma de pagamento.**

**Fonte 1:** Entrevista com o vendedor.
Fonte humana, nível **operacional**, classe de usuário **vendedor**.

**Fonte 2:** Procedimento comercial para registro de vendas.
Fonte não humana, categoria **documentação**.

---

### Requisito 1.2

**O sistema deve calcular automaticamente o valor total do pedido com base nos produtos e suas respectivas quantidades.**

**Fonte 1:** Entrevista com o vendedor.
Fonte humana, nível **operacional**, classe de usuário **vendedor**.

**Fonte 2:** Tabela de preços dos produtos.
Fonte não humana, categoria **documentação**.

---

### Requisito 1.3

**O sistema deve permitir que o vendedor consulte e confirme os dados do pedido antes de finalizar o registro da venda.**

**Fonte 1:** Entrevista com vendedores responsáveis pelo processo de vendas.
Fonte humana, nível **operacional**, classe de usuário **vendedor**.

**Fonte 2:** Procedimento interno de confirmação de pedidos.
Fonte não humana, categoria **documentação**.

---

# 2. Processo: Cadastro e Remoção de Produtos

### Requisito 2.1

**O sistema deve permitir que o administrador cadastre um produto informando nome, descrição, preço e quantidade inicial em estoque.**

**Fonte 1:** Entrevista com o administrador.
Fonte humana, nível **tático**, classe de usuário **administrador**.

**Fonte 2:** Catálogo de produtos utilizado pela empresa.
Fonte não humana, categoria **documentação**.

---

### Requisito 2.2

**O sistema deve permitir que o administrador remova um produto que não seja mais comercializado.**

**Fonte 1:** Entrevista com o administrador.
Fonte humana, nível **tático**, classe de usuário **administrador**.

**Fonte 2:** Política interna de manutenção do catálogo de produtos.
Fonte não humana, categoria **documentação**.

---

### Requisito 2.3

**O sistema deve impedir que usuários sem permissão de administrador cadastrem ou removam produtos.**

**Fonte 1:** Entrevista com o administrador responsável pelo sistema.
Fonte humana, nível **tático**, classe de usuário **administrador**.

**Fonte 2:** Regras de controle de acesso da empresa.
Fonte não humana, categoria **documentação**.

---

# 3. Processo: Controle de Estoque

### Requisito 3.1

**O sistema deve permitir que o responsável pelo estoque registre a entrada de produtos, informando o produto e a quantidade recebida.**

**Fonte 1:** Entrevista com o responsável pelo estoque.
Fonte humana, nível **operacional**, classe de usuário **estoque**.

**Fonte 2:** Notas fiscais e documentos de recebimento de mercadorias.
Fonte não humana, categoria **documentação**.

---

### Requisito 3.2

**O sistema deve realizar automaticamente a baixa da quantidade disponível em estoque quando um pedido for registrado.**

**Fonte 1:** Entrevista com o responsável pelo estoque.
Fonte humana, nível **operacional**, classe de usuário **estoque**.

**Fonte 2:** Processo atual de controle e baixa de estoque.
Fonte não humana, categoria **documentação**.

---

### Requisito 3.3

**O sistema deve informar a quantidade atual disponível de cada produto para permitir o controle do estoque.**

**Fonte 1:** Entrevista com o responsável pelo estoque.
Fonte humana, nível **operacional**, classe de usuário **estoque**.

**Fonte 2:** Relatório ou planilha atualmente utilizada para controle de estoque.
Fonte não humana, categoria **sistema legado**.

---

# Resumo das Fontes

| Processo            | Requisito | Fonte humana  | Nível / Classe         | Fonte não humana            | Categoria      |
| ------------------- | --------- | ------------- | ---------------------- | --------------------------- | -------------- |
| Registro de pedidos | 1.1       | Vendedor      | Operacional / Vendedor | Procedimento comercial      | Documentação   |
| Registro de pedidos | 1.2       | Vendedor      | Operacional / Vendedor | Tabela de preços            | Documentação   |
| Registro de pedidos | 1.3       | Vendedor      | Operacional / Vendedor | Procedimento de confirmação | Documentação   |
| Cadastro/remoção    | 2.1       | Administrador | Tático / Administrador | Catálogo de produtos        | Documentação   |
| Cadastro/remoção    | 2.2       | Administrador | Tático / Administrador | Política de catálogo        | Documentação   |
| Cadastro/remoção    | 2.3       | Administrador | Tático / Administrador | Regras de acesso            | Documentação   |
| Controle de estoque | 3.1       | Estoquista    | Operacional / Estoque  | Notas fiscais               | Documentação   |
| Controle de estoque | 3.2       | Estoquista    | Operacional / Estoque  | Processo atual              | Documentação   |
| Controle de estoque | 3.3       | Estoquista    | Operacional / Estoque  | Planilha/relatório atual    | Sistema legado |

## Conclusão

Foram identificados **3 processos principais**:

1. **Registro de pedidos**
2. **Cadastro e remoção de produtos**
3. **Controle de estoque**

Para cada processo foram definidos **3 requisitos**, totalizando **9 requisitos de sistema**. Cada requisito possui pelo menos uma fonte humana e uma fonte não humana, permitindo que os requisitos sejam especificados a partir de diferentes perspectivas do negócio.
