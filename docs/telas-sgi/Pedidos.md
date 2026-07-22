# Tela de Pedidos

Documentação da tela de gerenciamento de pedidos do sistema SGI.

## Visão geral

A tela de Pedidos permite visualizar, criar, editar e acompanhar o status de
todos os pedidos registrados no sistema.

![Tela de Pedidos](../assets/imagens/exemplo.png)

## Onde encontrar

`Menu Principal > Vendas > Pedidos`

## Campos da tela

| Campo | Descrição | Obrigatório |
|---|---|---|
| Número do Pedido | Gerado automaticamente pelo sistema | Sim |
| Cliente | Cliente vinculado ao pedido | Sim |
| Data do Pedido | Data de criação | Sim |
| Status | Pendente, Em Andamento, Concluído, Cancelado | Sim |
| Valor Total | Calculado com base nos itens | Automático |
| Forma de Pagamento | À vista, Parcelado, Boleto, etc | Sim |

## Como criar um novo pedido

1. Clique no botão **"Novo Pedido"** no canto superior direito
2. Selecione o cliente (ou cadastre um novo)
3. Adicione os itens do pedido
4. Escolha a forma de pagamento
5. Clique em **"Salvar"**

!!! tip "Dica"
    Use `Ctrl + N` como atalho para abrir um novo pedido rapidamente.

## Status possíveis

- 🟡 **Pendente** — pedido criado, aguardando processamento
- 🔵 **Em Andamento** — pedido sendo preparado/processado
- 🟢 **Concluído** — pedido finalizado com sucesso
- 🔴 **Cancelado** — pedido cancelado pelo cliente ou pela equipe

## Erros comuns

!!! warning "Atenção"
    Se o pedido não salvar, verifique se todos os campos obrigatórios foram
    preenchidos e se o cliente selecionado está ativo no sistema.

## Perguntas frequentes sobre essa tela

**Posso editar um pedido já concluído?**
Não diretamente. É necessário reabrir o pedido através do botão "Reabrir",
disponível apenas para usuários com permissão de supervisor.

**Como cancelar um pedido?**
Abra o pedido, clique em "Ações" > "Cancelar Pedido", e informe o motivo do
cancelamento.