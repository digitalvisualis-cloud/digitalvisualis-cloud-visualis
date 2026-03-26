---
step: "01"
name: "Diagnóstico do Cliente"
type: checkpoint
description: O Pablo fornece os dados do novo cliente para iniciar o onboarding.
---

# 🛑 Checkpoint: Diagnóstico

## Solicitação ao Usuário

🎯 Novo cliente! Preciso de algumas informações:

1. **Nome** da empresa/profissional
2. **Nicho** (saúde / imobiliário / advocacia / geral)
3. **Problema principal** (não aparece / não converte / não escala)
4. **Presença digital atual** (site? Instagram? Google? WhatsApp?)
5. **Orçamento mensal** (faixa)
6. **Objetivo em 90 dias**
7. **Pacote contratado** (Atendimento Inteligente / Operação Organizada / Piloto Automático)

## Ação do Runner
1. Coletar respostas
2. Ativar pack de nicho: carregar `pipeline/data/pack-{nicho}.md`
3. Salvar em `output/{cliente}/{data}/diagnostico.md`
4. Avançar para Step 02
