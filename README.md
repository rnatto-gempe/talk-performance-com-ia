# Você acha que está sendo produtivo com IA. Mas está?

> Talk apresentada no **StartSe AI Festival 2026** (13–14 maio, Pro Magno, SP) por **Renato Barbosa** — Head de Engenharia & Sócio na StartSe.

[![Talk](https://img.shields.io/badge/talk-AI%20Festival%202026-00d9ff?style=flat-square)](https://startse.com)
[![Slides](https://img.shields.io/badge/slides-HTML-orange?style=flat-square)](./index.html)
[![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)](./LICENSE)

---

## Sobre

Este repositório contém os **slides, roteiro, speaker notes e fontes** de uma talk de 45 minutos sobre **produtividade real (não vaidade) com IA na engenharia de software**.

A talk responde 3 perguntas operacionais que enfrentamos na StartSe:

1. **Como definimos um processo de trabalho com IA?** → Ralph Loop + skills `/prd` e `/ralph`
2. **Como mensuramos performance de verdade?** → DORA + Dev Fluency = Ralph Console
3. **Como acompanhamos alinhamento estratégico em escala?** → Skill `/tech-manager`

### Por que essa talk existe

Estudos recentes (METR, Faros AI, Ehsani et al., Chroma) mostram que **a percepção de produtividade com IA está descolada da realidade**:

- Devs experientes **superestimam** em até 39pp seu próprio ganho de produtividade com IA (METR, 2025)
- Throughput sobe, mas tempo de review sobe **+441%** e incidentes em produção **+242%** (Faros AI, 2026)
- 98% das falhas de PRs gerados por IA são **socio-técnicas e de processo**, não do código (Ehsani et al., 2026)

A talk apresenta um modelo operacional concreto pra atravessar isso.

---

## Como apresentar os slides

### Opção 1: Abrir direto no navegador
```bash
git clone https://github.com/<seu-user>/talk-performance-com-ia.git
cd talk-performance-com-ia
open index.html   # macOS
# xdg-open index.html  # Linux
# start index.html     # Windows
```

### Opção 2: Servir local
```bash
python3 -m http.server 8000
# abre http://localhost:8000
```

### Opção 3: GitHub Pages
Acesse `https://<seu-user>.github.io/talk-performance-com-ia/` após habilitar Pages nas settings do repo.

---

## Controles do deck

| Tecla | Ação |
|---|---|
| `→` / `Space` / `PageDown` | Próximo slide (ou próximo step interno em slides com reveal progressivo) |
| `←` / `PageUp` | Slide anterior (ou step interno anterior) |
| `N` | Toggle speaker notes |
| `F` | Toggle fullscreen |
| `Home` / `End` | Primeiro / último slide |
| Swipe (touch) | Avançar / voltar |

---

## Estrutura do repositório

```
.
├── index.html                  # Deck completo (HTML/CSS/JS, single-file)
├── docs/
│   ├── roteiro.md              # Roteiro narrativo completo da talk
│   ├── slides-outline.md       # Outline com todos os 28 slides
│   ├── speaker-notes.md        # Speaker notes consolidadas
│   └── fontes.md               # Bibliografia e fontes citadas
├── assets/                     # Imagens, foto de capa, QR codes
└── .github/workflows/
    └── deploy.yml              # Deploy automático pro GitHub Pages
```

---

## Stack do deck

- **HTML único** (~1400 linhas, sem build step) — abre em qualquer navegador moderno
- **Google Fonts**: Barlow Condensed, Barlow, JetBrains Mono
- **Animações CSS** com keyframes (sem framework de slides)
- **JavaScript vanilla** (~70 linhas) pra navegação + reveal progressivo + auto-scroll do chat demo
- **Paleta**: AI Festival 2026 — azul elétrico (`#00d9ff`) sobre fundo escuro (`#05060a`), com acentos amber/red/blue/purple
- **Speaker notes embedded** nos atributos `data-notes` de cada slide

---

## Slides em destaque

| # | Slide | Destaque |
|---|---|---|
| 4 | Diagnóstico METR | Gap percepção × realidade com reveal progressivo (4 steps) |
| 5 | Diagnóstico Faros AI | Acceleration Whiplash, reveal "Sim!" → números positivos → "Mas..." → negativos |
| 8 | Demo do jeito tradicional | **Chat animado de 40s** mostrando 15 mensagens de babysitting até "tá bom" |
| 11 | Context Rot | Curva U SVG + dados Chroma |
| 14 | Ralph Loop na prática | Skills `/prd` `/ralph` + `./ralph.sh --tool claude 15` + aviso `dangerously-skip-permissions` |
| 16 | Painel do vendor | **Gráfico SVG dos meus 2,5B tokens** vs time inteiro |
| 17 | Caso Meta · Claudeonomics | Tokenmaxxing, ~60T tokens, ~US$ 900M, leaderboard derrubado |

---

## Fontes principais

Bibliografia completa em [`docs/fontes.md`](./docs/fontes.md).

- **METR** · Becker, Rush, Barnes, Rein · _Measuring the Impact of Early-2025 AI on Experienced Open-Source Developer Productivity_ · arXiv:2507.09089 · Jul/2025
- **Faros AI** · _AI Engineering Report 2026: The Acceleration Whiplash_ · 22k devs, 4k times
- **Ehsani et al.** · _Where Do AI Coding Agents Fail?_ · arXiv:2601.15195 · Drexel University · Jan/2026
- **Chroma Research** · _Context Rot_ · Jul/2025
- **Liu et al.** · _Lost in the Middle_ · TACL 2024 · arXiv:2307.03172
- **DORA** · Google Cloud · livro _Accelerate_
- **The Information / Pragmatic Engineer** · Reportagens sobre Tokenmaxxing & Claudeonomics · Abr/2026

---

## Conecte-se

- **LinkedIn**: [renato-barbosa](https://www.linkedin.com/in/renatorbarbosa/)
- **StartSe**: [startse.com](https://startse.com)
- **Ralph Console** (waitlist): em breve
- **Bússola Executiva de IA**: em breve

---

## Licença

[MIT](./LICENSE) — sinta-se à vontade pra remixar, adaptar e usar como base pra suas próprias talks. Se reaproveitar, uma menção é bem-vinda mas não obrigatória.

---

<sub>Construído com Claude Code, usando o próprio Ralph Loop. Meta o suficiente?</sub>
