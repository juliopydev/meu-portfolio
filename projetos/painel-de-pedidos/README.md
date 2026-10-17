# Painel de pedidos (Casa Brasa)

Demonstração de um painel para uma hamburgueria fictícia acompanhar pedidos em tempo real, da chegada até a entrega.

## O que dá para fazer
- Ver os pedidos em quatro colunas: Novos, Em preparo, Saiu para entrega e Concluídos.
- Avançar cada pedido de etapa pelo botão do cartão.
- Buscar por cliente ou número e filtrar por canal (App, WhatsApp ou Balcão).
- Acompanhar indicadores que se recalculam sozinhos: pedidos do dia, em aberto, faturamento e ticket médio.
- Ver o faturamento por canal em barras.
- Simular novos pedidos, um a um ou de forma contínua com "Pedidos ao vivo".
- Alternar entre tema claro e escuro.

## Como testar
Abra o `index.html` no navegador. Clique em "Simular novo pedido" e depois em "Aceitar pedido" no cartão que aparecer.

## Tecnologias desta demonstração
HTML, CSS e JavaScript puro. Os dados são fictícios e ficam só na memória do navegador: ao recarregar, voltam ao início.

## Versão completa (planejada)
- Front-end em Next.js.
- API em Node.js para criar e atualizar pedidos.
- Banco PostgreSQL para guardar os pedidos.
- Login com níveis de acesso e atualização em tempo real.
