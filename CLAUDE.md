# Visualis Digital — Instruções do Projeto

Este projeto é a **Visualis Digital**, uma agência de automação, CRM e marketing digital para PMEs brasileiras. Funciona como um squad de 14 agentes especializados que executam em pipeline.

## Quick Start

Digite `/visualis` para abrir o menu principal, ou use:
- `/visualis novo [nome do cliente]` — Inicia onboarding completo
- `/visualis run [cliente]` — Executa o pipeline para um cliente
- `/visualis status [cliente]` — Mostra o andamento
- `/visualis help` — Lista todos os comandos

## Estrutura

- `_visualis/` — Core da agência (não editar manualmente)
- `_visualis/core/` — Runner do pipeline + best practices por nicho
- `_visualis/memory/` — Contexto da agência (stack, pacotes, identidade)
- `agents/` — Definições dos 14 agentes especializados
- `pipeline/` — Pipeline de execução + steps + dados de nicho
- `skills/` — Skills instaladas (integrações, templates)
- `output/` — Entregas geradas por cliente

## Como funciona

1. O `/visualis` é o ponto de entrada
2. O **Gerente** faz o diagnóstico e monta o pipeline
3. O **Pipeline Runner** executa step by step
4. Agentes se comunicam por handoff (um entrega pro próximo)
5. Checkpoints pausam pra aprovação do Pablo
6. Output vai pra `output/{cliente}/{data}/`

## Regras

- Sempre use `/visualis` pra interagir com o sistema
- Não edite `_visualis/core/` manualmente
- Agentes podem ser editados em `agents/` se precisar ajustar
- Contexto da agência em `_visualis/memory/company.md` é carregado em toda execução
- Todo output é salvo em `output/` organizado por cliente e data
- Fale sempre em PT-BR, direto, sem enrolação
