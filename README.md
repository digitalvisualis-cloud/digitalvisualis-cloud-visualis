# Visualis Digital — Squad de Agência

Squad de 15 agentes de IA que operam como uma agência completa de automação, CRM e marketing digital para PMEs brasileiras. Inspirado no [OpenSquad](https://github.com/renatoasse/opensquad).

## O que é

Um repositório que você abre no **Claude Code** ou **Cowork** e ele vira uma agência completa. 15 especialistas que trabalham em pipeline — do diagnóstico do cliente à operação rodando.

## Agentes

| Dept | Agente | Função |
|---|---|---|
| 🎯 | **Gabi Gerente** | Orquestra tudo, onboarding, distribui tarefas |
| 📊 | **Sara Estratégia** | Plano estratégico, funil, canais |
| 🔍 | **Raquel Research** | Concorrentes, benchmarks, referências |
| 📈 | **Daniel Dados** | Métricas, ROI, relatórios |
| 🤝 | **Clara Cliente** | Retenção, upsell, satisfação |
| 💡 | **Caio Criativo** | Conceitos, hooks, ideias |
| ✍️ | **Carol Copy** | Textos, CTAs, roteiros |
| 📅 | **Pedro Pauta** | Calendário editorial |
| 🎬 | **Victor Vídeo** | Roteiros, briefing produtora |
| 🎨 | **Diana Design** | Direção visual, prompts IA |
| 📢 | **Paula Paid** | Meta Ads, Google Ads |
| 🤖 | **André Automação** | CRM, WhatsApp, n8n |
| 🌐 | **Wesley Web** | Sites, landing pages |
| 📋 | **Patrícia Projeto** | Prazos, entregas |
| 🔎 | **Sofia SEO** | Google Meu Negócio, ranqueamento |

## Nichos suportados

- 🏥 **Saúde** — clínicas, consultórios (regras CFM)
- 🏠 **Imobiliário** — corretores, imobiliárias (CRECI)
- ⚖️ **Advocacia** — escritórios, advogados (OAB)
- 🏪 **Geral** — PMEs, comércio, serviços

## Como usar

### Claude Code
```bash
cd visualis
claude
```
Depois: `/visualis novo Clínica Sorrir`

### Cowork
Abra o projeto apontando pra esta pasta. O `CLAUDE.md` é lido automaticamente.

## Comandos

| Comando | O que faz |
|---|---|
| `/visualis novo [nome]` | Onboarding completo |
| `/visualis conteúdo [cliente]` | Creative + Copy + Calendário |
| `/visualis campanha [cliente]` | Paid Media + Copy + Design |
| `/visualis automação [cliente]` | CRM + WhatsApp + n8n |
| `/visualis site [cliente]` | Web Developer |
| `/visualis seo [cliente]` | SEO + Google Meu Negócio |
| `/visualis vídeo [cliente]` | Video Strategist + briefing PMF |
| `/visualis relatório [cliente]` | Data Analyst |
| `/visualis status [cliente]` | Project Manager |
| `/visualis escalar [cliente]` | Client Success (upsell) |

## Pipeline de onboarding

```
Diagnóstico → Pesquisa → Estratégia → ✅ APROVAÇÃO
                                         ↓
                          ┌──── Trilha Criação ────┐
                          │ Conceito → Copy →      │
                          │ Calendário → Vídeo →   │
                          │ Design → ✅ APROVAÇÃO   │
                          └────────────────────────┘
                          ┌──── Trilha Operação ───┐
                          │ Automação → Site →     │
                          │ SEO → Tráfego →        │
                          │ ✅ APROVAÇÃO            │
                          └────────────────────────┘
                                         ↓
                          Cronograma → KPIs → 🏁 PRONTO
```

4 checkpoints de aprovação. Você valida antes de avançar.

## Estrutura

```
visualis/
├── CLAUDE.md                    ← Lido automaticamente
├── README.md
├── squad-party.csv              ← Registro dos 15 agentes
├── _visualis/
│   ├── core/runner.pipeline.md  ← Motor de execução
│   └── memory/company.md        ← Contexto da agência
├── agents/                      ← 15 definições .agent.md
├── pipeline/
│   ├── pipeline.yaml            ← 17 steps
│   ├── steps/                   ← Instruções por step
│   └── data/                    ← Packs de nicho
├── skills/                      ← Integrações futuras
└── output/                      ← Entregas por cliente
```

## Licença

Uso privado — Visualis Digital.
