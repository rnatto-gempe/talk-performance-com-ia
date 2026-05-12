# Outline dos slides

> 28 slides · ~45 minutos · estrutura em 3 blocos (Diagnóstico → P1 → P2 → P3 → Fechamento)

---

## Bloco 0 · Abertura (slides 1–3)

| # | Slide | Tipo | Objetivo |
|---|---|---|---|
| 1 | **Capa** | Título cheio | Provocação central: "Você acha que está sendo produtivo com IA. Mas está?" |
| 2 | **Apresentação** | 4 cards | Renato Barbosa · Head de Engenharia & Sócio · Generalista / Open Source / Consultoria IA 2+ anos / Inovação |
| 3 | **Índice** | 3 cards | As 3 perguntas operacionais |

## Bloco 1 · Diagnóstico (slides 4–7)

| # | Slide | Tipo | Destaque |
|---|---|---|---|
| 4 | **METR** | 3 cards · reveal progressivo (4 steps) | Gap percepção × realidade · 24% → 20% → **-19%** |
| 5 | **Faros AI** | Bars · reveal progressivo (4 steps) | Acceleration Whiplash · positivos verde → "Mas isso é produtividade?" → DEPENDE + negativos |
| 6 | **Ehsani et al.** | Bars horizontais | 71,48% PRs mergeados + 4 causas de falha (38% / 31% / 22% / 2%) |
| 7 | **Síntese** | Frase âncora | Entregar ≠ Produtividade |

## Bloco 2 · P1 — Como definimos um processo (slides 8–14)

| # | Slide | Tipo | Destaque |
|---|---|---|---|
| 8 | **Abertura P1** | Chat demo + 3 cards reveal | **Demo animada de 40s** com 15 mensagens de babysitting + barra de contexto crescendo |
| 9 | **Inimigo 1 · Não-replicável** | 2 cards lado a lado | Prompt não escala |
| 10 | **Inimigo 2 · Babysitting** | 2 cards (problema + solução) | Mudar de USO da IA para TRABALHO COM agentes |
| 11 | **Inimigo 3 · Context Rot** | Curva U SVG + checklist | Chroma, Lost in the Middle |
| 12 | **Ralph Loop** | Quote + frameworks | Spec-driven + GSD/SDD/BMAD/Compozy |
| 13 | **Como funciona** | 4 step cards | Planejar → Validar plano → Solicitar → Validar |
| 14 | **Na prática** | 3 cards + terminal + aviso | Skills `/prd` `/ralph` + `./ralph.sh --tool claude 15` + ⚠ `dangerously-skip-permissions` |

## Bloco 3 · Transição P1 → P2 (slide 15)

| # | Slide | Tipo | Destaque |
|---|---|---|---|
| 15 | **Transição** | Frase âncora + mini-roadmap | "Agora, como medimos se está funcionando?" · P1 ✓ · P2 ⟶ · P3 ___ |

## Bloco 4 · P2 — Como mensuramos performance (slides 16–19)

| # | Slide | Tipo | Destaque |
|---|---|---|---|
| 16 | **Painel do vendor** | Gráfico SVG + bignum | **Meus 2,5B tokens em 30 dias** vs 5 devs do time (1B / 320M / 290M / 240M / 150M) |
| 17 | **Caso Meta** | 3 bignums + 2 cards | **Claudeonomics** · ~60T tokens · ~US$ 900M · **Tokenmaxxing** |
| 18 | **DORA Metrics** | 4 metric cards | Lead Time / Deployment Frequency / Change Failure Rate / Recovery Time |
| 19 | **Dev Fluency** | 4 metric cards + quote | Criação skills / Qualidade especificação / % background / Paralelismo |
| 20 | **Ralph Console** | Tabela comparativa | DORA + Dev Fluency = decisão (não vaidade) |

## Bloco 5 · Intermediário (slide 21)

| # | Slide | Tipo | Destaque |
|---|---|---|---|
| 21 | **Recapitulando** | 3 recap rows | P1 ✓ Ralph Loop · P2 ✓ Ralph Console · P3 ??? |

## Bloco 6 · P3 — Alinhamento estratégico (slides 22–24)

| # | Slide | Tipo | Destaque |
|---|---|---|---|
| 22 | **Abertura P3** | 2 cards antes/depois | Skill `/tech-manager` · não precisa estar nas dailies, precisa da transcrição |
| 23 | **Anatomia da skill** | Code block + checklist | Corpo + 6 passos do pipeline diário |
| 24 | **Operacional** | 2 cards lado a lado | Estrutura do board + formato do relatório semanal |

## Bloco 7 · Fechamento (slides 25–28)

| # | Slide | Tipo | Destaque |
|---|---|---|---|
| 25 | **Pra levar pra casa** | Numbered list | 3 takeaways (processo / fuja de tokens / acompanhe evolução) |
| 26 | **Fechamento do ciclo** | Frase em prosa | Resposta à pergunta-título da capa |
| 27 | **Conecte-se** | 3 QR cards | LinkedIn / Ralph Console waitlist / Bússola Executiva |
| 28 | **Obrigado** | Frase cheia | Obrigado · Excelente evento |

---

## Slides com reveal progressivo (data-steps)

| # | Slide | Steps | Atalho |
|---|---|---|---|
| 4 | METR | 4 | → revela expectativa → percepção → realidade → gap |
| 5 | Faros AI | 4 | → revela "Sim!" → positivos → "Mas isso é produtividade?" → "DEPENDE..." + negativos |
| 8 | P1 abertura (chat demo) | 2 | → revela frase de transição → 3 cards-problema |

Em todos os outros slides, a seta direita avança direto pro próximo slide.

---

## Slides com animação em loop

| # | Slide | Animação |
|---|---|---|
| 8 | Chat demo do jeito tradicional | 15 mensagens em sequência, ~40s total, com auto-scroll do chat-body e barra de contexto enchendo |

---

## Tempo estimado por bloco

| Bloco | Tempo |
|---|---|
| Abertura (1-3) | 2 min |
| Diagnóstico (4-7) | 8 min |
| P1 (8-14) | 12 min |
| Transição (15) | 1 min |
| P2 (16-20) | 10 min |
| Recap (21) | 1 min |
| P3 (22-24) | 6 min |
| Fechamento (25-28) | 4 min + Q&A |
| **Total** | **~45 min** |
