# API de agendamentos (Hora Certa)

Playground interativo de uma API de agendamentos que não deixa dois clientes reservarem o mesmo horário.

## O que dá para fazer
- Enviar requisições reais contra a lógica da API: listar horários livres, criar, listar e cancelar agendamentos.
- Provocar erros de propósito e ver os códigos de status: 409 (horário já ocupado, com sugestões de horários livres), 422 (dados inválidos) e 404 (não encontrado).
- Ver a agenda da semana (segunda a sexta, das 9h às 16h) mudar a cada criação ou cancelamento.
- Ver a fila de lembretes por e-mail (24 horas antes de cada agendamento).
- Rodar oito testes automatizados contra a lógica da API.

## Endpoints
| Método | Rota | O que faz |
|---|---|---|
| GET | `/horarios?dia=2` | Lista horários livres de um dia (0 é segunda, 4 é sexta) |
| GET | `/agendamentos` | Lista todos os agendamentos |
| POST | `/agendamentos` | Cria um agendamento |
| DELETE | `/agendamentos/:id` | Cancela e libera o horário |

## Como testar
Abra o `index.html` no navegador, escolha "Forçar conflito" e clique em "Enviar requisição". Depois clique em "Executar testes".

## Tecnologias desta demonstração
HTML, CSS e JavaScript puro. A "API" roda dentro da página, com dados fictícios. Nenhum e-mail é enviado de verdade.

## Versão completa (planejada)
- API REST em Node.js com Express.
- Banco PostgreSQL acessado com Prisma.
- Redis para a fila de lembretes.
- Docker para rodar o ambiente e testes automatizados no pipeline.
