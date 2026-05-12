# Speaker notes — talk performance com IA

> Notas de fala de cada slide, na ordem da apresentação.
> Pressione `N` durante a talk pra ver na tela.

---

## Slide 1 · CAPA

Você acha que está sendo produtivo usando IA? Mas realmente está? PAUSA LONGA. Deixar a pergunta no ar.

---

## Slide 2 · ABERTURA

Olá pessoal, muito bom dia. Hoje vamos falar sobre produtividade real com IA. Sou Renato Barbosa, Head de Engenharia e Sócio na StartSe. Sou de perfil generalista, passei por várias cadeiras de tecnologia. Entusiasta de open source, acompanho de perto novas soluções que surgem no mercado. Atuo na consultoria de IA da StartSe há mais de 2 anos, ajudando empresas a aplicarem IA do jeito certo. E dentro do meu time, ocupo o papel de inovação, sendo braço de inovação junto aos squads.

---

## Slide 3 · ÍNDICE

Aqui o índice da nossa conversa. As 3 perguntas que respondemos operacionalmente na StartSe: como definir um processo de trabalho com IA na engenharia, como mensurar performance de verdade, e como acompanhar alinhamento estratégico em escala.

---

## Slide 4 · DIAGNÓSTICO - METR

STEP 0 (inicial): Vou contar o experimento. METR é uma organização sem fins lucrativos focada em medir capacidades de IA. Em 2025 fizeram um estudo controlado com 16 devs experientes em projetos open source maduros (5+ anos de contribuição). 246 tarefas reais. Cada tarefa foi randomicamente atribuída pra ser feita COM ou SEM IA. SETA DIREITA - STEP 1: Pergunta 1 - antes de começar, qual a expectativa? +24% mais rápidos com IA. SETA DIREITA - STEP 2: Pergunta 2 - depois de usar, qual a percepção? Ainda achavam que tinham acelerado, +20%. SETA DIREITA - STEP 3: Pergunta 3 - qual a realidade medida? -19% MAIS LENTOS. PAUSA LONGA. SETA DIREITA - STEP 4: Um gap de ~39 pontos percentuais entre o que você ACHA e o que está acontecendo.

---

## Slide 5 · DIAGNÓSTICO - FAROS AI

STEP 0 (inicial): Só a pergunta. Mas espera, entregamos mais com IA? PAUSA pra deixar a pergunta no ar. SETA DIREITA - STEP 1: Sim! Faros AI analisou telemetria real de 22 mil devs em 4 mil times. SETA DIREITA - STEP 2: Os números positivos. Épicos completados por dev +66%. Task throughput +34%. PRs por dev +67%. SETA DIREITA - STEP 3: PAUSA. Mas isso é produtividade? SETA DIREITA - STEP 4: DEPENDE... O estudo se chama Acceleration Whiplash. Tempo de review +441%. Incidentes por PR +242%. Bugs por dev +54%. PRs mergeados sem review +31%. Então a IA acelera o que está na frente e estrangula o que está atrás.

---

## Slide 6 · DIAGNÓSTICO - EHSANI ET AL

Mas a IA não consegue entregar código bom? Sim, consegue. Estudo da Drexel University com 33 MIL PRs agênticos no GitHub: 71,48% são mergeados. OpenAI Codex tem a maior taxa, 82%. Copilot a menor, 43%. Mas a parte interessante é quando você olha os PRs REJEITADOS. Análise qualitativa de 600 PRs rejeitados. 38% foram abandonados pelo reviewer: ninguém revisou o que a IA submeteu. 31% são problemas no próprio PR: duplicação 23%, features indesejadas 4%. 22% são problemas de código: falhas de CI/testes, implementações incorretas. Só 2% são problemas específicos do agente. Olha o que isso está dizendo: o código não é o problema. O processo é o problema.

---

## Slide 7 · DIAGNÓSTICO - SÍNTESE

Pausa de 3 segundos antes de falar. Entregar MAIS não é o mesmo que ser PRODUTIVO. Entregar mais cria volume. Produtividade gera valor. O problema não é entregar código. O problema está no processo embaixo. PAUSA. E aí que entram nossas 3 perguntas operacionais.

---

## Slide 8 · P1 - COMO DEFINIMOS UM PROCESSO

STEP 0: Primeira pergunta. Por que é importante ter um processo? O jeito tradicional de usar IA é abrir o Claude e pedir implementa a feature X. Pode funcionar - mas olha o que acontece na prática. Deixa a demo rodar uns 50 segundos enquanto narra: aqui você pede a feature, ele entrega errado, você corrige. Tenta de novo, quebra outra coisa. Você manda esquecer. Ele tenta com outro approach. Você ainda corrige refresh tokens. Você ainda corrige Redis. Você ainda corrige TypeScript. Finalmente fica bom. Olha o contexto lá em cima já no vermelho. Você tem o que pediu, mas pagou o preço. SETA DIREITA - STEP 1: Esses sintomas você já viu acontecer. SETA DIREITA - STEP 2: Três problemas estruturais. Não replicável, babysitting, context rot.

---

## Slide 9 · P1 - PROBLEMA 1 - NÃO REPLICAVEL

Problema 1: não é replicável. Você pode ser muito bom em escrever prompts. Você conhece os truques, sabe dar contexto, sabe pedir formato de resposta. Mas como você ensina isso pra um time de 15 pessoas? Como você garante que o jeito que VOCÊ consegue resultado seja o mesmo jeito que TODO MUNDO consegue resultado? Sem processo, você vira gargalo do seu próprio time. Você precisa estar em toda interação pra dar dica de prompt. Isso não escala.

---

## Slide 10 · P1 - PROBLEMA 2 - BABYSITTING

Problema 2: Babysitting. Você manda a IA fazer, fica olhando as letrinhas se mexerem na tela. Ela pede permissão, você diz sim. Ela faz uma parte, você valida, solicita mudança, espera de novo. Reprovou, espera, valida... Você virou BABÁ. No tempo que ela trabalha, você devia estar produzindo valor em outra coisa. Alt+Tab. 3, 5 agentes em paralelo. Quem fica olhando IA trabalhar não é produtivo. Tem que mudar o modelo mental de USO da IA pra TRABALHAR COM agentes.

---

## Slide 11 · P1 - PROBLEMA 3 - CONTEXT ROT

Problema 3: Context Rot. Conforme você usa a mesma janela do Claude, o contexto vai inchando. E a performance DEGRADA. Pesquisa da Chroma de julho de 2025: testaram 18 modelos SOTA. De 10 mil pra 100 mil tokens, queda de 20 a 50% de acurácia. O padrão tem nome: Lost in the Middle, curva em U. Atenção alta no começo da conversa, alta no final, PERDIDA NO MEIO. Vale até para os modelos mais novos. Conversa longa com IA igual a lixo.

---

## Slide 12 · P1 - COMO RESOLVEMOS - RALPH LOOP

Como definimos um processo na StartSe? Começamos por um padrão da comunidade. Ralph Loop. Não se prendam ao Ralph Loop especificamente, testem em casa. Mas existem outros: GSD, SDD, BMAD, Compozy. Pega um e roda. O importante não é qual framework você escolhe, é ter um processo padronizado pra plugar com seu time. Ralph Loop é um processo derivado de desenvolvimento orientado a especificação. Eu defino o que quero, e a IA itera em cima da especificação, não em cima de prompts soltos no chat.

---

## Slide 13 · P1 - COMO FUNCIONA O RALPH LOOP

Como funciona na prática. Ao invés de eu abrir a janela e pedir 'implementa X', eu vou seguir um processo de 4 etapas. Etapa 1: Planejar. Eu descrevo a feature, a IA me faz perguntas pra fechar gaps, gera planejamento inicial. Etapa 2: Validar o planejamento. Abro outra janela em paralelo: 'analise esse planejamento de forma crítica', re-revisão por perspectiva. Etapa 3: Solicitar implementação. Com plano validado, agente faz em background. Etapa 4: Validar a implementação. Eu não acompanho letrinhas se mexendo. Eu valido o resultado final.

---

## Slide 14 · P1 - RALPH LOOP NA PRÁTICA

Na prática, o Ralph Loop roda com 3 comandos. Primeiro: skill /prd. Eu descrevo a feature em linguagem natural e essa skill gera um Product Requirements Document estruturado. Segundo: skill /ralph. Ela pega o PRD e gera o plano de execução: tasks, ordem, dependências, critérios de aceite. Tudo num arquivo .md versionado no repo. Terceiro: rodo o ralph.sh, passando a ferramenta - aqui Claude - e quantas iterações ele pode fazer, 15 por exemplo. Ponto importante: ele abre o Claude com a flag dangerously skip permissions. Isso é o que permite o agente rodar autonomamente em background sem precisar eu aprovar cada read, cada write, cada bash. Sem essa flag, você volta pro babysitting. Com ela, o agente trabalha sozinho dentro do worktree isolado. PAUSA pra falar do aviso: dangerously não está no nome por acaso. O agente vai executar comandos sem confirmação, incluindo rm, git push, instalar dependências, chamar APIs. Plano ruim, estrago real. Por isso a etapa 2 com a skill ralph e a segunda janela de validação crítica não são opcionais. Validar o plano antes de soltar o agente é o que separa autonomia produtiva de prejuízo no fim do mês.

---

## Slide 15 · TRANSIÇÃO P1 → P2

Transição. Pausa de 2 segundos. Respondemos a primeira pergunta - como definimos um processo. Ralph Loop, skills, validação. Mas agora vem a segunda pergunta, e ela é igualmente crítica: como mensuramos performance de verdade? Sem isso, você não consegue justificar o investimento, não consegue evoluir, não consegue mostrar pro board que está funcionando.

---

## Slide 16 · P2 - COMO MENSURAMOS PERFORMANCE

Segunda pergunta. Como mensuramos performance? O painel do vendor te mostra o que? Tokens consumidos. Linhas de código geradas. PRs abertos. Janela de contexto. Olha bonito. Inclusive, olha aqui esse gráfico. Esse verdão gigante sou eu, nos últimos 30 dias. 2.5 BILHÕES de tokens consumidos em UM mês. Aqueles risquinhos rasteiros embaixo são meu time todo - várias pessoas. Eu sozinho queimei mais que o time inteiro junto. E aí eu te pergunto: faz sentido eu chegar no board e dizer fomos super produtivos porque consumi 2.5 bilhões de tokens? Claro que não. Token não paga conta. Linhas não geram ROI. PR aberto é PR aberto. Precisamos de outras métricas.

---

## Slide 17 · P2 - QUANDO A MÉTRICA VIRA META

E se você acha que isso é só comigo, é só uma piada do Renato em palestra, deixa eu te contar o que aconteceu na Meta. Abril de 2026. Um funcionário criou um leaderboard interno chamado Claudeonomics. Olha o nome - já é uma piada. Painel que rankeia os 85 mil funcionários da Meta pelo consumo de tokens. Quem consome mais ganha títulos tipo Token Legend, Cache Wizard, Model Connoisseur. Importante: esses números são ESTIMATIVAS apuradas por jornalistas - The Information e Pragmatic Engineer - a partir de relatos internos. A Meta nunca confirmou oficialmente. Mas mesmo com a margem de erro, a ordem de grandeza é absurda. Em 30 dias o time inteiro queimou estimados 60 TRILHÕES de tokens. O top user, sozinho, queimou estimados 281 bilhões num mês. Custo estimado em preço de API da Anthropic: cerca de 900 milhões de dólares em UM MÊS - a Meta provavelmente paga bem menos por contratos enterprise, mas mesmo descontando isso, é absurdo. Aí vem o problema. Engenheiros começaram a deixar agentes rodando sozinhos só pra inflar número. Outros começaram a perguntar pra IA coisas que estavam na documentação interna - só pra subir no ranking. Outros prototipavam features que nunca iam shipar. Vários SEVs - incidentes em produção - foram causados por código IA gerado sem cuidado, porque o cara estava mais preocupado em queimar token que em entregar qualidade. Esse padrão tem nome: tokenmaxxing. Quando você mede a coisa errada, as pessoas otimizam pra coisa errada. A Meta tirou o leaderboard do ar 2 dias depois da história vazar. Lição: token consumido é métrica de input, não de output. É proxy de proxy. Não te diz se algo de valor foi entregue.

---

## Slide 18 · P2 - DORA METRICS

Pra medir performance de engenharia de verdade, começamos pelo DORA. DevOps Research and Assessment, do Google Cloud. Validado em centenas de organizações ao longo de mais de 10 anos. 4 métricas core. Lead Time: tempo da alteração até chegar em produção. Deployment Frequency: com que frequência você entrega. Change Failure Rate: percentual de deploys que falham. Recovery Time: tempo pra restaurar quando algo quebra. Essas métricas dizem se você está entregando rápido E com qualidade. Token não diz isso, lead time diz.

---

## Slide 19 · P2 - DEV FLUENCY

DORA é do mundo pré-IA. Pra times trabalhando com agentes, precisamos de um pilar a mais: Dev Fluency. Esse termo veio das nossas conversas internas e captura algo que o DORA não captura: a fluência do time em CRIAR, OPERAR e EVOLUIR agentes de IA dentro do processo. Como o time está criando skills? Como está evoluindo as específicações? Quanto do trabalho já roda em background sem babysitting? Quanto da operação já está automatizada? Esses são indicadores que dizem se o time está amadurecendo na IA — ou apenas usando ela.

---

## Slide 20 · P2 - RALPH CONSOLE

Quando você junta DORA com Dev Fluency, você tem o Ralph Console. E a ferramenta que construímos pra olhar essas duas dimensões ao mesmo tempo: o quanto você está entregando rápido E com qualidade, e o quanto seu time está amadurecendo na prática com IA. O painel do vendor te dá vaidade. O Ralph Console te dá DECISÃO. Onde alocar esforço, onde ta o gargalo, qual time precisa de mais investimento em método, qual já consegue rodar 5 agentes em paralelo. Ainda está no início, vocês podem entrar na waitlist no QR do final.

---

## Slide 21 · RECAPITULANDO

Antes de seguir, deixa eu fazer uma pausa pra recapitular. O que vimos até aqui? Como definimos um processo com IA? Adotamos o Ralph Loop, junto com outros frameworks possíveis do mercado. Como mensuramos produtividade? Criamos o Ralph Console juntando DORA com Dev Fluency. E agora a terceira pergunta, que é a mais crítica em escala: como eu acompanho a evolução do time todo sem virar microgerente? E aí que entra a última parte da nossa conversa.

---

## Slide 22 · P3 - COMO ALINHAMOS COM A ESTRATEGIA

Terceira pergunta. Como acompanhamos alinhamento estratégico em escala? Como Head de Engenharia, eu gastava grande parte do dia entrando em dailies ao vivo de todos os squads pra entender o que estava sendo priorizado. A pergunta que me fiz: eu precisava ESTAR nas dailies de forma síncrona? Não. Eu precisava da TRANSCRIÇÃO delas. A daily não precisava ser uma reunião, ela precisava ser um INPUT. E aí criei uma skill personalizada que processa esse input automaticamente todo dia: a tech-manager. Vou mostrar como funciona em 2 partes: a anatomia, e o operacional.

---

## Slide 23 · P3 - ANATOMIA DA SKILL

Vamos olhar como a skill funciona por dentro. O corpo da skill define o que ela faz: le todas as transcrições das dailies do Slack, cruza com o board, identifica drift entre o que está sendo discutido é o que está priorizado. Os passos são um pipeline diário: 1 le transcrições, 2 cruza com o board, 3 detecta lacunas, 4 cria card automaticamente ou cobra prazo via Slack, 5 gera resumo do estado da semana. Tudo isso roda de manhã sem eu pedir nada.

---

## Slide 24 · P3 - OPERACIONAL

Como isso aparece operacionalmente? Estrutura do board: cada iniciativa tem dono, squad, status, prazo e link pra discussão. O agente atualiza tudo isso sozinho cruzando com as dailies. E o output mais importante pra mim como Head: o relatório semanal. Toda sexta de manhã eu recebo um documento estruturado: o que foi entregue, o que ficou em risco, onde precisa de decisão minha. Eu não preciso entrar em reunião pra saber. Eu só abro o relatório e sei pra onde redirecionar foco.

---

## Slide 25 · PRA LEVAR PRA CASA

Pra levar pra casa, 3 direcionamentos práticos. Um: defina um processo. Ralph Loop, GSD, BMAD, Compozy, SDD, qualquer um. Mas padronize suas iterações com a IA. Assim você sabe evoluir. Dois: fuja de mensurar tokens, PRs, linhas de código. Você não quer um time viciado em tokens. Você quer uma empresa que entrega resultado. Três: acompanhe o processo. Não é porque funciona hoje que vai continuar funcionando amanhã. As ferramentas evoluem, ainda mais agora. Tendo métricas, você sabe POR QUE trocar da A pra B, e não fica refém de benchmark enviesado.

---

## Slide 26 · FECHAMENTO

E o fechamento. Comecei perguntando se você está sendo produtivo com IA. Agora dá pra responder. Se você tem processo, mede outcomes e mantém alinhamento estratégico em escala, você ESTÁ. Se está olhando token, linha, PR aberto, fazendo babysitting da IA ou usando ela como um chat infinito até ela quebrar, provavelmente ainda não está.

---

## Slide 27 · CONECTE-SE

Antes de fechar, três QRs. Quem quiser receber esta apresentação, me chama no LinkedIn no primeiro QR. Quem quiser entrar na waitlist do Ralph Console, segundo QR. E pra quem ainda não fez, o terceiro QR é o da Bússola Executiva de IA, um diagnóstico gratuito de 5 minutos onde um time de agentes analisa seu perfil. Deixa 30 segundos pra galera escanear sem pressa.

---

## Slide 28 · OBRIGADO

Muito obrigado pelo tempo e atenção. Foi um prazer compartilhar. Excelente evento a todos.

---
