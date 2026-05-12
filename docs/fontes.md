# Fontes citadas na talk

> Bibliografia completa, validada via web search durante a construção do deck.

---

## Diagnóstico (slides 4–7)

### METR — Gap percepção × realidade

**Becker, J., Rush, N., Barnes, E., & Rein, D.** (2025). _Measuring the Impact of Early-2025 AI on Experienced Open-Source Developer Productivity_. arXiv preprint **arXiv:2507.09089**.

- 🔗 Paper: https://arxiv.org/abs/2507.09089
- 🔗 Post da METR: https://metr.org/blog/2025-07-10-early-2025-ai-experienced-os-dev-study/
- Metodologia: RCT (randomized controlled trial) com 16 devs experientes, 246 tarefas em projetos open source maduros (média 5 anos de contribuição, 23k stars)
- Achados-chave:
  - Devs **esperavam** ganho de **+24%** com IA
  - Após usar, **achavam** que ganharam **+20%**
  - Realidade medida: **-19%** (foram MAIS LENTOS)
  - Gap percepção × realidade ≈ **39 pontos percentuais**

---

### Faros AI — Acceleration Whiplash

**Faros AI** (2026). _The AI Engineering Report 2026: The Acceleration Whiplash_.

- 🔗 Relatório: https://www.faros.ai/research/ai-acceleration-whiplash
- 🔗 Blog: https://www.faros.ai/blog/ai-acceleration-whiplash-takeaways
- Metodologia: Telemetria real de **22.000 desenvolvedores** em **4.000 times**, comparando períodos de baixa vs alta adoção de IA dentro de cada organização
- Achados positivos:
  - Épicos completados por dev: **+66%**
  - Task throughput: **+34%**
  - PRs por dev (daily contexts): **+67%**
- Achados negativos (downstream):
  - Tempo de review de PR: **+441%** (mediana)
  - Incidentes por PR: **+242,7%**
  - Bugs por desenvolvedor: **+54%**
  - PRs mergeados sem review: **+31,3%**

---

### Ehsani et al. — Por que PRs agênticos falham

**Ehsani, R., Pathak, S., Rawal, S., Al Mujahid, A., Imran, M. M., & Chatterjee, P.** (2026). _Where Do AI Coding Agents Fail? An Empirical Study of Failed Agentic Pull Requests in GitHub_. arXiv preprint **arXiv:2601.15195**.

- 🔗 Paper: https://arxiv.org/abs/2601.15195
- 🔗 HTML: https://arxiv.org/html/2601.15195
- Instituições: Drexel University + Missouri University of Science and Technology
- Metodologia: análise de **33.596 PRs agênticos** em 5 agentes (OpenAI Codex, GitHub Copilot, Devin, Cursor, Claude Code) em repositórios reais do GitHub
- Achados:
  - **71,48%** de taxa geral de merge dos PRs agênticos
  - Por agente: OpenAI Codex 82,59% / Devin moderado / Copilot 43,04%
  - Maior taxa: documentação (84%) / CI (79%) / build (74%)
  - Menor taxa: performance (55%) / fix (64%)
- Análise qualitativa de 600 PRs rejeitados — causas de falha:
  - **38%** Abandono do reviewer (ninguém revisou)
  - **31%** Problemas no PR (duplicação 23%, features indesejadas 4%)
  - **22%** Problemas no código (CI/testes/implementação)
  - **2%** Específicos do agente

---

## P1 · Context Rot (slide 11)

### Chroma Research — Context Rot

**Chroma Research** (Jul/2025). _Context Rot: How Increasing Input Tokens Impacts LLM Performance_.

- 🔗 Estudo: https://research.trychroma.com/context-rot
- Metodologia: testou **18 modelos SOTA** com inputs variando de 10k até 100k tokens
- Achados:
  - Queda de **20–50%** de acurácia entre 10k e 100k tokens
  - Comportamento persiste mesmo em modelos de "contexto longo" (1M+)

### Liu et al. — Lost in the Middle

**Liu, N. F., Lin, K., Hewitt, J., Paranjape, A., Bevilacqua, M., Petroni, F., & Liang, P.** (2024). _Lost in the Middle: How Language Models Use Long Contexts_. **TACL** (Transactions of the Association for Computational Linguistics). arXiv:2307.03172.

- 🔗 Paper: https://arxiv.org/abs/2307.03172
- Achado: curva em **U** da atenção dos LLMs — performance alta no início e no fim do contexto, **rebaixada no meio**

### NoLiMa Benchmark

- 11 de 12 modelos avaliados ficam **abaixo de 50% de acurácia** com 32k tokens de contexto

---

## P2 · DORA (slide 18)

### DORA — DevOps Research and Assessment

**Forsgren, N., Humble, J., & Kim, G.** (2018). _Accelerate: The Science of Lean Software and DevOps_. IT Revolution Press.

- 🔗 Site oficial: https://dora.dev
- 🔗 Estado anual: https://cloud.google.com/devops/state-of-devops
- 10+ anos de pesquisa, centenas de organizações
- 4 métricas core:
  1. **Lead Time** — tempo da alteração de código até produção
  2. **Deployment Frequency** — frequência de entregas
  3. **Change Failure Rate** — % de deploys que falham
  4. **Recovery Time** — tempo para restaurar após incidente

### DORA Report 2025

Conclui que "engineering foundations sólidos amplificam benefícios de IA e protegem contra downsides" — mas o **Faros AI 2026 contesta** com dados de telemetria de que times com alta maturidade DORA enfrentam a mesma deterioração downstream.

---

## P2 · Caso Meta · Claudeonomics (slide 17)

### The Information

**The Information** (Abr/2026). Reportagem original que revelou o leaderboard interno "Claudeonomics" da Meta.

- Disponível via paywall em https://www.theinformation.com

### The Pragmatic Engineer — Tokenmaxxing

**Orosz, G.** (Abr/2026). _The Pulse: 'Tokenmaxxing' as a weird new trend_. **The Pragmatic Engineer Newsletter**.

- 🔗 Post: https://newsletter.pragmaticengineer.com/p/the-pulse-tokenmaxxing-as-a-weird-6b2
- 🔗 Mirror: https://blog.pragmaticengineer.com/the-pulse-tokenmaxxing-as-a-weird-new-trend/
- Entrevistas com engenheiros da Meta, Microsoft, Salesforce
- Cunhou o uso popular do termo **"tokenmaxxing"** no setor

### Fortune

**Fortune** (Abr/2026). _A Meta employee created a dashboard so coworkers can compete to be the company's No. 1 AI token user—and Zuckerberg doesn't even rank in the top 250_.

- 🔗 https://fortune.com/2026/04/09/meta-killed-employee-ai-token-dashboard/

### The Decoder

**The Decoder** (Abr/2026). _Meta employees compete for token consumption on an internal AI leaderboard_.

- 🔗 https://the-decoder.com/meta-employees-compete-for-token-consumption-on-an-internal-ai-leaderboard/

### Dados-chave (estimados)

⚠ Todos os números abaixo são **estimativas apuradas por jornalistas a partir de relatos internos**. Meta nunca confirmou oficialmente.

- ~85.000 engenheiros rankeados no leaderboard
- **~60 trilhões** de tokens consumidos em 30 dias
- **~281 bilhões** de tokens só do top user em 1 mês
- **~US$ 900M** custo estimado a preço de API da Anthropic (Meta provavelmente paga menos)
- Top user médio: 281B tokens
- Títulos do leaderboard: "Token Legend", "Cache Wizard", "Model Connoisseur", "Session Immortal"
- Leaderboard removido **2 dias após** história vazar
- Microsoft tem leaderboard similar **desde janeiro/2026**
- Salesforce: widget no Mac que atualiza spend a cada 15 minutos · meta mínima de US$ 100 Claude Code + US$ 70 Cursor / engenheiro / mês
- **Jensen Huang (Nvidia)**: declarou estar "deeply alarmed" se um eng. de $500k/ano não gastar pelo menos $250k em tokens

---

## P2 · Ralph Loop / referências de processo (slide 12)

### Ralph (snarktank/ralph)

- 🔗 https://github.com/snarktank/ralph
- Repositório público de referência usado como base do framework adotado na StartSe

### Frameworks complementares mencionados

- **GSD** — Get Shit Done (filosofia de execução)
- **SDD** — Spec-Driven Development
- **BMAD** — Framework comunitário
- **Compozy** — Orquestração de workflows com agentes

---

## Citações diretas usadas no deck

> "Token consumption is an input metric, not an output metric. (...) A proxy for a proxy."
> — Análise crítica do Claudeonomics (Vucense, Abr/2026)

> "I'd be deeply alarmed if an engineer pulling in $500,000 a year wasn't consuming at least $250,000 worth of tokens."
> — **Jensen Huang**, CEO Nvidia, Mar/2026

---

## Como verificar / atualizar fontes

Todas as fontes foram validadas via busca pública até **Maio/2026**. Se for usar a talk em datas posteriores, vale revalidar especialmente:

- Os números do Faros AI (eles publicam relatório anualmente)
- O caso Meta · Claudeonomics (status atual do leaderboard, novas reportagens)
- Estudos METR posteriores (eles planejam refazer o experimento periodicamente)
