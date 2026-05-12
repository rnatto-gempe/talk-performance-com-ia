# Roteiro — Talk "Performance com IA"

> **Autor:** Renato Barbosa (Partner & Tech Manager, StartSe)
> **Duração-alvo:** 40-50 minutos
> **Formato:** Mescla das talks anteriores Ralph Loop + Ralph Console + novo conteúdo sobre processo
> **Audiência:** Profissionais de tecnologia e líderes interessados em produtividade real com IA

---

## SUMÁRIO

1. [Possíveis Títulos](#1-possíveis-títulos-para-a-palestra)
2. [Transcrição Corrigida](#2-transcrição-corrigida)
3. [Mapa do Conteúdo Original (25 min) → Roteiro Expandido (45 min)](#3-mapa-do-conteúdo-original-→-roteiro-expandido)
4. [Roteiro Detalhado com Fontes](#4-roteiro-detalhado)
5. [Argumentos & Conteúdos para Estender a Apresentação](#5-argumentos-e-conteúdos-resgatados-para-estender)
6. [Bibliografia Completa](#6-bibliografia-completa)

---

## 1. POSSÍVEIS TÍTULOS PARA A PALESTRA

### Categoria A — Provocativos (chamam atenção, geram curiosidade)

1. **"Token não entrega ROI: como medir produtividade real com IA"**
2. **"95% das empresas falham com IA. Como estar nos 5%."**
3. **"Pare de ser babá da sua IA: o jeito certo de programar com agentes"**
4. **"O paradoxo da produtividade: por que mais código com IA não significa mais entrega"**
5. **"Você não está sendo mais produtivo com IA — e nem sabe disso"**

### Categoria B — Técnicos (focam no método)

6. **"Do prompt ao processo: planejamento como diferencial competitivo na era da IA"**
7. **"Ralph Loop + DORA: o caminho da IA artesanal para a IA industrial"**
8. **"Anatomia de um workflow de IA que funciona em produção"**
9. **"Engenharia de software com IA: planejamento, validação e métricas que importam"**

### Categoria C — Diretos (espelham o conteúdo do áudio)

10. **"Como aplicar IA do jeito certo: lições de quem está fazendo"**
11. **"Performance real com IA: do hype às métricas que importam"**
12. **"De vibe coding a desenvolvimento agêntico industrializado"**

### 🏆 RECOMENDAÇÕES DE TOP 3

Para uma audiência mista (técnicos + líderes), as três que melhor capturam o tom original e a tese central:

> **1. "Token não entrega ROI: como medir produtividade real com IA"**
> Alinha-se à frase mais marcante do áudio ("Token não entrega resultado") e cria expectativa imediata de valor.
>
> **2. "Você acha que está sendo mais produtivo com IA. Mas está?"**
> Provoca a audiência logo no título, é honesto sobre a tese (apenas 14% conseguem) e prepara o terreno para o reveal de processo + métricas.
>
> **3. "Do hype ao ROI: o método que separa os 5% de sucesso na IA"**
> Mais executivo, vincula o número de falha (MIT NANDA, RAND) ao método (Ralph Loop + DORA + Ralph Console).

---

## 2. TRANSCRIÇÃO CORRIGIDA

> **Notas de correção aplicadas:**
> - "Starts" → "StartSe"
> - "grupo Al" → "Grupo Alun"
> - "chat EPT" → "ChatGPT"
> - "intelig" / "intelig artificial" → "inteligência artificial"
> - "H loop" / "Half Loop" / "Half" / "Half Console" / "Ralf" → **"Ralph Loop"** / **"Ralph"** / **"Ralph Console"** (referência ao padrão snarktank/ralph e ao seu produto Ralph Console)
> - "barra PRD" / "barra BRD" → "**slash PRD** (`/prd`)" — comando Claude Code
> - "barra" → "slash" (comando)
> - "Jason" → "JSON"
> - "tool list" → "TODO list"
> - "talpiva" / "tal piva" → "perspectiva"
> - "out tab" / "alt tab" → "Alt+Tab"
> - "K" / "KA" → "QA"
> - "stage" → "staging"
> - "CD" → "CI/CD"
> - "Roy" → "ROI"
> - "hora" / "Dora Matrix" → "**DORA Metrics**" (DevOps Research and Assessment)
> - "Germa" → "forma"
> - "Gabriel Stablin" → "Gabriel Esteblein" (presumido — confirmar grafia correta com o time)
> - "C" (final) → "CLI"
> - "se zará" → "guarda" / "memoriza"
> - "ele se baseia em Git" — preservado, contexto Git
> - "skill do cloud" → "skill do Claude (Code)"
> - "vendors" → preservado (termo técnico)

### Transcrição limpa

Olá, pessoal. Muito bom dia. É um prazer estar aqui com vocês. Meu nome é Renato Barbosa, sou atualmente líder de engenharia na StartSe — fazemos parte do Grupo Alun. Tô há mais de 10 anos atuando com tecnologia. Aqui dentro da StartSe eu já ocupei várias cadeiras, já tive vários papéis. Eu tenho um contexto muito de tecnologia, mas sempre precisei me adaptar a conversar com quem não é de tecnologia.

Nos últimos tempos eu andei, como eu comentei, sentei por várias cadeiras aqui. Atuei com performance de aplicações, com aplicações cloud, com inteligência artificial, com desenvolvimento web, frontend, backend, aplicativo. Enfim, passei por vários desafios, tem o contexto de praticamente tudo que tem de tecnologia dentro da StartSe.

Atualmente, meu desafio está muito voltado para inteligência artificial nos últimos tempos, acho que igual o de todo mundo aqui. Nos últimos dois anos, depois que tivemos a virada de chave do ChatGPT, tivemos a necessidade de começar a conversar com nossos clientes sobre inteligência artificial. Então desenvolvemos alguns programas de inteligência artificial — muitos de vocês já fizeram, inclusive. Desses programas, surgiu a necessidade de alguns clientes de aplicar consultoria. Então diversas vezes nós iniciamos programas de consultoria junto aos clientes. E nesse programa de consultoria, o nosso papel era conseguir ajudar os clientes a compreender e aplicar a inteligência artificial.

Tô trazendo esse contexto pra vocês terem uma noção da minha bagagem. Já ajudei a aplicar inteligência artificial em vários cenários, várias empresas, vários modelos de negócio. E o primeiro insight importante a trazer aqui: **não adianta tentar colocar inteligência artificial num processo ruim**. Se você tenta automatizar um processo que não deveria existir, você está aumentando o seu problema, não resolvendo. Essa tem que ser uma premissa: primeiro valida o processo e depois pensa na inteligência artificial. Hoje a gente vê muito uma necessidade de todo mundo colocar IA a qualquer custo em um dos seus produtos, e isso está trazendo muitos problemas no mercado.

Essa talk eu já apresentei numa vertente pro Human-in-the-Loop, que eu achava na época que era o ponto mais importante da inteligência artificial — e ele continua sendo, mas de uma forma diferente hoje em dia.

Então hoje eu vou falar pra vocês de **por que vocês devem aplicar inteligência artificial do jeito certo, e quais os meus conselhos pra que vocês não se tornem menos eficientes com IA, ao invés de se tornarem mais eficientes**.

Tem um dado que eu já apresentei em algumas palestras: qual porcentagem das empresas que conseguem ter sucesso ao aplicar IA num produto e lançar no mercado? Naquele momento, **5% das empresas conseguiam ter sucesso**. E mais do que isso, hoje em dia **apenas 14% dos profissionais conseguem realmente se tornar mais produtivos** ao aplicar inteligência artificial no seu processo.

O objetivo da IA é ser mais produtivo, você colocar ela no seu modelo de trabalho. E você começa a aplicar inteligência artificial e está menos produtivo, e você nem sabe disso, você nem consegue medir isso. Por quê? Porque tudo que os vendors, as empresas de inteligência artificial te dão, é: quantos PRs você conseguiu abrir com IA, quantas linhas de código você escreveu, quantos tokens você gastou. É tudo uma corrida por token. "Nossa, estourei minha janela hoje, consigo liberar daqui a algumas horas." E você vai gerenciando assim, achando que está sendo mais produtivo cada vez que gasta mais token. **Isso não é verdade. Token não entrega resultado. Token não entrega ROI.**

Esse é um grande problema que nós temos aqui dentro da StartSe e começamos a tentar resolver com padrões mais sólidos. A primeira coisa pra se tornar mais produtivo é **investir tempo em definir um processo**.

Tem vários no mercado. Pra quem é de tecnologia, tem processos pra desenvolvimento de software com IA. Tem frameworks que vários players estão inventando por aí. Já vai ter benchmarks comparando modelos, comparando frameworks, e vai te falar qual é o melhor. Mas eu acho que **não existe bala de prata**. Você tem que pegar um e testar. **É melhor ter um processo definido do que não ter nenhum e trabalhar a Deus dará.** Se você coloca um workflow de trabalho, você vai ser mais produtivo do que não colocar.

Nos workshops aqui no evento, vocês vão ver pessoas falando sobre Ralph Loop, provavelmente alguém vai falar sobre GDD, alguém vai falar sobre desenvolvimento orientado a especificação. Não interessa muito o processo. Comece a adotar um. Isso é muito importante porque vai guiar muito o sucesso de como você tem sucesso com IA.

Se você só abre o Claude Code, dá uma instrução, copia e cola um texto, joga um PDF, dá uma instrução, fala "eu quero uma página HTML que faça isso" — seu processo ainda está defasado. É assim que a gente trabalhava com IA em 2024. A gente está em 2026, evoluímos muito.

A primeira coisa que você tem que ter é um **processo de planejamento**. Isso é o que mais traz resultado. Eu tô aplicando inteligência artificial em processos há muito tempo, desde quando saiu o ChatGPT eu tento colocar a IA dentro dos processos pra de fato agregar valor. E o que mais me dá resultado é investir tempo no planejamento.

Vou usar um exemplo com o Ralph Loop, mas não se prenda ao Ralph Loop. Em todo processo, **boa parte do tempo você investe em planejamento e validação, não em execução**. É meio óbvio: a IA consegue executar bem, mas depende. Depende das suas instruções. Depende do seu planejamento de como aquilo tem que ser executado. Depende do planejamento de validação. Como o que eu preciso validar pra que um endpoint que criei novo no checkout vá pra produção? Eu posso usar IA pra criar um endpoint no checkout? Pode. Não é que não pode. Mas como é sua pipeline de QA? O que define que isso pode ir pra produção e o que não pode? Esse é o ponto que vai te dar diferencial no mercado, que vai fazer você usar IA igual gente grande e não replicar prompt.

Então, qual workflow de trabalho eu sugiro? O Ralph Loop é uma boa. Pra quem é técnico é muito fácil se adaptar. Pra quem não é técnico ainda acho que vale a pena. Vai ter alguns conhecimentos importantes, porque ele se baseia em Git. Antigamente, quando a gente precisava criar um novo software, criava o código, colocava na máquina, mandava pro cliente, e o cliente falava "eu preciso modificar tal botão". Eu criava a versão dois pra não perder a primeira. Tinha duas pastas de arquivo, mandava o segundo arquivo pro cliente. É igual versionamento — você emite um, gera o PDF, manda pro cliente, pede validação, gera outro PDF e tem que ficar armazenando vários arquivos. Era a bagunça que a gente tinha dentro da engenharia de software. Pra isso criamos o Git. O Git ajuda no versionamento. É a mesma coisa que entrar no Google Docs e conseguir voltar no histórico e ver as alterações. Eu sei que a maioria aqui deve conhecer Git, mas é importante dar esse conceito porque o Ralph Loop depende dele.

Depois que você define e consegue monitorar seu histórico de alterações, e tem um processo que te ajuda a manter esse histórico, ele vai te ajudar a planejar. O primeiro comando que a gente vai ter aqui é o **`/prd`**. É uma skill do Claude — pode ser usado no Codex, no Gemini, em qualquer lugar. É uma skill. O conceito de skill hoje é multimodelo. Todas as IAs conseguem conversar com esse estilo de skill.

O `/prd`, o que ele faz? Você descreve pra ele o que quer planejar. Ele vai olhar pro seu código, entender o que você está falando, entender o que tem no seu código, e vai começar a te fazer perguntas pra ajudar a definir melhor o que precisa ser feito. A partir dessas perguntas, você define o escopo de trabalho. Ele te faz cinco perguntas nesse cenário. Eu retorno as perguntas, começo a entender melhor quais gaps tem no que estou pedindo, e começo a repensar no que preciso implementar. Descrevo os gaps e ele faz o planejamento — me retorna esse planejamento bonito, grande, com vários tópicos, checklist pra eu validar, open questions pra eu responder, coisas que ele não conseguiu definir e pede pra eu definir.

Nesse momento, **eu não vou mandar ele executar**. Eu vou validar em paralelo. Antes de validar esse cara, abro uma segunda janela e falo: "**analise isso de forma crítica**", e deixo ele trabalhar. Se retornar alguma coisa relevante, aceito. Se não, não preciso. Mas eu vou focar aqui agora, ler e entender. "Essa parte da funcionalidade é isso que eu quero. Essa parte, hum, isso aqui não está bem descrito, tem uma lógica que talvez possa quebrar." E vou modificando. Volto na análise crítica que ele me fez, ele me dá uma vertente do que precisa mudar. Gostei dos tópicos, vou aceitar.

Agora eu vou desenvolver? Não. Agora eu vou pedir pra ele avaliar isso sob outra perspectiva. Tô falando de uma funcionalidade de checkout, por exemplo. Vamos avaliar sob a perspectiva de segurança. Mando: "**`/prd` avalie o PRD pela perspectiva de segurança e me fale quais os gaps de segurança que eu tenho**". Ele me dá os gaps de segurança. Alguns gaps eu não preciso resolver nesse mesmo PRD. Posso criar uma TODO list e definir a prioridade do que é prioritário pra esse cenário. Posso pedir `/prd` pra revisar pela perspectiva de experiência do usuário, de infraestrutura, de escalabilidade. E começo a tentar definir aonde preciso chegar.

Como engenheiro de software, eu tenho conhecimento de qual é o problema de ter overfit e underfit da funcionalidade. Eu preciso fazer exatamente esta garrafa. Não preciso fazer um galão de 5 litros, mas não preciso fazer um copo de 200ml. Preciso fazer esta garrafa. Tenho que ter esse conhecimento. Tenho que saber onde paro, até onde vou. Esse conhecimento a IA não vai substituir. O conhecimento de saber escrever as linhas de código, ela vai. Mas o conhecimento de saber exatamente o que o meu negócio precisa, é eu que sei. É eu que sei pra onde o negócio tem que ir. É eu que sei até onde é seguro escalar. É eu que sei até onde tenho que ter segurança. Se eu não sei esse conhecimento, preciso buscar, porque meu negócio depende disso. A IA vai me falar qualquer bobeira que vier à cabeça dela — no caso, qualquer bobeira que vier aos bits dela.

Planejei, rodei várias validações, gostei do planejamento, gostei dos gaps, aceitei. Vamos executar. Nesse caso, eu vou executar o **Ralph**. Por que o Ralph é legal? Ele trabalha com um modelo de iteração **limpando o contexto**. Ele vai pegar uma janela do Claude, abrir uma nova por baixo — sem ficar me dando ela visualmente — e vai dar uma instrução específica do que precisa ser executado. Ele pega esse planejamento, transforma em um JSON. Não se preocupe com o termo JSON. JSON é só um formato. Esse Markdown aqui, só que num formato melhor pra comunicação. É melhor pra conversar porque o Ralph vai usar esse JSON pra marcar até onde já foi na funcionalidade. É uma TODO list pra ele.

Ele pega esse list e escreve exatamente o que precisa ser feito. Pra construir essa garrafa, eu preciso começar pela base. Ele vai instanciar uma versão do Claude que vai iniciar e construir a base. Terminou de construir a base, fez as validações que pedi, implementou os testes, implementou a camada de segurança, fez a validação de lint, fez minha validação de CI, finaliza e passa pro próximo. Que vai construir o restante do corpo, finaliza e passa pro próximo. Que vai construir a parte de cima, finaliza e passa pro próximo. Que vai construir a tampa, finaliza e passa pro próximo. Que vai pintar a garrafa, finaliza e passa pro próximo. Que vai testar a funcionalidade da garrafa, finaliza e passa pro próximo. Que vai testar a resistência da garrafa. E assim vai até ele construir tudo que pedi.

**Isso dá um poder absurdo.**

Por quê? Se eu tentar fazer essa mesma coisa com o Claude numa janela aberta, mandando um prompt atrás do outro, pode funcionar — se você abrir a janela, pegar essas instruções, começar a conversar e mandar uma coisa atrás da outra, pode funcionar. Mas eu tenho **dois grandes problemas** que impactam em performance e que às vezes as pessoas não notam, e que são os dois pontos principais que te deixam mais lento usando IA, não mais rápido.

**Primeiro: babysitting.** Você virou uma babá da IA. Dá um comando, espera ela responder, fica assistindo a janelinha, assistindo monte de letrinha mudar. Aí ela responde, você manda outra mensagem, ela responde outra mensagem. Você é a babá. Esse tempo que ela está fazendo aqui, **você está agregando zero**. Ela que está trabalhando, mas você não está, você está esperando. "Ah, o que tô fazendo? Tô esperando a IA trabalhar." Isso não é performance. Você não está performando mais o tempo. Talvez ela vá executar mais rápido, mas aí você cai no segundo problema.

**Segundo: Context Rot.** No começo ela começa a acertar, mas a gente cai num problema com os LLMs em qualquer cenário, onde o conhecimento da janela de contexto que ele vai adotando, faz um formato de **U**. Ele consegue guardar bastante o conhecimento do que você mandou no começo, bastante o que está no final, mas o conhecimento do meio vai se perdendo. Conforme vou implementando algo complexo, vou tentando gerir essa janela de contexto, e crio um problema maior. Ele começa a errar mais, esquecer do conhecimento do meio, que às vezes é a parte importante que ele precisava pra aquela funcionalidade. E como o escopo não está tão bem definido, porque eu não tive um bom planejamento, eu crio um grande problema. Fico brigando com a IA pra ela fazer o que preciso.

No outro cenário — o do Ralph — eu gastei o tempo planejando, tenho segurança do que precisa ser implementado, enxerguei outros gaps, comecei a implementar, coloquei pra ligar e dou Alt+Tab. Se eu for mexer no Instagram agora, depois que dei Alt+Tab, caí no mesmo problema de antes. Mas agora a IA está desenvolvendo. Eu posso abrir um novo agente, pegar um novo problema, pegar uma issue pra resolver, pegar outro cenário. **A IA está trabalhando pra mim em background.** Isso é o Ralph Loop. Ele te dá esse potencial de iniciar a IA com instruções bem definidas e só validar o resultado final.

Depois disso, ele vai ter commitado todas as alterações no Git. Eu posso abrir o PR. O PR vai dar a funcionalidade que eu quero. Eu executo o código, faço o que preciso, subo o PR. No PR, faço o code review. Posso ser mais performático também? Pode. Mas **não dependa de uma IA exatamente pra fazer a validação do código**. Você pode pedir pra uma IA validar e aceitar alguns feedbacks, mas também faça review. Isso vai te dar qualidade.

Outro ponto: **tenha um bom processo de CI/CD** no seu código pra validar, fazer testes antes de subir em produção. Depois que você fez tudo isso, testou em QA, sobe em staging e tem que ter alguém que olha em staging e valida se aquilo é exatamente o que precisa ser feito. Depois de toda essa camada de validação — boa parte é processo de software, mas precisa continuar existindo —, você muda pra produção e está um pouco mais seguro pra implementar, porque o ser humano ainda erra. A IA também. Você com a IA também vai errar. Aqui vocês vão ser perfeitos? Não. Mas agora você tem um processo mais maduro que pode melhorar, porque sabe exatamente quais passos seguiu pra implementar a funcionalidade, e consegue ter maior qualidade na entrega final.

**Isso é o Ralph Loop.**

Beleza. Agora, **como eu meço de verdade na minha equipe se eles estão performando bem?**

Primeiro passo: definir um processo. Meu time está usando. Aqui na StartSe temos atualmente um time de tecnologia só da StartSe pra cuidar da nossa plataforma e dos nossos produtos. Time de 15 pessoas. Nesse time estabelecemos o processo. Todo mundo está usando Ralph Loop. Toda funcionalidade que precisamos desenvolver, seguimos esse processo. A maioria deles encaixa usando o processo.

Comecei a desenvolver, comecei a ter resultado. Como valido se tenho performance usando IA? Se eu tentar olhar o painel do Claude, é isso que ele me dá de informação: quantos PRs eu abri, quantas linhas de código escrevi, quantos tokens gastei. Isso é performance? Não.

O que pra mim é importante é a **forma legal de medir performance de equipe que se chama DORA Metrics**. São métricas DORA. DORA é uma sigla, mas no fundo é conseguir medir: quanto tempo passei desenvolvendo, quanto tempo passei revisando, quanto tempo passei validando em staging, quando isso foi pra produção. Começo a medir todo o ciclo de vida de fato — quanto tempo cada um leva pra entregar uma funcionalidade pra produção, quanto tempo demoro pra entregar uma funcionalidade complexa, quantas funcionalidades estou entregando, o quanto essas funcionalidades agregam. Sabendo do ROI daquela funcionalidade, eu tenho o tempo que demorei pra entregar o ROI. Consigo calcular isso.

Pra isso, criamos o **Ralph Console**. Ele não está medindo ROI ainda, mas já consegue medir todo o ciclo de vida. Inclusive — se quiserem testar — estamos abrindo uma waitlist. Ele não está aberto pra ser utilizado ainda, ainda estamos implementando, mas já temos a list. É só escanear o QR code aí, se quiserem.

O que é o Ralph Console? Depois que eu uso o Ralph por um processo específico, nós temos um CLI que o Gabriel Esteblein, do nosso time, criou — vai ter uma talk sobre isso. Recomendo muito que vocês vejam, ele fez um processo muito legal pra criar esse CLI utilizando Ralph, inclusive. A partir do momento que eu uso o Ralph, **consigo coletar métricas**: quanto tempo demorei pra planejar, quanto tempo a IA demorou pra executar, quanto tempo demorei pra testar, quanto tempo demorou pra ser validado em QA, quanto tempo isso ficou em produção, quantos bugs gerou em produção.

**Tá vendo? Eu consigo medir o ciclo de vida inteiro da minha funcionalidade.** Versus poderia olhar no painel do Claude e falar: "Renato entregou 5000 linhas de código." É performático? Não sei. "Renato gastou 1 bilhão de token." É performático? Não sei. Eu em dois meses gastei 1.200.000 tokens no Claude. Consigo medir token, consigo medir linhas de código entregues, consigo medir PRs abertos. Mas eu **consigo medir quanto tempo a IA ficou desenvolvendo o que mandei, quanto tempo demorei planejando, quanto tempo demorou em QA, quanto tempo meu time demora pra validar, quanto tempo isso fica em produção até algum bug acontecer**. Tenho todo o ciclo de vida. Isso me dá muita métrica, muito controle.

Isso é o que eu queria trazer pra vocês. Obrigado.

---

## 3. MAPA DO CONTEÚDO ORIGINAL → ROTEIRO EXPANDIDO

| # | Bloco | Original (~25 min) | Expandido (~45 min) |
|---|---|---|---|
| 0 | Abertura & autoridade | 2 min | 3 min |
| 1 | Premissa: processo ruim + IA = problema maior | 1 min | 4 min |
| 2 | Os números do fracasso (5%, 14%) | 1 min | 5 min |
| 3 | A armadilha das métricas de vendor (token, linhas, PRs) | 2 min | 4 min |
| 4 | Por que processo > prompt | 2 min | 4 min |
| 5 | Planejamento como diferencial (slash PRD, validação multi-perspectiva) | 4 min | 7 min |
| 6 | Ralph Loop em ação | 4 min | 6 min |
| 7 | Os dois inimigos: Babysitting + Context Rot | 3 min | 5 min |
| 8 | Code review, CI/CD, staging, produção | 2 min | 3 min |
| 9 | Como medir? DORA Metrics | 2 min | 4 min |
| 10 | Ralph Console | 1 min | 3 min |
| 11 | Encerramento + CTA | 1 min | 2 min |

> **Total estimado:** **~50 min com Q&A** ou **45 min sem**

---

## 4. ROTEIRO DETALHADO

### 🎬 BLOCO 0 — Abertura & Autoridade *(3 min)*

**Objetivo:** Estabelecer credibilidade técnica, sinalizar que é uma fala de operador (não de academic).

**Falar:**
- Nome, papel atual (Partner & Tech Manager StartSe / Grupo Alun).
- 10+ anos na StartSe, várias cadeiras: cloud, performance, frontend, backend, IA, consultoria.
- "Tô trazendo esse contexto pra vocês terem noção da minha bagagem — já ajudei a aplicar IA em vários cenários, várias empresas, vários modelos de negócio."
- **Gancho de transição:** "E sabe qual foi o primeiro insight que eu tirei desses anos todos? Esse aqui."

**Visual sugerido:** Foto + linha do tempo simples mostrando a progressão dentro da StartSe, terminando em "Tech Manager — 15 pessoas, 5 squads".

---

### 🧱 BLOCO 1 — Premissa: IA num processo ruim amplifica o problema *(4 min)*

**Tese central:** "Não adianta tentar colocar IA num processo ruim. Se você automatiza um processo que não deveria existir, você está aumentando seu problema, não resolvendo."

**Conteúdo expandido:**

- Trazer o conceito de **automation paradox**: automação amplifica padrões — bons e ruins.
- **Exemplo prático:** "Imagine um processo de QA manual que está mal definido. A pessoa testa o que lembra, depende de quem está disponível. Se você automatiza isso com IA, você não consertou o processo — você só fez o caos rodar mais rápido."
- Citar o pattern do EPAM: *"When such a 'code-first, figure out later' approach runs ahead of architecture, security, and governance, the system eventually crumbles under its own weight"* — fonte: [EPAM Insights, Spec-Driven Development, jan/2026](https://www.epam.com/insights/ai/blogs/inside-spec-driven-development-what-githubspec-kit-makes-possible-for-ai-engineering).
- **Ligar à própria experiência:** "Diversas vezes nós iniciamos programas de consultoria com clientes — e o primeiro que eu falo é 'antes da IA, vamos olhar seu processo'. Sempre."

**Gancho de transição:** "E pra entender por que isso importa tanto, deixa eu te mostrar números que vão te fazer repensar tudo."

---

### 📉 BLOCO 2 — Os Números do Fracasso *(5 min)*

**Tese:** "5% das empresas têm sucesso com IA. 14% dos profissionais ficam mais produtivos. **A maioria fica pior.**"

**Dados a apresentar (com fontes):**

#### 1. **5% de sucesso em produtos com IA** — MIT NANDA
- *"Despite the rush to integrate powerful new models, about 5% of AI pilot programs achieve rapid revenue acceleration; the vast majority stall, delivering little to no measurable impact on P&L"* — [MIT Project NANDA, "The GenAI Divide", jul/2025](https://mlq.ai/media/quarterly_decks/v0.1_State_of_AI_in_Business_2025_Report.pdf), reportado por [Fortune, ago/2025](https://fortune.com/2025/08/18/mit-report-95-percent-generative-ai-pilots-at-companies-failing-cfo/).
- 150 entrevistas com líderes, 350 funcionários, 300 deployments públicos analisados.

#### 2. **80% de falha geral em projetos de IA** — RAND Corporation
- *"80.3% of AI projects fail to deliver their intended business value. Of those, 33.8% are abandoned before ever reaching production, 28.4% reach completion but fail to deliver expected business value, and 18.1% deliver some value but cannot justify the cost"* — [RAND Corporation, 2025, sintetizado em Pertama Partners, fev/2026](https://www.pertamapartners.com/insights/ai-project-failure-statistics-2026).
- Comparar: **2x mais que projetos de TI tradicionais**.

#### 3. **42% das empresas abandonaram iniciativas em 2025** (subiu de 17% em 2024)
- [S&P Global Market Intelligence, 2025](https://beam.ai/agentic-insights/why-42-percent-of-ai-projects-show-zero-roi-and-how-to-be-in-the-58-percent).

#### 4. **Devs com IA são 19% MAIS LENTOS** (estudo controlado) — METR
- *"Surprisingly, we find that allowing AI actually increases completion time by 19%—AI tooling slowed developers down"* — [METR, "Measuring the Impact of Early-2025 AI", arXiv:2507.09089](https://arxiv.org/abs/2507.09089), 16 devs experientes, 246 tasks reais em projetos com avg 22k stars no GitHub.
- **O ponto crítico:** os próprios devs **acharam** que estavam **20% mais rápidos**. A percepção é o oposto da realidade.

#### 5. **CircleCI: 2026 State of Software Delivery — 28 milhões de workflows analisados**
- *"Average workflow throughput across all teams grew 59% year over year — the largest single-year increase ever recorded"* — [CircleCI 2026 Report, fev/2026](https://circleci.com/blog/five-takeaways-2026-software-delivery-report/).
- *"Main branch success rates dropped to 70.8%, the lowest in over five years and well below CircleCI's recommended benchmark of 90%. That means nearly 3 out of every 10 attempts to merge into production are failing"*.
- **A leitura honesta:** mais código entrando, menos código chegando em produção. *"More code, less software"* — [DevOpsDigest, mar/2026](https://www.devopsdigest.com/more-code-less-software-what-28-million-workflows-revealed-about-the-state-of-software-delivery-in).

**Slide-chave:** Big number. **"5%"** sozinho na tela. Pausa. Depois: **"14%"**. Pausa. Depois: **"19% mais lentos."** Deixar o número fazer o trabalho.

**Gancho de transição:** "Por que isso acontece? Porque a maioria de vocês está medindo a coisa errada."

---

### 🎯 BLOCO 3 — A Armadilha das Métricas de Vendor *(4 min)*

**Tese:** "Token não entrega ROI. Linhas de código não entregam ROI. PR aberto não entrega ROI."

**O problema dos painéis dos vendors:**
- O painel do Claude/Cursor/Copilot mostra: **tokens gastos, linhas geradas, PRs abertos**.
- Esses números são **vanity metrics** — bonitos pra reportar, mas não dizem se você está mais produtivo.
- **Goodhart's Law:** "Quando uma medida se torna alvo, ela deixa de ser uma boa medida."
- **Faros AI sobre o estudo METR:** *"Developers are completing a lot more tasks with AI, but organizations aren't delivering any faster"* — [Faros AI, jul/2025](https://www.faros.ai/blog/lab-vs-reality-ai-productivity-study-findings).
- **DORA 2025 Report:** *"AI adoption improves throughput by an estimated 2-18% yet often leads to declining stability with significantly higher change failure rates"* — [Google DORA 2025, sintetizado em Exceeds.ai](https://blog.exceeds.ai/dora-metrics-engineering-effectiveness/).

**Aprofundamento — o "Acceleration Whiplash" do CircleCI:**
*"Real throughput gains at the top, compounding quality costs at every stage below"* — citação literal do [CircleCI Report 2026](https://circleci.com/blog/five-takeaways-2026-software-delivery-report/).

| Indicador | Tendência YoY 2025→2026 |
|---|---|
| Daily workflow throughput | **+59%** ⬆️ |
| Median time in PR review | **+441%** ⬆️ |
| Pull request size | **+51.3%** ⬆️ |
| Bugs por dev | **+54%** ⬆️ |
| Incidents per PR | **+242.7%** ⬆️ |
| Main branch success rate | **70.8%** (mínima de 5 anos) ⬇️ |

**Frase de impacto:** *"Você está abrindo mais PR. Mas eles estão demorando mais pra revisar, ficando maiores, e quebrando mais a produção. Isso é performance?"*

**Gancho de transição:** "Se token não é a métrica, e PR não é a métrica, **o que é?** Antes de chegar nela, vamos primeiro à parte que ninguém quer fazer mas que separa os 5% que dão certo: o processo."

---

### 🧭 BLOCO 4 — Por que Processo > Prompt *(4 min)*

**Tese:** "Não existe bala de prata. **É melhor ter um processo definido do que não ter nenhum e trabalhar a Deus dará.**"

**Conteúdo:**

- Mercado tem vários frameworks: Ralph Loop, BMAD-METHOD, GitHub Spec Kit, Kiro (AWS), Tessl, cc-sdd.
- **Pesquisar fontes:**
  - [GitHub Blog — "Spec-driven development with AI"](https://github.blog/ai-and-ml/generative-ai/spec-driven-development-with-ai-get-started-with-a-new-open-source-toolkit/) (set/2025).
  - *"We treat coding agents like search engines when we should be treating them more like literal-minded pair programmers. They excel at pattern recognition but still need unambiguous instructions"* — Den Delimarsky, Principal PM no GitHub.
  - [Martin Fowler / ThoughtWorks — comparativo Kiro vs Spec Kit vs Tessl](https://martinfowler.com/articles/exploring-gen-ai/sdd-3-tools.html).
  - [BrainGrid — "The Babysitting is Over"](https://www.braingrid.ai/blog/the-babysitting-is-over-a-new-plan-for-ai-coding) (jul/2025).

**Argumentos para defender:**
1. **Processo dá repetibilidade.** Sem processo, todo dev usa IA do jeito dele — você não consegue medir, comparar, melhorar.
2. **Processo dá memória organizacional.** O que funcionou na sprint passada vira skill/template/PRD reutilizável.
3. **Processo dá guardrails.** O CI/CD, o code review obrigatório, o staging — eles existem por uma razão. A IA não te dispensa deles. **Te obriga mais ainda a tê-los.**

**Citação âncora:**
*"AI is now seen as an amplifier of performance, accelerating and optimising processes on a large scale. […] AI doesn't create a performance gap; it reveals it."* — [CircleCI 2026 State of Software Delivery](https://www.prnewswire.com/news-releases/circleci-publishes-2026-state-of-software-delivery-302691131.html).

**Provocação para a audiência:**
"Levanta a mão quem tem documentado **como** seu time usa IA hoje. Não é a ferramenta — é o processo. Quem tem `CLAUDE.md` versionado? Quem tem comandos `/prd` compartilhados no time? Quem revisa código gerado por IA com a mesma rigidez que código humano?"

**Gancho:** "Se a maioria das mãos está abaixada — e eu aposto que está — o que vou mostrar agora vale mais do que qualquer comparativo de modelo."

---

### 📋 BLOCO 5 — Planejamento como Diferencial *(7 min)*

**Tese:** "Boa parte do tempo do processo você investe em planejamento e validação, **não em execução**."

#### 5.1 Por que a IA executa bem — desde que bem instruída

- **Frase:** "A IA executa bem. Depende. Depende das suas instruções."
- Citar Anthropic sobre design de prompt: especificidade > eloquência.
- O conceito de **"literal-minded pair programmer"** do GitHub Spec Kit.

#### 5.2 O fluxo de planejamento que eu uso (`/prd` + revisão multi-perspectiva)

**Passo a passo (ao vivo se possível, ou screencast):**

1. **`/prd <descrição da feature>`** — Skill do Claude Code analisa o código atual e faz 5 perguntas pra fechar gaps de requisito.
2. **Você responde as perguntas** — aqui já reveste seu próprio entendimento. Muitas vezes você descobre que nem sabia direito o que queria.
3. **`/prd` gera o documento** — checklist, open questions, escopo, casos de borda.
4. **Em paralelo, abre uma 2ª janela:** "Analise esse PRD de forma crítica. Encontre lacunas, problemas, conflitos."
5. **Aceita ou rejeita os pontos da análise crítica.**
6. **Re-revisão por perspectiva específica:**
   - `/prd revise pela perspectiva de segurança`
   - `/prd revise pela perspectiva de UX`
   - `/prd revise pela perspectiva de escalabilidade`
   - `/prd revise pela perspectiva de infraestrutura`
7. **Decide o que entra no escopo agora vs. backlog (TODO list).**

**Por que isso funciona:**
- **Reduz ambiguidade** (raiz #1 das falhas em IA).
- **Cria um artefato versionado** — vira spec executável.
- **Distribui o risco** — múltiplas "lentes" pegam coisas que uma só não pega.

#### 5.3 O conhecimento que a IA NÃO substitui

**Frase âncora:** *"Eu preciso fazer exatamente esta garrafa. Não preciso fazer um galão de 5 litros, mas não preciso fazer um copo de 200ml. Preciso fazer esta garrafa."*

- Conhecimento de **escopo do negócio** → você que sabe.
- Conhecimento de **até onde escalar com segurança** → você que sabe.
- Conhecimento de **trade-offs de produto** → você que sabe.
- *"Se eu não sei esse conhecimento, preciso buscar, porque meu negócio depende disso. A IA vai me falar qualquer bobeira que vier aos bits dela."*

**Visual sugerido:** A imagem de uma garrafa, ladeada por um galão de 5L (overengineering) e um copo de 200ml (underengineering). Texto: **"Você é o único que sabe qual das três é a certa."**

**Gancho:** "Planejou. Validou. Validou de novo, sob outras perspectivas. Aceitou os gaps. Agora — agora — sim. Vamos executar. Mas não na janela aberta do Claude. Vamos executar **com loop**."

---

### ⚙️ BLOCO 6 — Ralph Loop em Ação *(6 min)*

> **Atenção:** Este bloco é um **recap** da talk anterior do Ralph Loop. Sinalizar pra audiência: "Quem viu minha talk anterior, isso vai ser uma passagem rápida — pra nivelar quem não viu. Quem viu, posso pular?" (Geralmente eles querem ver de novo, mas vale perguntar.)

#### 6.1 O que é o Ralph Loop

- Pattern criado por Geoffrey Huntley (referência: [ghuntley.com/ralph](https://ghuntley.com/ralph/)).
- Implementação prática: **[snarktank/ralph](https://github.com/snarktank/ralph)** — bash script que roda Claude Code (ou Amp) em **instâncias frescas**, uma por user story.
- O nome vem do Ralph Wiggum (Os Simpsons) — **persistência ingênua**: itera até funcionar.

#### 6.2 Como funciona (visual de fluxo)

```
1. Lê prd.json → acha próxima story onde passes:false
2. Spawna NOVA instância Claude Code (contexto limpo!)
3. Claude implementa a story
4. Roda quality checks (typecheck, testes, lint)
5. Se passou: commita, marca passes:true, escreve aprendizado em progress.txt
6. Repete até todas stories passarem
7. Emite <promise>COMPLETE</promise> e encerra
```

**Diferença fundamental do uso manual:**

| | Sem Ralph (sessão longa) | Com Ralph (instância por story) |
|---|---|---|
| Contexto | Acumula → context rot | Fresco a cada iteração |
| Performance | Degrada ao longo do tempo | Consistente |
| Memória | Janela de contexto (frágil) | Git + prd.json + progress.txt (durável) |
| Tamanho da task | Ilimitado (e arriscado) | 1 story cabe na janela |
| Você | Babá (alt+tab no Instagram não vale) | Liberado pra outro problema |

#### 6.3 Por que "small tasks" importa

- *"Cada story do prd.json precisa caber em uma janela de contexto"*.
- Se a task é grande demais → LLM gasta o contexto antes de terminar → produz código ruim.
- **Analogia:** "É como vocês devs — ninguém olha o codebase inteiro de uma vez. Você pega a fatia relevante e trabalha nela. O Ralph faz a mesma coisa."

#### 6.4 Demo curta (live ou screencast)

Mostrar:
1. Estrutura mínima: `scripts/ralph/`, `prd.json`, `CLAUDE.md`, `progress.txt`.
2. Comando de execução: `./scripts/ralph/ralph.sh --tool claude 10`
3. Logs em tempo real: ver o Claude trabalhar, commitar, marcar passes:true.
4. **Trocar pra outra atividade enquanto o loop roda** — esse é o ponto.

**Gancho:** "Massa, né? Mas se você está me ouvindo e pensando 'o que faz isso ser tão diferente de só conversar com Claude por mais tempo' — agora vamos ao **porquê técnico** disso funcionar."

---

### 🧠 BLOCO 7 — Os Dois Inimigos: Babysitting + Context Rot *(5 min)*

#### 7.1 Babysitting: o tempo morto da IA

- *"Você dá um comando, espera ela responder, fica assistindo a janelinha. Esse tempo, você está agregando zero."*
- Estudo de Gloria Mark (UC Irvine): após uma interrupção/troca de contexto, leva-se **>20 minutos** pra retornar ao estado de foco anterior. Fonte: [Super Productivity blog](https://super-productivity.com/blog/what-to-do-while-waiting-for-claude-code/).
- BrainGrid chama isso de **"babysitting tax"**: *"the cognitive overhead of constantly reviewing, reverting, and re-explaining"* — [BrainGrid, jul/2025](https://www.braingrid.ai/blog/the-babysitting-is-over-a-new-plan-for-ai-coding).
- Cerbos: *"AI coding assistants feel productive because they give instant feedback. […] More context is not always better."* — [Cerbos, set/2025](https://www.cerbos.dev/blog/productivity-paradox-of-ai-coding-assistants).

**O dado mais brutal pra inserir aqui:**
- METR descobriu que devs **se sentiam 20% mais rápidos** com IA, **mas eram 19% mais lentos**. A diferença é **39 pontos percentuais** entre percepção e realidade.

#### 7.2 Context Rot: por que conversas longas viram lixo

- **Fonte primária:** [Chroma Research, "Context Rot: How Increasing Input Tokens Impacts LLM Performance", jul/2025](https://research.trychroma.com/context-rot).
- Avaliaram **18 modelos SOTA** (GPT-4.1, Claude 4, Gemini 2.5, Qwen3).
- Resultado: queda de **20-50% de acurácia** ao passar de 10k pra 100k+ tokens — mesmo em tarefas simples.

#### 7.3 Lost in the Middle: o formato em U

- Pesquisa de Liu et al. (2023, TACL 2024): *"Performance is often highest when relevant information occurs at the beginning or end of the input context, and significantly degrades when models must access relevant information in the middle of long contexts"* — [arXiv:2307.03172](https://arxiv.org/abs/2307.03172).
- *"Liu et al. (2024) measured a 30%+ accuracy drop on multi-document question answering when the answer document moved from position 1 to position 10 in a 20-document context"* — [Morph](https://www.morphllm.com/lost-in-the-middle-llm).
- **NoLiMa benchmark:** em 32k tokens, 11 de 12 modelos caem abaixo de 50% da performance original.
- *"Found in the Middle" (Hsieh et al., 2024)*: a curva em U existe na própria atenção do modelo, **independente do conteúdo**.

#### 7.4 Por que o Ralph Loop resolve isso

> **Visual chave:** ilustração do "U" do Context Rot. À esquerda, a janela de contexto que vai degradando com o tempo. À direita, o Ralph Loop com várias mini-janelas frescas, cada uma curta o suficiente pra ficar na zona de alta performance.

- **Cada iteração reseta o contexto** → modelo nunca entra na "dumb zone".
- **Memória persiste no filesystem** (Git + prd.json + progress.txt) — não na janela.
- **O ser humano também escala melhor** — sem babysitting, dá pra ter 3-5 agentes em paralelo, em git worktrees.

**Citação âncora pra fechar o bloco:**
*"AI tools at the February-June 2025 frontier slow developers down by 19% — but the developers themselves estimate a 20% speedup. The gap between perceived and actual productivity is the warning sign."* — METR ([arXiv:2507.09089](https://arxiv.org/abs/2507.09089)).

**Gancho:** "Ok. Você planejou. Você executou com Ralph. **A IA terminou.** Agora vem a parte que muita gente esquece — e que faz toda a diferença entre ir pra produção ou criar um problema enorme."

---

### ✅ BLOCO 8 — Code Review, CI/CD, Staging, Produção *(3 min)*

**Tese:** "Tudo que era processo de software antes da IA continua valendo — **com mais força ainda**."

- **Code review é seu.** Pode pedir IA pra fazer um pre-review e aceitar feedbacks. Mas o review humano não é negociável. Tem que continuar.
- **CI/CD tem que estar maduro.** Sem isso, o ganho de velocidade da IA vira buraco na produção (CircleCI 2026 mostrou isso: 30% de PRs falhando em main).
- **Staging não é decoração.** Tem que ter alguém olhando o staging e validando que aquilo é o que precisa ser feito de verdade.
- **Produção depois de tudo isso** — e ainda assim você vai errar. Mas vai errar **menos**, e vai conseguir **rastrear** onde errou.

**O ponto fundamental:**
- *"Aqui vocês vão ser perfeitos? Não. Mas agora você tem um processo mais maduro que pode melhorar, porque sabe exatamente quais passos seguiu pra implementar a funcionalidade, e consegue ter maior qualidade na entrega final."*

**Slide-chave (decisor):** Pipeline visual com as 5 fases — **Plan → Execute → Review → CI/CD → Staging → Prod** — destacando que IA atua principalmente na fase Execute, e tudo o resto continua sendo gente + processo + ferramenta tradicional.

**Gancho:** "Beleza. Você fez tudo certo. Sua equipe fez tudo certo. Agora — **como você prova isso?** Como você mostra pra liderança, pro cliente, pra você mesmo, que está sendo mais produtivo de verdade?"

---

### 📊 BLOCO 9 — Como Medir? DORA Metrics *(4 min)*

**Tese:** "DORA Metrics medem outcomes do ciclo de entrega. Token mede atividade. Você precisa do primeiro."

#### 9.1 As 4 (agora 5) métricas DORA

Origem: **DORA** (DevOps Research and Assessment), Google Cloud, livro *Accelerate* (Forsgren, Humble, Kim).

| Métrica | O que mede | Elite |
|---|---|---|
| **Deployment Frequency** | Quantas vezes você deploya | On-demand (multiple/day) |
| **Lead Time for Changes** | Tempo de commit até prod | < 1 hora |
| **Change Failure Rate** | % de deploys que falham | 0-2% |
| **Failed Deployment Recovery Time (ex-MTTR)** | Tempo pra restaurar serviço | < 1 hora |
| **Rework Rate** *(nova em 2025)* | % de mudanças não planejadas em prod | Próximo de 0 |

Fontes:
- [DORA Report 2025 — State of AI-assisted Software Development](https://www.future-processing.com/blog/dora-devops-metrics/)
- [Plandek — DORA Metrics in the Age of AI](https://plandek.com/blog/dora-metrics-in-the-age-of-ai-how-engineering-leaders-should-measure-delivery-in-2025)

#### 9.2 Por que DORA é melhor que vanity metrics

- **Tokens** medem **atividade da IA**.
- **Linhas/PRs** medem **atividade do dev**.
- **DORA** mede **outcome do sistema todo** — chega ou não chega na mão do usuário?
- Os números do DORA 2025 mostram o paradoxo: **90% dos devs usam IA**, mas estabilidade está caindo. *"AI adoption improves throughput by 2-18% yet often leads to declining stability."*

#### 9.3 Onde DORA não basta — métricas de Effectiveness com IA

- DORA não distingue **código gerado por IA** vs **código humano**.
- Por isso o Ralph Console adiciona dimensões específicas (próximo bloco).

#### 9.4 Conexão com Ralph Loop

> Quando você usa Ralph Loop com `prd.json` versionado, **você já está coletando os eventos** que alimentam DORA:
> - `prd_started_at` → `pr_created` → Lead Time
> - Sessão concluída → Deployment trigger → Deployment Frequency
> - Quantas iterações até passar quality checks → proxy de Change Failure Rate

**Slide-chave:** Tabela comparando "O que o painel do Claude te dá" vs "O que DORA + Ralph Console te dá". Fica visualmente óbvio o quão diferente são as conversas que você consegue ter com cada conjunto.

**Gancho:** "Massa. Falei muito de teoria, falei muito de processo, falei de DORA. Mas e como sair daqui hoje e começar a medir isso? Foi pra resolver isso que a gente criou o Ralph Console."

---

### 🛠️ BLOCO 10 — Ralph Console *(3 min)*

> **Atenção:** Recap da talk anterior. **Aqui é onde a mescla das duas talks faz mais sentido.**

#### 10.1 O que é

- Painel + CLI (criado pelo Gabriel Esteblein — *confirmar grafia*) que coleta telemetria do Ralph Loop.
- Mede o **ciclo de vida completo** de cada PRD/funcionalidade.

#### 10.2 O que ele já mede (versão atual)

**Eventos coletados via SSE/OpenTelemetry → SigNoz:**
- Tempo de planejamento (de `/prd` ao primeiro commit)
- Tempo de execução IA (loop start → COMPLETE)
- Iteração-a-iteração: duration, exit code, stories concluídas, git hash, tokens, linhas
- Status de PRD: `in_progress` → `pr_open` → `merged` → `master_merged`
- Tempo em QA / staging
- Bugs subsequentes ligados ao commit/PR

#### 10.3 DevFluency Score

Inspirado em DORA, com 4 dimensões ponderadas:

| Dimensão | Peso | O que mede |
|---|---|---|
| AI Effectiveness | 30% | first-try success, completion rate, avg iterations |
| Process Consistency | 20% | uso de PRD, planning time, skills usadas |
| Delivery Speed | 25% | Lead Time, Deployment Frequency |
| Quality & Reliability | 25% | Change Failure Rate, Rework Rate, MTTR |

**5 níveis (CMMI-inspired):** Inicial → Repetível → Definido → Gerenciado → Otimizado.

#### 10.4 Stack

- CLI com OAuth GitHub (1-click setup com GitHub App)
- Multi-tool (Claude Code, Amp, OpenCode)
- Multi-tenant por org GitHub
- Observabilidade: OpenTelemetry + SigNoz (ClickHouse SQL)
- Pipeline CI/CD: vulnerabilidades, testes, lint
- Insights Engine (em desenvolvimento) com 16 padrões compound-trigger inspirados em CircleCI/Thoughtworks/Anthropic/DORA/BMAD

#### 10.5 Roadmap visível

- **Em construção:** fase de planejamento no pipeline, métricas de tokens/linhas, dimensionamento de esforço técnico por story.
- **Gaps assumidos:** depende do Ralph Loop hoje (evolução pra SDD/Spec-Driven Development), sugestão de quick wins, sugestão de skills personalizadas, otimização do score.

**CTA:**
> 🔗 **Waitlist:** ralph.ai-solutions.startse.com
> Mostrar QR code grande na tela. Deixar o slide visível por 30 segundos enquanto fala.

**Gancho de fechamento:** "Quem quiser entrar pra waitlist, escaneia agora. Vamos pro fechamento."

---

### 🎤 BLOCO 11 — Encerramento + CTA *(2 min)*

**Recapitulação em 4 frases:**

1. **Processo > Prompt.** Não existe bala de prata, mas qualquer processo é melhor do que nenhum.
2. **Planejamento > Execução.** A IA executa bem **se** bem instruída. Invista 50%+ do tempo planejando.
3. **Background > Babysitting.** Se você está olhando a IA trabalhar, está agregando zero. Use Ralph (ou similar) e ganhe paralelismo.
4. **Outcomes > Vanity.** Token, linhas, PRs não dizem nada. DORA + ciclo de vida completo dizem tudo.

**Frase de encerramento (volta ao tema da abertura):**

> "Eu comecei essa fala dizendo que **5% das empresas conseguem ter sucesso com IA** e **14% dos profissionais ficam mais produtivos**. Esses números não são castigo divino. São consequência de método. **Os outros 86% têm IA. O que falta é processo, planejamento, e métrica que importa.** O que eu te trouxe aqui hoje não é uma bala de prata. É o método que está funcionando pra mim e pro meu time há quase um ano. Se servir pra um de vocês, missão cumprida. Obrigado."

**Slides finais:**
1. QR code da waitlist Ralph Console.
2. Contato (LinkedIn / X / email).
3. Slide de referências (resumido — bibliografia completa neste roteiro).

**Q&A:** Reservar 5-10 min depois.

---

## 5. ARGUMENTOS E CONTEÚDOS RESGATADOS PARA ESTENDER

### Da talk anterior do Ralph Loop (que dá pra puxar se sobrar tempo):

#### A. Snippet `ralph.sh` simples
Mostrar literalmente o while-loop com stop hook em ~15 linhas pra desmistificar. *"O script é bobo de propósito. O poder está no `CLAUDE.md` que ele alimenta."*

#### B. Live coding mini de Road Rush
Você já fez talk usando Ralph Loop pra construir Road Rush (jogo de corrida arcade em Canvas 2D). É um excelente "vamos ver isso funcionando" se quiser uma demo visual. Pode ser substituído por screencast pra não comer 20 min ao vivo.

#### C. Comparação de complexidade — task simples vs Ralph
"Pra implementar essa feature manualmente eu levaria 3 dias. Com Ralph rodando enquanto eu fazia outra coisa: 4 horas de máquina + 30 min de revisão minha."

### Da talk anterior do Ralph Console:

#### D. Slide do "Whiplash gap" (CircleCI)
Visual com top 5% das equipes vs mediana — top dobrou throughput, mediana só aumentou 4%. *"AI doesn't create a performance gap; it reveals it."*

#### E. Os 4 padrões da CircleCI/Thoughtworks pra escapar do whiplash:
1. Internal Developer Platforms.
2. Test strategies redesenhadas pra código gerado por IA.
3. AI no ciclo todo (não só na geração de código).
4. **DORA Metrics ao invés de throughput bruto.**

#### F. Insights Engine — INS-01 a INS-16
Se a audiência for muito técnica (DevOps, Eng. Lead), pode mostrar 1-2 insights compound-trigger pra dar gostinho do que vem por aí no Ralph Console.

### Conteúdo novo a incorporar (eleva o nível da talk):

#### G. Skills do Claude Code como interface mental compartilhada
- *"Um skill é um slash command reutilizável que dá ao Claude instruções específicas pra uma tarefa."* — [Claude Code Docs](https://code.claude.com/docs/en/skills).
- Ponto importante: skills viraram a forma canônica (substituindo `commands/`).
- Exemplo: `/prd` é skill. `/qa-checklist` é skill. Cada empresa cria as suas → memória organizacional codificada.

#### H. Comparativo dos frameworks SDD em 1 slide
| | GitHub Spec Kit | Kiro (AWS) | BMAD-METHOD | Ralph Loop | cc-sdd |
|---|---|---|---|---|---|
| Origem | GitHub (set/2025) | AWS (jul/2025) | Comunidade | snarktank | gotalab (Kiro-inspired) |
| Foco | Spec → plan → tasks → impl | IDE com EARS notation | Multi-agente orquestrado | Loop autônomo via bash | Skills mode + per-task review |
| Multi-tool | Sim | Não (proprietary IDE) | Sim | Sim (Claude/Amp/OpenCode) | Sim (8 agentes) |
| Living spec | Não | Parcial | Sim | Não (mas progress.txt) | Sim |

Fonte: [Augment Code — 6 Best SDD Tools 2026](https://www.augmentcode.com/tools/best-spec-driven-development-tools).

#### I. Prosumer / Bottom-up — quem dá certo
MIT NANDA: as empresas que dão certo deixam **power users** experimentarem antes de centralizar. "Prosumers" intuitivamente entendem capacidades e limites. Isso justifica por que o Ralph Loop emerge bem em times de 5-15 pessoas (como o seu) — está perto da escala onde o método se prova antes de escalar.

#### J. O risco de cancelamento — Gartner
Gartner: **40% dos projetos de agentic AI serão cancelados até 2027** por custo escalando, valor pouco claro, ou controles de risco insuficientes.
→ Justificativa pra você ter Ralph Console: você está construindo o painel de controle de risco que o Gartner aponta como ausente.

#### K. Linha argumentativa filosófica (opcional, pra fechar com chave de ouro)

> "Engenharia de software sempre foi sobre **lidar com complexidade**. Brooks escreveu *No Silver Bullet* em 1986. Fred Brooks dizia que os ganhos viriam de software design fundamental, não de ferramentas.
> A IA é a ferramenta mais poderosa que vimos em décadas. Mas não é bala de prata — Brooks continua certo. **O que muda é que agora a complexidade pode escalar tão rápido quanto a IA gera código. Se você não tem processo, ela te enterra.** Se você tem, ela te liberta."

---

## 6. BIBLIOGRAFIA COMPLETA

### Estudos primários

1. **MIT Project NANDA — "The GenAI Divide: State of AI in Business 2025"** (jul/2025) — https://mlq.ai/media/quarterly_decks/v0.1_State_of_AI_in_Business_2025_Report.pdf
2. **METR — "Measuring the Impact of Early-2025 AI on Experienced Open-Source Developer Productivity"** (Becker et al., jul/2025) — https://arxiv.org/abs/2507.09089
3. **METR Update — "We are Changing our Developer Productivity Experiment Design"** (fev/2026) — https://metr.org/blog/2026-02-24-uplift-update/
4. **Chroma Research — "Context Rot: How Increasing Input Tokens Impacts LLM Performance"** (Hong, Troynikov, Huber, jul/2025) — https://research.trychroma.com/context-rot
5. **Liu et al. — "Lost in the Middle: How Language Models Use Long Contexts"** (TACL 2024 / arXiv:2307.03172) — https://arxiv.org/abs/2307.03172
6. **Hsieh et al. — "Found in the Middle: Calibrating Positional Attention Bias"** (arXiv:2406.16008) — https://arxiv.org/pdf/2406.16008
7. **CircleCI — "2026 State of Software Delivery Report"** (sponsored by Thoughtworks, fev/2026) — https://circleci.com/blog/five-takeaways-2026-software-delivery-report/
8. **Google DORA — "2025 State of AI-assisted Software Development"** — sintetizado em https://www.future-processing.com/blog/dora-devops-metrics/
9. **RAND Corporation — análise 80% AI failure rate** (2024-2025) — sintetizado em https://www.pertamapartners.com/insights/ai-project-failure-statistics-2026

### Análises e síntese

10. **Fortune — "MIT report: 95% of generative AI pilots at companies are failing"** (ago/2025) — https://fortune.com/2025/08/18/mit-report-95-percent-generative-ai-pilots-at-companies-failing-cfo/
11. **WorkOS — "Why most enterprise AI projects fail"** (jul/2025) — https://workos.com/blog/why-most-enterprise-ai-projects-fail-patterns-that-work
12. **Faros AI — "What METR's Study Missed"** (jul/2025) — https://www.faros.ai/blog/lab-vs-reality-ai-productivity-study-findings
13. **Sean Goedecke — "Is it worrying that 95% of AI enterprise projects fail?"** (nov/2025) — https://www.seangoedecke.com/why-do-ai-enterprise-projects-fail/
14. **Thoughtworks — perspective on CircleCI 2026 report** (mar/2026) — https://www.thoughtworks.com/insights/blog/generative-ai/a-thoughtworks-perspective-on-circleci-s-2026-state-of-software-
15. **Cerbos — "The Productivity Paradox of AI Coding Assistants"** (set/2025) — https://www.cerbos.dev/blog/productivity-paradox-of-ai-coding-assistants

### Frameworks e ferramentas

16. **GitHub — "Spec-driven development with AI: Get started with a new open source toolkit"** (set/2025) — https://github.blog/ai-and-ml/generative-ai/spec-driven-development-with-ai-get-started-with-a-new-open-source-toolkit/
17. **GitHub Spec Kit (repo)** — https://github.com/github/spec-kit
18. **snarktank/ralph (repo)** — https://github.com/snarktank/ralph
19. **Geoffrey Huntley — "Ralph Wiggum as a Software Engineer"** — https://ghuntley.com/ralph/
20. **gotalab/cc-sdd (Kiro-inspired SDD harness)** — https://github.com/gotalab/cc-sdd
21. **Martin Fowler / ThoughtWorks — comparativo SDD tools** — https://martinfowler.com/articles/exploring-gen-ai/sdd-3-tools.html
22. **EPAM — "Inside Spec-Driven Development"** (jan/2026) — https://www.epam.com/insights/ai/blogs/inside-spec-driven-development-what-githubspec-kit-makes-possible-for-ai-engineering
23. **Augment Code — "6 Best Spec-Driven Development Tools for AI Coding in 2026"** — https://www.augmentcode.com/tools/best-spec-driven-development-tools
24. **Claude Code — "Extend Claude with skills" (docs)** — https://code.claude.com/docs/en/skills

### Babysitting e produtividade

25. **BrainGrid — "The Babysitting is Over"** (jul/2025) — https://www.braingrid.ai/blog/the-babysitting-is-over-a-new-plan/ai-coding
26. **Super Productivity — "What to Do While Waiting for AI Code Assistants"** (jan/2026) — https://super-productivity.com/blog/what-to-do-while-waiting-for-claude-code/
27. **Push to Prod — "The Productivity Ceiling of AI Coding Tools"** (jan/2026) — https://pushtoprod.substack.com/p/stop-babysitting-your-ai-coding-agents
28. **Colin McNamara — "Stop Babysitting Your AI Agents"** (out/2025) — https://colinmcnamara.com/blog/stop-babysitting-your-ai-agents-superpowers-breakthrough

### DORA e métricas

29. **Plandek — "DORA Metrics in the Age of AI"** (jan/2026) — https://plandek.com/blog/dora-metrics-in-the-age-of-ai-how-engineering-leaders-should-measure-delivery-in-2025
30. **GetDX — "What are DORA metrics?"** — https://getdx.com/blog/dora-metrics/
31. **Faros AI — "DORA Report 2025 Key Takeaways"** (set/2025) — https://www.faros.ai/blog/key-takeaways-from-the-dora-report-2025
32. **Exceeds.ai — "DORA Metrics Engineering Effectiveness 2026"** — https://blog.exceeds.ai/dora-metrics-engineering-effectiveness/

### Outras referências

33. **Pertama Partners — "AI Project Failure Rate 2026"** (fev/2026) — https://www.pertamapartners.com/insights/ai-project-failure-statistics-2026
34. **Talyx — "Why 90% of Enterprise AI Implementations Fail"** (jan/2026) — https://talyx.ai/insights/enterprise-ai-implementation-failure
35. **DevOpsDigest — "More Code, Less Software"** (mar/2026) — https://www.devopsdigest.com/more-code-less-software-what-28-million-workflows-revealed-about-the-state-of-software-delivery-in
36. **MorphLLM — "Lost in the Middle LLM"** (fev/2026) — https://www.morphllm.com/lost-in-the-middle-llm
37. **MorphLLM — "Context Rot Complete Guide"** (mar/2026) — https://www.morphllm.com/context-rot

---

## 📌 NOTAS FINAIS PARA O APRESENTADOR

### Cuidados específicos

1. **O dado dos "14%"** que você cita no áudio precisa de fonte. Não encontrei exatamente esse número nas fontes pesquisadas — ele pode ter vindo de uma matéria específica que você leu. **Validar a origem antes de citar em palco**, ou substituir por uma fonte primária equivalente (METR mostra **19% mais lentos**, MIT NANDA mostra **5% sucesso em produtos**, S&P mostra **42% abandonaram em 2025**).

2. **Confirmar grafia "Gabriel Esteblein"** — transcrição original deu "Stablin", presumi correção. Validar antes da apresentação.

3. **Validar URL de waitlist** — usei `ralph.ai-solutions.startse.com` baseado em conversa anterior, mas pode ter mudado.

4. **Considerar cortar** o exemplo da garrafa (overfit/underfit) se sobrar pouco tempo — é poderoso, mas não é central. Vale guardar pra Q&A.

5. **Demo do Ralph ao vivo é arriscada** — recomendo screencast gravado com voz over. Tempo controlado, sem dependência de wi-fi/API.

### Estrutura visual recomendada por slide

- Slides 1-3: Abertura, autoridade, premissa.
- Slides 4-7: **Os números** (5%, 14%, 19%, 70.8%) — cada um sozinho na tela. Big number style.
- Slides 8-10: Armadilha das vanity metrics (tabela CircleCI Whiplash).
- Slides 11-15: Planejamento (`/prd` flow). Pode ser um único slide com 7 passos numerados.
- Slides 16-19: Ralph Loop (fluxo, comparativo, demo).
- Slides 20-23: Context Rot (gráfico Chroma) + Lost in the Middle (curva U) + Babysitting.
- Slides 24-26: CI/CD pipeline visual.
- Slides 27-29: DORA Metrics (tabela), comparativo "Vanity vs DORA".
- Slides 30-33: Ralph Console (DevFluency Score, dimensões, QR waitlist).
- Slides 34-36: Recap, frase final, contato.

### Tempo de prática recomendado

- **1ª passada (60-70 min):** Lendo o roteiro em voz alta, sem cortes. Identifica onde travou.
- **2ª passada (50-55 min):** Cortando muletas linguísticas e duplicações.
- **3ª passada (45-48 min):** Final, com cronômetro por bloco.

Boa palestra! 🚀
