# Skate Flow — Aluguel de Patins

Protótipo de interface para uma loja de aluguel de patins, cobrindo o fluxo operacional completo: dashboard de aluguéis, novo aluguel, encerramento com taxa de danos e fechamento de caixa.

Projeto acadêmico da disciplina de **IHC (Interface Humano-Computador)** — UNIFESO.

## Telas

| Tela | Arquivo | Função |
|---|---|---|
| Dashboard | `index.html` | Visão geral e aluguéis recentes |
| Novo aluguel | `alugar.html` | Registro de um novo aluguel de patins |
| Encerrar aluguel | `encerrar.html` | Devolução, taxa de danos e forma de pagamento |
| Fechar caixa | `fechar-caixa.html` | Relatório de fechamento do caixa |

## Stack

| Área | Tecnologia |
|---|---|
| Marcação | HTML5 |
| Estilização | Tailwind CSS (configuração local em `js/tailwind.config.js`) |
| Comportamento | JavaScript vanilla (`js/encerrar.js`, `js/layout.js`) |

## Como executar

O projeto é estático e sem build. Basta servir a raiz do repositório:

```bash
python -m http.server 5500
```

Acesse `http://localhost:5500`. Alternativa: extensão **Live Server** no VS Code.

## Design

O sistema visual está documentado em [`DESIGN.md`](DESIGN.md) — tema **"Urban Kinetic"**, com paleta, tipografia e tokens de cor definidos para a identidade da loja.

## Estrutura

```text
.
├── index.html            # dashboard
├── alugar.html           # novo aluguel
├── encerrar.html         # encerramento e pagamento
├── fechar-caixa.html     # relatório de fechamento
├── DESIGN.md             # sistema de design
├── css/
├── js/
│   ├── encerrar.js       # cálculo de total e seleção de pagamento
│   ├── layout.js         # comportamento do layout
│   └── tailwind.config.js
└── docs/                 # entregas acadêmicas (PDF/HTML)
```

## Limitações

Protótipo de interface: não há backend, autenticação ou persistência. Os valores exibidos são simulados (aluguel base de R$ 45,00 e taxa de danos de R$ 50,00).

## Documentação acadêmica

A pasta `docs/` reúne as entregas do trabalho de IHC: documentação, apresentação, plano de aulas e o projeto de interface da empresa de patins.

## Autor

Erick Lopes — [LinkedIn](https://www.linkedin.com/in/SEU-USUARIO/) · [GitHub](https://github.com/ErickLopesSC)
