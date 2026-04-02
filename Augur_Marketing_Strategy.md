# Augur — Estratégia de Marketing, Posicionamento e Growth

Documento de estratégia de marketing, posicionamento e crescimento para a plataforma Augur — inteligência para prediction markets focada na América Latina.
Data: 2026-04-01

---

## Sumário Executivo

O Augur é uma plataforma de inteligência para prediction markets focada na América Latina. Num mercado que explodiu de ~$3B para $44B+ em volume global (2023→2025) e que não possui NENHUMA ferramenta em português ou espanhol, o Augur nasce para ocupar esse vazio com três pilares: **sinais inteligentes com IA, educação gamificada, e zero complicação crypto** (PIX direto).

**Estado atual:**

- Protótipo funcional (Next.js 16, dados reais via Polymarket Gamma API)
- Landing page + Dashboard + Signals + Academy (todas com dual-theme Zaun/Piltover)
- Zero usuários (pré-lançamento)
- Monetização: não definida no protótipo (proposta neste documento)
- Plataforma: Web-first (desktop + mobile responsive), app nativo posterior
- Mercado: Brasil primeiro, depois LATAM (ES), depois global (EN)

**Oportunidade central:** O mercado de prediction markets é o equivalente a "bolsa de valores dos eventos futuros" — e está em fase de explosão. Polymarket sozinha fez $9B+ em volume na eleição americana de 2024. Mas toda essa infraestrutura existe apenas em inglês, exige carteira crypto, e foi feita POR traders PARA traders. Não existe nada para o público LATAM que quer participar mas não sabe por onde começar.

**Premissa estratégica:** O Augur NÃO é uma exchange — é um **terminal de inteligência e execução** no modelo MetaTrader/NinjaTrader. O usuário opera por dentro do Augur, mas a execução acontece na Polymarket (e futuramente em múltiplas exchanges como Kalshi via XP/Clear). A estratégia prioriza: (1) educação como porta de entrada, (2) sinais como motor de retenção e monetização, (3) execução integrada como lock-in e segundo stream de revenue.

**Metas de 90 dias (fase de validação):**

1. Lançamento web público com dados reais (Polymarket API)
2. Waitlist de 5.000+ interessados via campanha de conteúdo orgânico
3. 1.000+ usuários cadastrados na plataforma
4. Academy: 500+ usuários completaram a primeira missão
5. Validação de pricing: 50+ assinantes pagantes (signals premium)
6. Conteúdo orgânico: 100K+ impressões totais no Twitter/X + YouTube
7. Posição #1 para "mercados de previsão" no Google Brasil

---

## Índice

0. Contexto e Premissas
1. Análise de Mercado e Oportunidade
2. Análise Competitiva
3. Avaliação do Protótipo Atual (com destaques de alterações)
4. Posicionamento e Mensagem Central
5. Personas de Aquisição
6. Estratégia de Monetização e Pricing
7. Unit Economics e Projeções Financeiras
8. Estratégia de Aquisição (Orgânica + Paga)
9. Growth Loops e Viralidade
10. Gamificação e Retenção (Academy)
11. Criativos e Copy
12. Métricas e KPIs por Fase
13. Orçamento e Alocação
14. Cronograma de Execução — 90 Dias
15. Riscos e Mitigações

---

## 0. Contexto e Premissas

### O Produto

O Augur resolve um problema real: prediction markets são a ferramenta de previsão mais precisa que existe — mais que pesquisas, mais que analistas, mais que modelos estatísticos (Tetlock, "Superforecasting", 2015). Mas para o público LATAM, esse mercado é inacessível por três barreiras:

1. **Idioma** — Tudo em inglês. Polymarket, Kalshi, Manifold — zero conteúdo em PT/ES
2. **Complexidade crypto** — A maioria exige carteira Ethereum, USDC, bridges. Isso elimina 95% do público
3. **Intimidação** — Interfaces de trading são feitas para traders. Quem nunca operou, desiste em 30 segundos

O Augur ataca as três barreiras simultaneamente:

- **Sinais Inteligentes com IA** — Rastreamento de baleias (grandes traders), convergência de mercado, volume anômalo, divergência notícia/preço. Cada sinal vem com contexto: quem é o trader, qual sua acurácia histórica, por que esse movimento importa
- **Academy Gamificada** — Missões progressivas, quizzes interativos, ranking de previsores. Não é um curso — é conhecimento no momento certo (learn-by-doing)
- **Zero Complicação** — Deposite via PIX e comece. Sem carteira, sem seed phrase, sem MetaMask
- **Design Cinematográfico** — Dois temas: Zaun (escuro, neon violeta/azul, partículas flutuantes) e Piltover (claro, dourado Art Deco). Nenhum outro produto no mercado se parece com isso

### Features do Protótipo Atual

| Feature | Status | Dados |
|---------|--------|-------|
| Landing page com proposta de valor | ✅ Funcional | Dual-theme |
| Dashboard com mercados | ✅ Funcional | Polymarket API real |
| Cards de mercado (probabilidade, volume, tendência) | ✅ Funcional | 4 categorias |
| Feed de sinais (whale, convergência, volume, notícia) | ✅ Funcional | Dados mock |
| Paywall de sinais (lock após 3 free) | ✅ Funcional | UI implementada |
| Academy (missões, quiz, leaderboard) | ✅ Funcional | Dados mock |
| Toggle Zaun/Piltover | ✅ Funcional | Ambos os temas |
| Mobile responsive | ✅ Funcional | Hamburger menu |
| API route para mercados | ✅ Funcional | /api/markets |
| Navegação entre páginas | ✅ Funcional | Next.js Link |
| i18n (PT/EN/ES) | ❌ Ausente | — |
| Autenticação/cadastro | ❌ Ausente | — |
| Trading/operação real | ❌ Ausente | — |
| Dados de sinais reais | ❌ Ausente | — |
| Notificações/push | ❌ Ausente | — |

### Premissas do Documento

Este documento usa referências de **quatro verticais** para definir KPIs, dado que prediction markets é uma categoria híbrida:

1. **Fintech/Trading Apps (Brasil)** — Benchmarks de apps como Rico, Clear, Toro, Binance BR. CPI alto (R$8-25), mas retention e LTV superiores
2. **Sports Betting Apps (Brasil pós-regulação)** — Benchmarks de Bet365, Betano, Sportingbet. Mercado massivo (R$100B+ em apostas/ano), CPI competitivo (R$3-8)
3. **Crypto Apps (Brasil)** — Benchmarks de Mercado Bitcoin, Foxbit, Binance. Alta adoção (Brasil top 5 global)
4. **SaaS/Signal Platforms (Global)** — Benchmarks de TradingView, Seeking Alpha, StockTwits. Freemium com alto ARPU nos pagantes

### Tabela de Referência: Benchmarks por Vertical

| Métrica | Sports Betting BR | Crypto BR | Fintech BR | Signal Platforms | Nosso Target |
|---------|-------------------|-----------|------------|-----------------|-------------|
| CPI Android | R$3-8 | R$5-15 | R$8-25 | R$4-12 | R$5-10 |
| D1 retention | 35-50% | 25-35% | 20-30% | 15-25% | 30% |
| D7 retention | 18-28% | 12-18% | 10-15% | 8-15% | 15% |
| D30 retention | 8-15% | 5-10% | 4-8% | 4-8% | 8% |
| Free-to-paid | 5-12% | 3-8% | 2-5% | 3-7% | 5% |
| ARPU mensal (pagante) | R$150-500 | R$30-100 | R$20-60 | R$30-80 | R$39,90 |

**Por que os targets do Augur são ambiciosos mas realistas:**

O Augur combina o melhor de cada vertical:
- **Retenção de betting** (conteúdo que muda todo dia, FOMO de eventos)
- **Educação de crypto** (Academy remove barreira de entrada)
- **ARPU de signal** (informação assimétrica tem alto valor percebido)

### Dados de Mercado (atualizados com pesquisa abril/2026)

- **Prediction markets global:** ~$44B em volume notional (2025). Kalshi ($24.2B) + Polymarket (~$21.5B reportado, mas Paradigm documentou ~50% de double-counting — volume real ~$10-12B) = ~$34-36B reais. Duopólio quase completo (~97.5% do mercado)
- **Kalshi:** Revenue $260M em 2025 (+994% YoY). Valuation $11B (Series E Jan/2026: Paradigm + Sequoia + a16z + ARK). Volume mensal março/2026: $12B (ATH). **Já opera no Brasil via XP/Clear** (investidores profissionais R$10M+)
- **Polymarket:** Nate Silver advisor desde julho/2024. Volume mensal saltou de $111M (jun/2024) para $213M (jul/2024) com entrada de Silver. Dominante em crypto-native
- **Brasil — crypto:** $318.8B em valor de transações crypto em 2024 (+110% YoY). 5º no Chainalysis Global Crypto Adoption Index 2025
- **Brasil — PIX:** 160M+ usuários registrados. Recorde: 250.5M transações em um único dia (06/04/2024), R$124.4B processados. PIX é o método #1 de pagamento para apostadores brasileiros (Pay4Fun, 2024)
- **Brasil — betting:** Mercado regulado desde Jan/2025 (Lei 14.790/2023). Arrecadação legal: R$9.6B+ nos primeiros 3 meses. **Crypto PROIBIDO para B2C** (Ordinance 615, Art. 3)
- **Brasil — prediction markets:** CVM aprovou B3 para operar como instrumento financeiro (profissionais apenas). Grey market: Previas, Palpitada, Futuriza já operam. Ministério da Fazenda estudando regulamentação (março/2026)
- **LATAM — gap:** Zero ferramentas de inteligência/educação para prediction markets em PT/ES. Kalshi via XP é a única entrada, limitada a profissionais
- **Fontes:** Phemex, The Block, Paradigm Research, Kalshi News, Sacra, Gambling Insider, Chainalysis, Banco Central do Brasil, iGaming Brazil, iGaming Business, Finance Magnates, Yogonet, Pay4Fun Research

### Especialistas de Referência

Este documento é fundamentado nos frameworks e pesquisas de:

| Especialista | Área | Obra/Framework | Aplicação no Augur |
|-------------|------|----------------|-------------------|
| **Philip Tetlock** | Forecasting | "Superforecasting" (2015) | Base teórica de por que prediction markets funcionam |
| **Nate Silver** | Previsão estatística | "The Signal and the Noise" (2012), Silver Bulletin | Metodologia de sinais vs ruído |
| **Robin Hanson** | Economia | "Shall We Vote on Values, But Bet on Beliefs?" | Prediction markets como agregadores de informação |
| **Vitalik Buterin** | Crypto/Tecnologia | Escritos sobre prediction markets como bens públicos | Visão de prediction markets descentralizados |
| **Eric Seufert** | Mobile/Growth | Mobile Dev Memo, Heracles Capital | Frameworks de retention, monetização, UA |
| **Nir Eyal** | Produto/Psicologia | "Hooked" (2014) | Hook Model para formação de hábito |
| **Yu-kai Chou** | Gamificação | Octalysis Framework | Base da Academy gamificada |
| **Andrew Chen** | Growth/Network Effects | "The Cold Start Problem" (2021) | Como resolver o cold start de uma plataforma de inteligência |
| **Brian Balfour** | Growth | Reforge, Growth Loops | Loops virais content-driven |
| **Alex Hormozi** | Ofertas/Pricing | "$100M Offers" (2021) | Estruturação da oferta irrecusável |

---

## 1. Análise de Mercado e Oportunidade

### O que são Prediction Markets

Prediction markets permitem comprar e vender contratos sobre o resultado de eventos futuros — eleições, economia, esportes, tecnologia, cultura. O preço reflete a probabilidade estimada pelo mercado. Diferente de apostas tradicionais:

- **Sem "casa"** — É trader contra trader, sem house edge
- **Saída a qualquer momento** — Pode vender sua posição antes do evento resolver
- **Baseado em informação** — O preço agrega a inteligência coletiva de milhares de participantes
- **Mais preciso que pesquisas** — Tetlock demonstrou que "superforecasters" + mercados de previsão superam analistas e pesquisas eleitorais consistentemente

### Por que agora?

**1. Explosão de volume (14x em 1 ano)**

O mercado de prediction markets passou de ~$3B para $44B+ em volume entre 2023 e 2025. A eleição americana de 2024 foi o catalisador — Polymarket se tornou referência global de previsão, citada por NYT, Bloomberg, WSJ. Nate Silver passou a usar Polymarket como fonte primária no Silver Bulletin.

**2. Legitimação institucional**

- Kalshi obteve aprovação da CFTC para mercados de eleições nos EUA (2024)
- Bloomberg e Reuters passaram a publicar odds de Polymarket como indicadores
- A precisão dos prediction markets na eleição de 2024 (acertou todos os swing states) legitimou o mercado para o mainstream

**3. Regulação de betting no Brasil abre porta**

A Lei 14.790/2023 regulamentou apostas esportivas no Brasil. Isso criou:
- Infraestrutura de pagamento (PIX para betting já existe)
- Educação do público sobre "apostas baseadas em eventos"
- Precedente regulatório (se aposta em esporte é legal, por que não em evento político?)
- ~30M de brasileiros já fazem apostas esportivas online (estimativa Jota/2025)

**4. Gap absoluto em LATAM**

Nenhuma plataforma de prediction markets existe em português ou espanhol. O brasileiro que quer participar precisa:
- Ler em inglês
- Ter carteira crypto (MetaMask, Phantom)
- Comprar USDC em exchange brasileira
- Fazer bridge para Polygon
- Navegar interface técnica de trading

Isso elimina 99% do público potencial.

### Dimensionamento do Mercado

**TAM (Total Addressable Market) — LATAM:**

- Brasil: 25M+ com contato crypto + 30M+ em betting online = ~40-50M de brasileiros familiarizados com "operações baseadas em eventos" (overlap significativo)
- LATAM (Brasil + Argentina + México + Colômbia): ~80-120M de adultos com acesso digital que já apostam ou operam crypto
- Receita potencial do mercado de prediction markets LATAM: estimada em $500M-$1B/ano em volume (se atingir 2-3% do volume global)

**SAM (Serviceable Addressable Market):**

- ~5-10M de brasileiros que entendem probabilidades, acompanham eventos, e têm renda para operar
- Perfil: já apostam em betting, operam crypto, ou acompanham bolsa/investimentos
- Dispostos a pagar por informação assimétrica (signals)

**SOM (Serviceable Obtainable Market) — Ano 1:**

- Target realista: 15.000-30.000 usuários cadastrados
- MAU: 5.000-10.000
- DAU: 1.000-3.000
- Assinantes pagantes: 300-700
- Revenue: R$10.000-R$30.000/mês ao fim do ano 1

### Comportamento do Público-Alvo no Brasil

**Onde operam hoje:**

- **Polymarket** — Direto, em inglês, com crypto. Apenas os mais sofisticados
- **Kalshi** — Regulado nos EUA, acesso limitado para brasileiros
- **Betfair Exchange** — Exchange de apostas esportivas. Conceito similar mas limitado a esportes
- **Betting apps** (Bet365, Betano, Sportingbet) — Apostas simples, sem profundidade analítica
- **Twitter/X** — Onde o debate sobre probabilidades acontece (threads de análise)
- **YouTube** — Canais de análise política, econômica, crypto

**Gaps não atendidos (oportunidade do Augur):**

1. **Ninguém traduz a probabilidade em insight** — Polymarket mostra 34% para BTC $200k. E daí? O que isso significa? Quem está comprando? Por quê?
2. **Sem educação** — Não existe material em PT sobre como operar prediction markets
3. **Sem sinais** — Ninguém rastreia baleias, convergência de traders, ou volume anômalo em PT
4. **Sem comunidade LATAM** — Os fóruns são todos em inglês (Reddit, Discord de Polymarket)
5. **Sem análise de mercados relevantes para LATAM** — "Lula 2026", "Selic", "Copa 2026" são mercados que interessam ao brasileiro, mas a cobertura é toda em inglês

### Tendências de Mercado

1. **"Polymarket effect"** — Prediction markets passaram de nicho crypto para mainstream após a eleição de 2024. NYT, Bloomberg, CNN passaram a citar odds como indicadores. Nate Silver virou advisor da Polymarket (julho/2024) — legitimação máxima
2. **AI + prediction markets** — O cruzamento de IA com dados de mercado é a próxima fronteira. Signal generation, sentiment analysis, pattern recognition. Buterin cunhou o termo **"Info Finance"** (nov/2024) — prediction markets como infraestrutura de informação, não especulação
3. **Regulação acelerando** — Kalshi abriu precedente nos EUA. **CVM/B3 já aprovaram no Brasil** (instrumento financeiro). Ministério da Fazenda estudando framework. O Brasil pode ser o 2º país a regular prediction markets formalmente
4. **Gamificação de finanças** — Robinhood provou que gamificar investimentos atrai milhões. **Mas CVM brasileira está aumentando escrutínio sobre apps que gamificam decisões financeiras** — posicionar como educação, não gambling
5. **LATAM como frontier market** — Brasil é o 5º maior mercado crypto ($318.8B em transações 2024), 1º em adoção de PIX (160M+), e tem mercado de betting em explosão (R$9.6B arrecadados nos primeiros 3 meses)
6. **Consolidação em duopólio** — Kalshi + Polymarket controlam ~97.5% do volume global. Espaço para player regional que domine um mercado geográfico (LATAM) antes que os duopolistas o façam
7. **"Info Finance" como narrativa** — Vitalik Buterin (nov/2024): prediction markets são um subconjunto de "info finance" — mecanismos financeiros explicitamente desenhados para extrair e agregar informação. Essa narrativa eleva o produto de "aposta" para "infraestrutura epistêmica"

### Takeaways Estratégicos da Pesquisa

Com base nos dados levantados, 7 conclusões que devem guiar toda a estratégia:

1. **Brasil é o ÚNICO ponto de entrada viável em LATAM** — 5º em crypto, 160M+ PIX, primeiras aprovações de prediction market. Nenhum outro mercado LATAM está perto
2. **A janela regulatória é estreita mas real** — Grey market operators já existem. Ministério da Fazenda estudando. Quem engajar reguladores construtivamente vai moldar as regras
3. **O trilho CVM/instrumento financeiro é superior ao trilho SPA/betting** — "Info finance" evita o backlash regulatório atingindo operadores de sports betting e se alinha com como B3/CVM já pensam
4. **PIX é o payment rail obrigatório** — Crypto proibido para B2C betting. Plataforma PIX-native tem vantagem estrutural sobre TODOS os players globais
5. **O mercado global de $44B não tem player LATAM retail** — Kalshi entrou apenas via XP (profissionais R$10M+). A oportunidade mass-market retail está 100% desatendida
6. **A marca "Augur" requer clearance legal urgente** — Lituus Foundation está ativamente rebootando o protocolo. O nome NÃO está disponível sem verificação
7. **O stack de legitimidade intelectual é o moat** — Tetlock + Hanson + Buterin + Silver fornecem narrativa poderosa de "epistemics sérios, não gambling". Um equivalente brasileiro (economistas, jornalistas, data scientists proeminentes) como embaixadores seria o growth lever mais poderoso

---

## 2. Análise Competitiva

### Landscape: Zero Concorrente Direto em LATAM

O Augur não tem concorrente direto na América Latina. Não existe ferramenta de inteligência para prediction markets em português ou espanhol. Os concorrentes são globais, em inglês, e focados em traders sofisticados.

### Competidores Diretos (Globais)

| Plataforma | Tipo | Volume/Usuários | Diferencial | Fraqueza | Relação com Augur |
|-----------|------|-----------------|-------------|----------|------------------|
| **Polymarket** | Exchange descentralizada (Polygon/USDC) | ~$21.5B volume 2025 (nota: Paradigm documentou ~50% de double-counting; volume real ~$10-12B) | Liquidez, variedade, UX limpa, Nate Silver como advisor | Exige crypto, inglês only, sem educação, sem sinais | **Fornecedor de dados** (API) + concorrente em atenção |
| **Kalshi** | Exchange regulada (CFTC) | $24.2B volume 2025, revenue $260M (+994% YoY). Valuation: **$11B** (Series E Jan/2026, Paradigm + Sequoia + a16z + ARK) | Regulado, mainstream, app stores, ~3% do mercado de sports betting EUA | **⚠️ JÁ ENTROU NO BRASIL via XP/Clear** (apenas investidores profissionais R$10M+, contratos financeiros/econômicos) | Concorrente DIRETO no Brasil — mas apenas para investidores profissionais. Gap massivo no varejo |
| **Manifold Markets** | Play money / sweepstakes | 886 DAU (março/2025, recorde de baixa). Feature de dinheiro real sunset em março/2025 | Qualquer pessoa cria mercado, educacional | Colapsando — play money não sustenta engagement | Irrelevante como concorrente |
| **Metaculus** | Forecasting (não-financial) | ~50K forecasters | Comunidade EA/tech de alta qualidade intelectual, rigor | Sem dinheiro real, nicho acadêmico | Inspiração para Academy |
| **PredictIt** | Exchange regulada | Declinando, incerteza regulatória | First-mover em eleições EUA | Limites de $850, interface datada, possível shutdown | Referência do que NÃO fazer |

### ⚠️ NOVO: Competidores no Brasil (Grey Market)

Dado crítico da pesquisa: **já existem operadores brasileiros de prediction markets em zona cinzenta regulatória:**

| Plataforma | Status | Mercados | Implicação para o Augur |
|-----------|--------|----------|------------------------|
| **Previas** | Operando (grey market) | Política, esportes, entretenimento | First-movers nacionais — Augur precisa diferenciar por sinais + educação, não apenas acesso |
| **Palpitada** | Operando (grey market) | Esportes, política | Mais focado em betting social |
| **Futuriza** | Operando (grey market) | Diversos | Mais recente |

**Implicação estratégica:** O Augur NÃO é o primeiro prediction market no Brasil — mas pode ser o primeiro com **inteligência, educação e design de classe mundial**. O posicionamento de "intelligence platform" (não exchange) continua sendo o diferencial.

### Competidores Indiretos (Brasil)

| Plataforma | Tipo | Relação com Augur |
|-----------|------|------------------|
| **Bet365, Betano, Sportingbet** | Betting esportivo | Público sobreposto (30M+ brasileiros). Augur pode capturar os que querem ir além de esportes |
| **Binance, Mercado Bitcoin** | Crypto exchanges | Público sobreposto (25M+). Augur pode capturar os que querem prediction markets além de crypto |
| **TradingView** | Análise técnica (60M+ MAU) | Modelo de monetização similar (free tools + premium $15-60/mês). Benchmark direto |
| **XP/Clear** | Corretora (parceira Kalshi) | Canal potencial — se Kalshi opera via Clear, Augur pode ser a camada de inteligência sobre |
| **Twitter/X Crypto BR** | Comunidade/análise | Canal de aquisição. Influencers de crypto/política podem amplificar |

### Moat do Augur

1. **First-mover LATAM** — Primeiro a oferecer prediction markets intelligence em PT/ES
2. **Sinais com IA** — Não é raw data — é insight processado com contexto (quem operou, por que importa, qual a acurácia histórica)
3. **Academy gamificada** — Ninguém ensina prediction markets em português. Quem educar, captura
4. **Design diferenciado** — A identidade Zaun/Piltover é única no mercado. Nenhuma plataforma financeira se parece com isso
5. **Zero-friction crypto** — PIX direto elimina a maior barreira de entrada
6. **Curadoria LATAM** — Mercados relevantes para o público brasileiro (eleições BR, Selic, Copa) que ninguém cobre

### Referência Internacional: O que Aprender

| Produto | Lição para o Augur |
|---------|-------------------|
| **Polymarket** | UX clean, mercados bem categorizados, focus on liquidity |
| **TradingView** | Freemium funciona: 90% free users criam ecossistema, 10% pagam premium |
| **Robinhood** | Gamificação atrai massa, mas cuidado com regulação e ética |
| **Duolingo** | Missões progressivas + streak + ranking = retenção de 50%+ D7 |
| **The Athletic** | Conteúdo premium em nicho esportivo pode ter ARPU alto ($8-10/mês) |

---

## 3. Avaliação do Protótipo Atual

### Nota Geral: 7/10

O protótipo é visualmente impressionante e tecnicamente sólido. O design Zaun/Piltover é único no mercado e cria uma identidade memorável. Porém existem **decisões estratégicas que precisam ser revisadas** antes do lançamento.

### O que Funciona Muito Bem

1. **Design é o maior diferencial competitivo** — A identidade visual é cinematográfica. Em um mercado dominado por interfaces genéricas de trading (fundo preto, gráficos verdes), o Augur se destaca brutalmente. O tema Zaun com partículas flutuantes e glow neon é hipnótico. O tema Piltover com Art Deco dourado é elegante. Isso é raridade em fintech.

2. **Market Cards são excelentes** — Mostram probabilidade, volume, traders, tendência de forma clara. A barra de probabilidade animada é um touch brilhante. Labels em PT ("Política", "Subindo", "Encerra em") são corretos.

3. **Signal Cards comunicam valor imediato** — A hierarquia whale > convergência > volume > notícia é intuitiva. Confidence dots são um padrão de UX familiar. O sistema de lock (3 free, depois premium) é a estratégia correta de paywall.

4. **Academy concept é o killer feature** — Nenhum concorrente tem educação gamificada. As missões progressivas (Entenda probabilidades → Paper trade → Identifique sinal → Trade real) são o funil perfeito de onboarding.

5. **Polymarket API integration funciona** — Dados reais, transformação robusta, categorização por tags. Pronto para produção.

### ⚠️ ALTERAÇÕES RECOMENDADAS

Cada item abaixo é um destaque para avaliação. Classificados por criticidade.

---

#### ⚠️ CRÍTICO #1: Conflito de Nome "Augur" — MAIS GRAVE DO QUE PARECIA

**Problema:** "Augur" foi uma das primeiras e mais conhecidas plataformas de prediction markets descentralizados, construída sobre Ethereum (Augur v1 lançada em 2018, v2 em 2020, "Augur Turbo" em 2022 via Chainlink).

**ATUALIZAÇÃO CRÍTICA (pesquisa abril/2026):** O protocolo Augur **NÃO está morto**. A Lituus Foundation (entidade que custodia o treasury do protocolo) publicou um roadmap de reboot em 2025. Lituus Labs, uma segunda equipe de engenharia, está ativamente desenvolvendo migração para L2, melhorias de oracle e modernização de UX. O site augur.net está ativo com messaging "Augur is Rebooting". O token REP continua sendo negociado em exchanges. A marca está ENCUMBERED — tem entidade legal ativa custodiando-a.

**Impacto:**
- Googlar "Augur prediction markets" retorna o protocolo, não esta plataforma
- Lituus Foundation é uma entidade legal ativa que pode reivindicar a marca
- Token REP em exchanges = continuidade econômica do projeto original
- SEO comprometido — competir com anos de backlinks e uma marca em reativação
- Risco legal real de trademark infringement

**Recomendação:** Dada a reativação do protocolo original, **renomear é a opção mais segura**:
1. **Variação do nome (menor risco):** "Augur Labs", "Augur Intelligence", "AugurAI" — diferencia mas não elimina confusão
2. **Nome alternativo (recomendado):** Considerar nomes que mantenham a essência (sacerdote que lê sinais/futuro) sem conflito:
   - "Oráculo" (em PT, mesma ideia)
   - "Presságio" (elegante, em PT)
   - "Sybil" (oráculo grego)
   - "Augure" (variação em PT do latim)
   - "Vidente" (direto, em PT)
3. **Manter "Augur" (alto risco):** Apenas se advogado de PI confirmar que não há trademark ativa registrada pela Forecast Foundation/Lituus Foundation nos mercados-alvo (Brasil, LATAM)

**Decisão URGENTE antes do lançamento.** Consultar advogado de propriedade intelectual IMEDIATAMENTE. Custo de rebrand agora = baixo. Custo de rebrand depois de lançar = altíssimo.

---

#### ✅ DEFINIDO #2: Modelo "MetaTrader" — Plataforma de Inteligência + Execução via Polymarket

**Decisão do fundador:** O Augur é a **plataforma/terminal**, a Polymarket é a **corretora**. O usuário abre operações, vê portfolio e resultados por dentro do Augur, mas a execução acontece de fato na Polymarket. Modelo idêntico à relação MetaTrader → Corretora ou NinjaTrader → Corretora.

**Implicações estratégicas desta decisão:**

| Aspecto | Implicação |
|---------|-----------|
| **"Launch App"** | ✅ MANTÉM — faz sentido, é um app de trading real |
| **Portfolio no Header** | ✅ MANTÉM — mostra saldo real do usuário na Polymarket |
| **Regulatório** | ✅ EXCELENTE — Augur não custodia fundos, não é exchange. A complexidade regulatória fica com a Polymarket. Similar a como MetaTrader não precisa de licença de corretora |
| **Monetização** | Abre stream de revenue via spread/markup nas operações (ver §6) |
| **Onboarding** | Precisa integrar wallet Polymarket ou criar flow de onboarding que abstraia a complexidade |
| **Dependência** | ⚠️ RISCO — Se Polymarket mudar API ou bloquear acesso, core product quebra (mitigação: suportar múltiplas "corretoras" — Kalshi, etc.) |

**Modelo de execução (2 fases — Fase 1+2 juntas no MVP):**

**PRINCÍPIO FUNDAMENTAL:** Se o Augur manda o trader para o Polymarket na Fase 1, ele aprende a operar lá e não volta. O Augur vira growth engine do Polymarket em vez de construir sua própria base. Portanto, **onboarding + execução devem existir desde o dia 1**. O trader nunca precisa saber que "por trás" é Polymarket — a experiência inteira acontece no Augur.

**MVP (lançamento) — "Terminal Completo"**

O MVP já inclui o que seria Fase 1 + 2 juntas:

- **Dashboard com dados reais** (✅ já existe via Polymarket Gamma API)
- **Sinais com IA** em tempo real (whale, convergência, volume, notícia)
- **Academy gamificada** (20+ missões, streaks, leaderboard)
- **Onboarding simplificado dentro do Augur:**
  1. Usuário se cadastra no Augur (email + senha, sem jargão crypto)
  2. Augur cria carteira Polygon automaticamente conectada ao Polymarket — o usuário NÃO precisa saber o que é Polygon, MetaMask ou seed phrase
  3. Augur integra depósito via PIX → converte para USDC → deposita na carteira Polygon do usuário. Tudo em um flow único ("Depositar via PIX")
  4. Usuário opera prediction markets por dentro do Augur — comprar YES/NO, ver portfolio, acompanhar resultados
  5. A execução acontece na Polymarket via API, mas a experiência é 100% Augur
- **Portfolio real** sincronizado com posições na Polymarket
- **Operação completa:** Comprar, vender, sair de posição — tudo dentro do Augur

**Fluxo do usuário no MVP:**
```
Cadastro no Augur (email + senha)
  → Carteira Polygon criada automaticamente (invisível pro usuário)
    → "Depositar" → PIX → USDC → carteira (1 flow, 1 QR code)
      → Academy: "Sua primeira previsão" (missão guiada)
        → Opera no dashboard do Augur
          → Polymarket executa por trás (usuário não vê)
            → Portfolio + P&L + histórico no Augur
```

**Isso é o que diferencia o Augur de simplesmente usar Polymarket:**

| Aspecto | Polymarket direto | Augur |
|---------|-------------------|-------|
| Depositar | Comprar USDC em exchange, bridge para Polygon | PIX (1 QR code) |
| Idioma | Inglês | Português |
| Sinais | Nenhum | Whale tracking, convergência, volume, notícia |
| Educação | Nenhuma | Academy gamificada com 20+ missões |
| Design | Funcional mas genérico | Zaun/Piltover (cinematográfico) |
| Suporte | Discord em inglês | PT-BR nativo |

**Fase 2 — "Multi-Broker Terminal" (6-12 meses pós-lançamento)**
- Suportar Polymarket + Kalshi (via XP/Clear no Brasil) + futuras exchanges
- Roteamento inteligente (melhor preço/liquidez entre exchanges)
- Marketplace de sinais/estratégias da comunidade
- "Augur é onde você opera. Não importa qual exchange está por trás."

**Referências de sucesso deste modelo:**
- **MetaTrader 4/5:** >10M de traders, não é exchange, conecta a 1.500+ corretoras. Revenue: licenciamento + markup. Trader nunca precisa saber qual corretora está executando
- **TradingView:** 60M+ MAU, integra execução via brokers (Interactive Brokers, OANDA). Revenue: subscription + broker referral
- **NinjaTrader:** Terminal premium, execução via brokers. Revenue: licença + comissão por trade
- **Nubank (analogia):** Não é banco (era Easynvest por trás), mas a experiência é 100% Nubank. O usuário não sabe e não precisa saber

**Justificativa (Andrew Chen, "The Cold Start Problem"):** Este é o modelo "Come for the tool, stay for the network" na prática. O tool é o terminal com sinais + onboarding zero-friction. O network é a comunidade de traders/previsores. A Polymarket fornece a liquidez — o Augur fornece a inteligência, a experiência, e o onboarding que a Polymarket nunca vai fazer para LATAM.

**⚠️ NOTAS REGULATÓRIAS CRÍTICAS:**

1. **Criação de carteira Polygon para o usuário:** O Augur está essencialmente operando custódia de chaves privadas. Isso pode enquadrá-lo como "provedor de serviços de ativos virtuais" (VASP) sob a regulação brasileira de crypto (Lei 14.478/2022, regulamentada pelo Banco Central). **Consultar advogado ANTES de implementar.**

2. **Conversão PIX → USDC:** O Augur está intermediando câmbio de moeda fiduciária para ativo virtual. Isso DEFINITIVAMENTE exige parceiro regulado (exchange brasileira licenciada: Mercado Bitcoin, Foxbit, Bitso, etc.) ou licença própria do Banco Central. **Não implementar sem parceiro regulado.**

3. **Modelo mais seguro:** Mesmo com essas complexidades, é mais seguro que operar como exchange própria. O Augur é um frontend que conecta a Polymarket — não cria mercados, não faz market-making, não define odds. A complexidade regulatória está na custódia e no câmbio, não na operação de mercados.

4. **Alternativa de menor risco regulatório:** Em vez de criar carteira Polygon internamente, usar solução de "wallet-as-a-service" de provedor regulado (ex: Fireblocks, Copper, ou exchange BR com API de custódia). Terceiriza a custódia e o câmbio para entidade já licenciada.

---

#### ⚠️ ALTO #3: Design Zaun/Piltover — Quem é o Público Real?

**Problema:** A inspiração Arcane é genial para um público gamer/crypto-native (18-30, masculino, tech-savvy). Mas se o objetivo é "prediction markets acessíveis para todos", o design pode intimidar ou confundir:

- O público de betting (que é a maior porta de entrada) espera interfaces como Bet365/Betano — clean, direta, sem "misticismo"
- O público financeiro (investidores) espera interfaces como TradingView — profissional, dados-heavy
- O público casual espera interfaces como Duolingo — friendly, colorida, sem complexidade visual

**Recomendação:** O design NÃO precisa mudar — é o maior diferencial competitivo. Mas precisa de **contexto**:
- Persona primária deve ser o gamer/crypto-native que JÁ se identifica com a estética (ver personas abaixo)
- A expansão para público mass-market (betting, casual) virá depois, possivelmente com uma versão "simplified" da UI
- O tema Piltover (light) já é mais acessível — pode ser o default para novos usuários, com opção de mudar para Zaun

---

#### ⚠️ ALTO #4: Academy Precisa de Profundidade

**Problema atual:** 4 missões mock (Entenda probabilidades, Paper trade, Identifique sinal, Trade real). Para reter usuários educacionais, precisa de muito mais.

**Recomendação (baseado em Yu-kai Chou, Octalysis):**

A Academy deve acionar 6 dos 8 core drives do Octalysis:

1. **Epic Meaning** (CD1) — "Você está entre os primeiros brasileiros a dominar prediction markets"
2. **Development & Accomplishment** (CD2) — XP, badges, níveis, leaderboard
3. **Empowerment of Creativity** (CD3) — Paper trading com estratégias próprias
4. **Ownership & Possession** (CD4) — "Seu portfolio virtual", conquistas colecionáveis
5. **Social Influence** (CD5) — Leaderboard, comparação com amigos
6. **Unpredictability** (CD7) — Quizzes com mercados reais que mudam todo dia

**Estrutura sugerida (20+ missões em 5 trilhas):**

| Trilha | Missões | Tema | XP |
|--------|---------|------|-----|
| Fundamentos | 5 | O que são prediction markets, probabilidade, expected value | 100-500 |
| Leitura de Mercado | 5 | Interpretar volume, liquidez, movimento de preço | 200-800 |
| Sinais | 4 | Identificar sinais de whale, convergência, anomalia | 300-1000 |
| Paper Trading | 3 | Operar com dinheiro virtual, gerenciar risco | 500-1500 |
| Trader Real | 3 | Depositar, operar real, estratégia de portfolio | 500-2000 |

---

#### ⚠️ MÉDIO #5: Link "Markets" Aponta para Página Inexistente

O Header tem link "Markets" apontando para `/markets`, mas essa rota não existe. Dashboard (`/dashboard`) mostra mercados, mas o link no nav diz "Markets".

**Recomendação:** Ou renomear o link para "Dashboard" ou criar uma página `/markets` dedicada com todos os mercados filtráveis.

---

#### ⚠️ MÉDIO #6: Links "About" e "Como Funciona" são Dead-ends

- Header da landing: "About" aponta para `#` (sem funcionalidade)
- Botão CTA "Como Funciona" na hero section não faz nada

**Recomendação:** Criar seção `/about` com a história do Augur, equipe, visão. "Como Funciona" deve fazer scroll suave para a seção "Por que Augur?" ou para uma nova seção explicativa com 3-4 passos.

---

#### ⚠️ MÉDIO #7: Sinais Mock Não Mudam

Os sinais são hardcoded. Para validar se o público quer sinais, precisa de sinais reais — mesmo que parcialmente automatizados.

**Recomendação MVP de sinais:**
1. **Whale alerts** — Monitorar Polymarket API para trades >$10K e gerar alerta automático
2. **Volume anomaly** — Comparar volume 24h vs média 7d, alertar se >2x
3. **Convergência** — Rastrear top traders via API pública da Polymarket e detectar quando múltiplos operam na mesma direção
4. **News sentiment** — Cruzar manchetes (RSS) com movimento de preço do mercado

Isso é implementável em 2-3 semanas e transforma o protótipo em produto real.

---

#### ⚠️ BAIXO #8: Emojis nos Labels de Filtros da Signals Page

Os filtros de sinais usam emojis: "🐋 Whales", "📊 Convergência", "⚡ Volume", "📰 Notícias". Para consistência com o design premium Zaun/Piltover, considerar trocar por ícones SVG custom (como já é feito nos MarketCards com Lucide icons).

**Recomendação:** Usar ícones do Lucide ou custom SVGs em vez de emojis.

---

## 4. Posicionamento e Mensagem Central

### Posicionamento

**Para** brasileiros e latino-americanos curiosos sobre prediction markets mas que hoje não conseguem participar por barreiras de idioma, crypto e complexidade,
**O Augur é** a primeira plataforma de inteligência e educação para prediction markets em português,
**Que diferente de** Polymarket, Kalshi e betting apps,
**Entrega** sinais inteligentes com IA, educação gamificada, e acesso via PIX — transformando um mercado técnico e intimidador em algo acessível e belo.

### Framework de Posicionamento (baseado em April Dunford, "Obviously Awesome")

| Dimensão | Definição |
|----------|-----------|
| **Alternativas competitivas** | Usar Polymarket em inglês com crypto, apostar em betting apps sem profundidade, ou simplesmente não participar |
| **Atributos únicos** | Sinais AI em PT, Academy gamificada, PIX, design Zaun/Piltover |
| **Valor que os atributos criam** | Entender o que está acontecendo nos mercados de previsão antes de todo mundo, em português, sem complicação |
| **Público que mais se importa** | Brasileiros crypto-curious, traders iniciantes, apostadores que querem upgrade, fãs de política/esportes que querem "skin in the game" |
| **Contexto de mercado** | Prediction markets explodiram 14x, Brasil é top 5 crypto, betting foi regulado, ZERO ferramentas em PT |

### Mensagem Central

> **"O Futuro, Revelado."**

O tagline atual é forte. Funciona em múltiplos níveis:
- Literal: prediction markets revelam probabilidades do futuro
- Aspiracional: você tem acesso a informação que outros não têm
- Místico: alinha com a identidade "Augur" (sacerdote romano)

### Mensagens por Canal

| Canal | Mensagem principal | Ângulo |
|-------|-------------------|--------|
| **Landing page** | "Sinais inteligentes, educação e trading para prediction markets" | Feature-driven, claro |
| **Twitter/X** | "Polymarket em português. Com sinais que Polymarket não tem." | Confronto direto com status quo |
| **YouTube** | "O que as odds de 34% para Bitcoin $200k realmente significam — e quem está por trás" | Educacional + curiosidade |
| **Instagram/TikTok** | "Sabia que você pode ganhar dinheiro prevendo se o Lula ganha em 2026? Sem apostar em esporte." | Curiosidade + novidade |
| **Betting communities** | "Cansou de apostar SÓ em esporte? Prediction markets: eleições, economia, tecnologia, tudo." | Bridge do betting |
| **Crypto communities** | "Prediction markets em PT, com PIX, sinais de whale e Academy gamificada. Finalmente." | Feature-driven para quem já conhece |

### Tom de Voz

- **Confiante mas não arrogante** — Como um amigo trader que sabe mais que você e quer te ensinar
- **Técnico quando necessário, acessível sempre** — Explica "expected value" sem ser condescendente
- **Dados primeiro, opinião depois** — "5 dos top 20 traders compraram YES" é mais forte que "achamos que vai subir"
- **Provocativo com propósito** — "Seu jornal mostra 1 lado. As odds mostram o que as pessoas colocam dinheiro para provar."
- Referência de tom: Nate Silver no Silver Bulletin — analítico, direto, com pitadas de humor
- NUNCA: tom de "guru financeiro", promessas de lucro, ou linguagem de scam crypto ("opportunity of a lifetime", "to the moon")

---

## 5. Personas de Aquisição

Personas definidas com segmentação de monetização (Seufert: whale, dolphin, minnow) e com os frameworks de Tetlock sobre o que torna bons previsores (curiosidade intelectual, pensamento probabilístico, atualização bayesiana).

### Persona 1: "O Crypto Trader" (Persona Primária — 40% do target)

| Aspecto | Detalhe |
|---------|---------|
| **Demografia** | 22-35 anos, masculino predominante, classes A/B |
| **Comportamento** | Opera crypto diariamente, acompanha Twitter Crypto BR, já ouviu falar de Polymarket |
| **Sofisticação** | Alta — entende probabilidades, já usou DEX, sabe o que é USDC |
| **Dor** | Sabe que Polymarket existe mas acha complicado (bridge Polygon, USDC), quer sinais/análise e não raw data |
| **Resultado desejado** | "Saber o que as baleias estão fazendo antes do mercado precificar — e operar com base nisso" |
| **Onde encontrar** | Twitter/X Crypto BR, Discord de crypto, YouTube (Fernando Ulrich, Investidor Sardinha), Telegram |
| **Barreira de entrada** | Baixa para o produto (já entende o conceito), alta para pagar (está acostumado a ferramentas free) |
| **Hook que funciona** | "Whale com 82% de acurácia acabou de comprar $50K YES em [mercado]. Você vai ficar de fora?" |
| **Monetização** | Dolphin→Whale — Pagará pelo premium se os sinais gerarem alpha real |
| **Tetlock profile** | "Fox" (sabe um pouco de muitas coisas, atualiza crenças) — alvo ideal |

### Persona 2: "O Apostador que Quer Upgrade" (30% do target)

| Aspecto | Detalhe |
|---------|---------|
| **Demografia** | 25-40 anos, M/F, classes B/C |
| **Comportamento** | Aposta em Bet365/Betano semanalmente, acompanha esportes e política, usa PIX |
| **Sofisticação** | Média — entende odds esportivas, mas não probabilidades bayesianas |
| **Dor** | Ganha nas odds esportivas mas sente que está limitado. Ouviu falar de "aposta em eleições" mas não sabe como |
| **Resultado desejado** | "Quero apostar em coisas que não são só futebol — eleições, economia, tecnologia. E quero uma vantagem sobre os outros." |
| **Onde encontrar** | Instagram/TikTok de betting, YouTube de tips esportivas, grupos de Telegram de apostas |
| **Barreira de entrada** | Média — conceito é familiar (apostar em resultado), mas "prediction market" é jargão novo |
| **Hook que funciona** | "Cansou de apostar SÓ em esporte? Prediction markets: preveja se o Lula ganha em 2026, se Bitcoin bate $200K, se o Fed corta juros." |
| **Monetização** | Dolphin — Pagará pelo premium se a Academy ensinar e os sinais derem resultado |
| **Bridge de conceito** | "Prediction market = Betfair Exchange para TUDO, não só esporte. Mesma lógica, mais mercados." |

### Persona 3: "O Curioso Político/Econômico" (20% do target)

| Aspecto | Detalhe |
|---------|---------|
| **Demografia** | 28-50 anos, M/F, classes A/B, ensino superior |
| **Comportamento** | Acompanha política e economia, lê Folha/Valor, assiste Globonews, segue analistas no Twitter |
| **Sofisticação** | Alta em política/economia, baixa em trading/crypto |
| **Dor** | Pesquisas eleitorais erram sempre. Analistas divergem. Quer uma forma objetiva de saber "o que o mercado realmente acha" |
| **Resultado desejado** | "Ver a probabilidade real de cada cenário — não a opinião de analista, mas onde as pessoas colocam dinheiro" |
| **Onde encontrar** | Twitter/X (política BR), LinkedIn, podcasts de política/economia, YouTube |
| **Barreira de entrada** | Alta — não quer operar, quer apenas consultar. Precisa ver valor sem depositar |
| **Hook que funciona** | "Pesquisa diz X. Analista diz Y. O mercado — onde as pessoas PAGAM para provar — diz Z." |
| **Monetização** | Minnow→Dolphin — Começa free consultando odds, pode converter para premium pelos sinais em época eleitoral |
| **Tetlock connection** | "Prediction markets são o termômetro mais preciso de probabilidades políticas que existe. Melhor que qualquer pesquisa." |

### Persona 4: "O Estudante de Finanças/Dados" (10% do target — crescimento futuro)

| Aspecto | Detalhe |
|---------|---------|
| **Demografia** | 18-25 anos, M/F, graduação em economia/engenharia/dados |
| **Comportamento** | Estuda finanças/dados, faz cursos online, quer experiência prática |
| **Sofisticação** | Teórica alta, prática baixa |
| **Dor** | Sabe a teoria de probabilidade mas nunca aplicou com dinheiro real. Quer praticar sem risco |
| **Resultado desejado** | "Praticar previsões, construir track record, provar que sou bom nisso" |
| **Onde encontrar** | Universidades, Discord de finanças, Reddit r/investimentos, YouTube educacional |
| **Hook que funciona** | "Academy gratuita. Aprenda prediction markets praticando. Seu track record fica registrado." |
| **Monetização** | Minnow (agora) → Whale (futuro) — Não paga agora, mas será o trader sofisticado de amanhã |

---

## 6. Estratégia de Monetização e Pricing

### Modelo: Freemium com Signal Subscription

O Augur usa modelo freemium com monetização via assinatura de sinais premium. Diferente de apps de conteúdo (Burburinho, GeoNews) que usam ads + subscription, o Augur é uma ferramenta de decisão financeira — ads degradam a percepção de premium e confiabilidade.

**Decisão: ZERO ADS.** Justificativa (Hormozi, "$100M Offers"):

> "Se seu produto ajuda alguém a ganhar dinheiro, o preço deve ser uma fração do valor gerado, e o delivery deve comunicar premium."

Ads em uma plataforma de signals financeiros comunicam "grátis = sem valor". O modelo é: free tier generoso para capturar → premium para monetizar.

### Free Tier (85-90% dos usuários)

**O que inclui:**

- Dashboard completo com todos os mercados (dados reais da Polymarket)
- 3 sinais por dia (whale, convergência, volume — os mais recentes)
- Academy completa (todas as 20+ missões, quizzes, leaderboard)
- Paper trading com portfolio virtual
- Toggle Zaun/Piltover
- Sem limite de uso

**Propósito:** O free tier é o motor de aquisição. Cada usuário free é um potencial evangelist (compartilha mercados interessantes, convida amigos para leaderboard) e um pipeline para premium.

### Premium Tier — "Augur Pro" (target: 5-8% dos MAU)

**O que inclui (além de tudo do Free):**

- Sinais ilimitados em tempo real (sem delay de 15min que free tem)
- Alertas push de sinais críticos (whale alert, convergência máxima)
- Histórico completo de sinais (backtesting)
- "Sinal do Dia" curado pela IA com análise profunda
- Acurácia histórica de cada whale rastreada
- Portfolio analytics avançado
- Badge "Pro" no leaderboard
- Acesso ao Discord/Telegram exclusivo de Pro members

### Pricing

| Plano | Preço | Equivalente Mensal | Desconto |
|-------|-------|-------------------|----------|
| Mensal | R$39,90/mês | R$39,90 | — |
| Trimestral | R$89,90/tri | R$29,97 | 25% |
| Anual | R$239,90/ano | R$19,99 | 50% |

**Racional do pricing (baseado em Hormozi e benchmarks de signal platforms):**

1. **R$39,90/mês** está posicionado como ferramenta profissional, não app casual:
   - Abaixo de TradingView Pro ($14.95/mês = ~R$75), Seeking Alpha Premium ($19.99/mês = ~R$100)
   - Acima de apps de entretenimento (R$9,90-19,90)
   - Posicionamento: "ferramenta que se paga" — se um sinal gerar um trade lucrativo de R$100+, o mês se pagou
   - Comparável a 2 cafés premium por semana — framing de acessibilidade

2. **R$239,90/ano** com 50% de desconto incentiva commitment:
   - Mesmo preço de ~4 meses de Netflix
   - Reduz churn drasticamente
   - Benchmark: TradingView oferece 60% desconto anual, Seeking Alpha 50%

3. **Trial:** 7 dias grátis no plano trimestral e anual. Sem trial no mensal — free tier é o trial infinito.

### Estratégia de Paywall

**Quando mostrar o paywall:**

1. **Sinal #4 do dia** — Ao tentar ver o 4º sinal, paywall com preview borrado + "Este sinal moveu 12% no último mercado similar"
2. **Alerta de whale em tempo real** — Free users recebem com delay de 15min. Paywall: "Receba em tempo real"
3. **Após completar Missão 10 da Academy** — Usuário engajado + educado = pronto para converter. "Pronto para sinais reais? Upgrade para Pro"
4. **Nunca na primeira sessão** — Deixar o usuário explorar, completar 1-2 missões, ver 3 sinais free

**Design do paywall (Hormozi framework):**
- **Dream outcome:** "Saiba o que as baleias sabem, antes de todo mundo"
- **Perceived likelihood:** "82% de acurácia nos últimos 90 sinais de whale" (mostrar track record real)
- **Time delay:** "Sinais em tempo real — não 15 minutos atrasado"
- **Effort & sacrifice:** "R$1,33/dia. Menos que um café."

### Monetização via Trading (Modelo MetaTrader — Fase 2+)

Com a decisão de integrar execução via Polymarket, abre-se um segundo stream de monetização além da subscription:

| Stream | Timeline | Modelo | Revenue Potencial |
|--------|----------|--------|-------------------|
| **Onboarding fee (PIX→USDC)** | MVP (dia 1) | Spread na conversão PIX→USDC embutido no flow de depósito. Usuário deposita R$100 via PIX, Augur fica com 1-2% do spread, restante vira USDC na carteira Polygon | 1-2% de todo volume depositado. Com 1.000 usuários depositando R$500/mês média: R$5.000-10.000/mês |
| **Rebate do taker fee Polymarket** | MVP (dia 1) | Integração via API garante 20% de rebate do taker fee da Polymarket em toda operação executada pelo Augur. Taker fee Polymarket ~0.5-1.25% → rebate de ~0.1-0.25% por operação para o Augur. **Invisível para o usuário — não paga nada a mais** | Com 1.000 traders ativos a $500/mês de volume: $500K volume → $500-1.250/mês. Com escala (5.000 traders, $1.000/mês): $5M volume → $5.000-12.500/mês |
| **Roteamento PIX → USDC (escala)** | M3-6 | Negociar melhores taxas com exchange parceira conforme volume cresce. Ou integrar múltiplos provedores (Mercado Bitcoin, Foxbit, Bitso) para melhor spread | Margem melhora de 1-2% para 1.5-2.5% com volume |
| **Enterprise/API** | Mês 8+ | Vender sinais via API para hedge funds, analistas, desks de trading | R$5.000-20.000/mês por cliente enterprise |
| **Sponsored markets** | Mês 6+ | Empresas pagam para criar/promover mercados sobre seus eventos | R$2.000-10.000 por mercado patrocinado |

**Resumo dos 3 Revenue Streams do MVP (dia 1):**

| Stream | Quando ganha | Quanto | Quem paga |
|--------|-------------|--------|-----------|
| **1. Subscription (Augur Pro)** | Usuário assina premium | R$19,99-39,90/mês | Usuário (voluntário) |
| **2. Rebate taker fee** | Toda operação executada via Augur | 0.1-0.25% do volume | Polymarket (rebate automático via API) |
| **3. Spread PIX→USDC** | Todo depósito via PIX | 1-2% do valor depositado | Embutido no câmbio (usuário não percebe) |

Streams 2 e 3 são **transaction-based** — crescem com volume, não dependem de conversion para premium. Isso significa que até free users geram revenue ao operar. O modelo é significativamente mais robusto que subscription-only.

**Nota sobre o modelo MetaTrader de revenue:** MetaTrader/MetaQuotes ganha dinheiro de 3 formas: (1) licenciamento para corretoras, (2) marketplace de indicadores/bots, (3) comissão indireta via volume. O Augur pode replicar as 3:
1. Se mais exchanges surgirem em LATAM, cobrar para integrar como "corretora" no terminal
2. Marketplace de sinais/estratégias criados por analistas da comunidade (plataforma fica com 20-30%)
3. Volume-based revenue via spread nas operações

---

## 7. Unit Economics e Projeções Financeiras

### Premissas Base

| Métrica | Valor | Fonte |
|---------|-------|-------|
| CPI Brasil geral (Android) | R$3,00 (~$0.59) | Mapendo/Business of Apps 2025 |
| CPI LATAM fintech (Android) | R$6-14 (~$1.20-2.80) | Adjust Finance App Report 2025 (nota: 3-7x acima de CPI geral) |
| CPI Brasil fintech/trading (iOS) | R$15,00 | Benchmark iOS premium (2.5x Android) |
| CPI blended (70% Android / 30% iOS) | R$8,70 | Calculado. Nota: IVT (invalid traffic) em LATAM acima da média global — CPI efetivo 20-40% maior após filtro de fraude |
| Retenção D1 | 30% | Target entre betting (35-50%) e fintech (20-30%) |
| Retenção D7 | 15% | Target entre betting (18-28%) e signal (8-15%) |
| Retenção D30 | 8% | Target entre betting (8-15%) e signal (4-8%) |
| Free-to-paid CVR | 5% | Benchmark signal platforms (3-7%) |
| ARPU mensal (pagante) | R$33,00 | Mix 50% anual (R$19,99) + 30% trimestral (R$29,97) + 20% mensal (R$39,90) |
| Churn mensal premium | 8% | Benchmark SaaS/signal com conteúdo contínuo |
| Custo fixo infra | R$1.500/mês | Vercel Pro + Supabase + Polymarket API + Claude API para sinais |

**Por que D1 de 30% é realista:**

O Augur tem 3 hooks imediatos no primeiro acesso:
1. **Mercados reais com dados ao vivo** — O usuário vê probabilidades de "Lula 2026" e "Bitcoin $200k" no primeiro segundo
2. **Academy Missão 1** — "Entenda probabilidades" é completável em 3 minutos e dá XP + badge
3. **3 sinais free** — "Whale comprou $50K YES" é irresistível para qualquer pessoa financeiramente curiosa

Combinados, esses hooks ativam 3 core drives do Octalysis imediatamente: Development (XP), Unpredictability (sinais), e Epic Meaning ("você está entre os primeiros").

### Projeção Financeira — 12 Meses

**Modelo: UA pago desde M1 para validação rápida, escala com métricas.**

- **Meses 1-3 (validação):** R$5.000/mês em UA a CPI R$8 = 625 installs pagos/mês + orgânico via conteúdo. Objetivo: volume suficiente para significância estatística em retention e conversion (R007)
- **Meses 4-6 (aceleração):** UA pago cresce para R$3.000-6.700/mês somente se unit economics positivo
- **Meses 7-12 (escala):** UA pago cresce até R$15.000/mês cap, orgânico deve ser >40% dos signups

**Projeção mensal — Usuários:**

| Mês | Fase | Budget UA | CPI | Paid | Org | Signups | Org% | MAU | DAU | Premium |
|-----|------|-----------|-----|------|-----|---------|------|-----|-----|---------|
| 1 | Valid | R$5.000 | R$8 | 625 | 500 | 1.125 | 44% | 560 | 168 | 10 |
| 2 | Valid | R$5.000 | R$8 | 625 | 850 | 1.475 | 58% | 780 | 234 | 25 |
| 3 | Valid | R$5.000 | R$8 | 625 | 1.300 | 1.925 | 68% | 1.050 | 315 | 45 |
| 4 | Accel | R$3.000 | R$8 | 375 | 1.500 | 2.400 | 63% | 1.400 | 420 | 65 |
| 5 | Accel | R$4.500 | R$8 | 562 | 1.800 | 3.300 | 55% | 2.000 | 600 | 100 |
| 6 | Accel | R$6.700 | R$8 | 838 | 2.200 | 4.400 | 50% | 2.700 | 810 | 150 |
| 7 | Scale | R$10.000 | R$8 | 1.250 | 2.800 | 6.200 | 45% | 3.800 | 1.140 | 220 |
| 8 | Scale | R$12.000 | R$8 | 1.500 | 3.200 | 7.300 | 44% | 4.700 | 1.410 | 300 |
| 9 | Scale | R$15.000 | R$8 | 1.875 | 3.800 | 9.000 | 42% | 5.800 | 1.740 | 400 |
| 10 | Scale | R$15.000 | R$8 | 1.875 | 4.000 | 9.500 | 42% | 6.600 | 1.980 | 480 |
| 11 | Scale | R$15.000 | R$8 | 1.875 | 4.300 | 10.000 | 43% | 7.400 | 2.220 | 560 |
| 12 | Scale | R$15.000 | R$8 | 1.875 | 4.500 | 10.500 | 43% | 8.200 | 2.460 | 650 |

**Projeção mensal — Revenue e P&L:**

**Premissas de revenue transacional:**
- Traders ativos = ~30% do DAU
- **Turnover ratio: 5x** — Um trader médio opera 5x o valor da conta dele em volume mensal (dado validado com dados reais de operação Polymarket pelo fundador). Ex: conta com R$300 → R$1.500 de volume/mês
- Rebate taker fee: 0.15% do volume (média entre 0.1-0.25%)
- Spread PIX→USDC: 1.5% do depósito mensal

**Derivação do Rev/trader/mês:**

```
Rev por trader = (Conta × 5x turnover × 0.15% rebate) + (Depósito mensal × 1.5% spread)
```

| Fase | Conta média | Volume (5x) | Rebate (0.15%) | Depósito/mês | Spread (1.5%) | **Rev/trader/mês** |
|------|-------------|-------------|----------------|-------------|---------------|-------------------|
| M1-3 (novato) | R$300 | R$1.500 | R$2,25 | R$300 | R$4,50 | **R$6,75** |
| M4-6 (engajando) | R$400 | R$2.000 | R$3,00 | R$350 | R$5,25 | **R$8,25** |
| M7-9 (ativo) | R$500 | R$2.500 | R$3,75 | R$400 | R$6,00 | **R$9,75** |
| M10-12 (maduro) | R$650 | R$3.250 | R$4,88 | R$500 | R$7,50 | **R$12,38** |

Conta média cresce porque: (a) depósitos acumulam, (b) ganhos ficam na conta, (c) traders confiantes depositam mais.

| Mês | Traders | API (1% MAU) | Vol Manual (USD) | Vol API (USD) | Vol Total (USD) | Rev Sub | Rev Txn | Rev Total | Custo | Resultado | Acumulado |
|-----|---------|-------------|-----------------|---------------|-----------------|---------|---------|-----------|-------|-----------|-----------|
| 1 | 50 | 6 | $15K | $36K | **$51K** | R$330 | R$635 | R$965 | R$6.500 | -R$5.535 | -R$5.535 |
| 2 | 70 | 8 | $21K | $48K | **$69K** | R$825 | R$879 | R$1.704 | R$6.500 | -R$4.796 | -R$10.331 |
| 3 | 95 | 11 | $28K | $66K | **$94K** | R$1.485 | R$1.215 | R$2.700 | R$6.500 | -R$3.800 | -R$14.131 |
| 4 | 126 | 14 | $50K | $112K | **$162K** | R$2.145 | R$1.926 | R$4.071 | R$4.500 | -R$429 | -R$14.560 |
| 5 | 180 | 20 | $72K | $160K | **$232K** | R$3.300 | R$2.790 | R$6.090 | R$6.000 | +R$90 | -R$14.470 |
| 6 | 243 | 27 | $97K | $216K | **$313K** | R$4.950 | R$3.840 | R$8.790 | R$8.500 | +R$290 | -R$14.180 |
| 7 | 342 | 38 | $171K | $380K | **$551K** | R$7.260 | R$6.361 | R$13.621 | R$11.800 | +R$1.821 | -R$12.359 |
| 8 | 423 | 47 | $212K | $470K | **$682K** | R$9.900 | R$7.995 | R$17.895 | R$14.000 | +R$3.895 | -R$8.464 |
| 9 | 522 | 58 | $261K | $580K | **$841K** | R$13.200 | R$10.022 | R$23.222 | R$17.000 | +R$6.222 | -R$2.242 |
| 10 | 594 | 66 | $386K | $858K | **$1.24M** | R$15.840 | R$14.058 | R$29.898 | R$17.000 | +R$12.898 | +R$10.656 |
| 11 | 666 | 74 | $433K | $962K | **$1.40M** | R$18.480 | R$16.015 | R$34.495 | R$17.000 | +R$17.495 | +R$28.151 |
| 12 | 738 | 82 | $480K | $1.07M | **$1.55M** | R$21.450 | R$18.020 | R$39.470 | R$17.000 | +R$22.470 | +R$50.621 |

**Cálculo Volume:** Manual = Traders × (Conta × 5x) ÷ 5.0 BRL/USD. API = Vibe coders × (Conta × 100x) ÷ 5.0. Rev Txn = Manual rebate + API rebate + spread PIX→USDC de ambos.
**Volume total ano 1: ~$7.2M** (Manual ~$2.2M + API ~$5.0M)
**1% dos usuários ativos (API) geram 69% do volume e 48% da receita transacional.**

**Cálculo:** Rev Sub = Premium × R$33/mês. Rev Txn = Traders ativos × Rev/trader/mês (derivado acima com 5x turnover). Traders ativos = 30% do DAU (M1: 50, M12: 738). Custo = Infra (R$1.500-2.000) + UA.

**Acumulado 12 meses:**

- Signups total: ~67.125
- MAU mês 12: 8.200
- DAU mês 12: 2.460
- Premium mês 12: 650 assinantes
- Traders manuais mês 12: ~738 | API/Vibe coders mês 12: ~82 (1% MAU)
- Volume total operado ano 1: **$7.2M** (Manual $2.2M + API $5.0M)
- Volume mês 12: **$1.55M/mês** (Manual $480K + API $1.07M)
- **Revenue total: ~R$182.921** (Sub ~R$99.165 + Txn Manual ~R$43.644 + Txn API ~R$40.112)
- Custo total: ~R$132.300 (infra ~R$21.100 + UA ~R$111.200)
- **Resultado ano 1: +R$50.621 (POSITIVO)**
- **Breakeven mensal: Mês 5** (revenue R$6.090 vs custo R$6.000 — primeiro mês positivo)
- **Breakeven acumulado: Mês 10** (acumulado vira positivo: +R$10.656)
- **Revenue M12: R$39.470/mês** (R$21.450 sub + R$18.020 txn)
- **Lucro M12: R$22.470/mês**
- **Revenue crescente:** M5 breakeven mensal, M10 breakeven acumulado, M12 lucro de R$22.470/mês

**Por que investir R$5K/mês em UA desde M1:**

1. **Validação rápida (R007):** 625 installs pagos + ~500 orgânicos = 1.125 no M1. Volume suficiente para significância estatística em D1/D7 retention e free-to-paid conversion. Sem isso, levaria 3+ meses para ter dados confiáveis
2. **Base maior compõe mais rápido:** A base 1.6x maior no fim do M3 (1.050 MAU vs 650) gera mais organic WOM, mais compartilhamento, mais atividade no leaderboard → orgânico cresce mais rápido
3. **Custo controlado:** R$15K total nos 3 primeiros meses. Se as métricas não validarem (D7 < 8%), para e perdeu apenas R$15K + R$4.500 infra = R$19.500. Perda tolerável para a informação obtida
4. **Revenue M12 é 15% maior** (R$30.284 vs R$26.256) e breakeven antecipado em 1 mês (M9 vs M10)

**Evolução do modelo financeiro (comparativo das 3 versões):**

| Métrica | v1: Sub only | v2: 3 streams (manual) | v3: 3 streams + API (atual) |
|---------|-------------|----------------------|----------------------------|
| Revenue M12 | R$18.480/mês | R$30.860/mês | **R$39.470/mês** |
| Volume M12 | — | $480K | **$1.55M** |
| Breakeven mensal | Mês 12 | Mês 8 | **Mês 5** |
| Resultado ano 1 | -R$35.064 | +R$10.509 | **+R$50.621** |
| Lucro M12 | +R$1.480 | +R$13.860 | **+R$22.470** |

### API Traders / Vibe Coders (1% do MAU) — já incorporado na projeção principal

Disponibilizando APIs e ferramentas analíticas, o Augur atrai um segmento de altíssimo valor: **vibe coders** — desenvolvedores que plugam bots e scripts nas APIs para operar automaticamente. Esses usuários geram **100x o depósito em volume mensal** (vs 5x do trader manual), porque seus algoritmos operam 24/7 em múltiplos mercados simultaneamente.

**Premissas (já incluídas na tabela de P&L acima):**
- 1% do MAU são API traders/vibe coders
- Turnover: 100x (vs 5x manual) — validado pelo comportamento de bots em prediction markets
- Mesmo depósito/conta que traders manuais (conservador — na prática, tendem a depositar mais)
- Mesmo rebate (0.15%) e spread (1.5%)

**Revenue por vibe coder vs trader manual:**

| Fase | Trader manual (5x) | Vibe coder (100x) | Multiplicador |
|------|--------------------|--------------------|---------------|
| M1-3 | R$6,75/mês | R$49,50/mês | **7.3x** |
| M4-6 | R$8,25/mês | R$65,25/mês | **7.9x** |
| M7-9 | R$9,75/mês | R$81,00/mês | **8.3x** |
| M10-12 | R$12,38/mês | R$105,00/mês | **8.5x** |

*Derivação M1: (R$300 × 100 × 0.15%) + (R$300 × 1.5%) = R$45 + R$4,50 = R$49,50*

**Concentração de valor — API traders vs manuais (M12):**

| Métrica | Traders manuais (99%) | API/Vibe coders (1%) | % API |
|---------|----------------------|---------------------|-------|
| Usuários M12 | 738 | 82 | 1% do MAU |
| Volume M12 | $480K | $1.07M | **69%** |
| Volume ano 1 | $2.2M | $5.0M | **69%** |
| Rev Txn M12 | R$9.410 | R$8.610 | **48%** |

> **1% dos usuários ativos geram 69% do volume e 48% da receita transacional.**

Isso não é anomalia — é o padrão de toda plataforma de trading. Na Polymarket, os top 1% de wallets geram a maior parte do volume. Em crypto exchanges, bots de arbitragem representam 60-80% do volume.

**Implicação estratégica:**

1. **API é prioridade de produto, não nice-to-have** — Deve existir no roadmap como feature core, não como addon futuro
2. **Developer experience é growth lever** — Documentação de API limpa, SDKs em Python/JS, exemplos de bots = atrai vibe coders organicamente
3. **Pricing de API separado** — Considerar tier de API (free: rate limited, Pro: full access) como stream de monetização adicional
4. **Comunidade de devs = moat** — Se 82 vibe coders estão operando via Augur no M12, eles são stickier que qualquer trader manual (custo de migração dos bots é alto)
5. **Volume de $7.2M/ano é argumento para Polymarket** — Justifica negociar rebate melhor (0.20-0.25% em vez de 0.15%) conforme volume cresce

**Por que o modelo funciona:**

1. **UA pago desde M1 acelera validação** — Dados de retention e conversion em 30 dias, não 90
2. **Subscription tem compound effect** — Cada mês novos premium entram, os antigos renovam (92% taxa de renovação com 8% churn)
3. **Revenue transacional cresce com TODA a base** — Free users que operam geram rebate + spread sem converter para premium
4. **CPI de R$8 é competitivo** — Dentro do range fintech LATAM (R$6-14) e sustentável
5. **Orgânico >40% a partir de M4** — A base paga semeia os growth loops orgânicos
6. **ARPU alto** — R$33/mês sub + R$12/mês txn por trader = modelo robusto

### Gates de Decisão

| Gate | Go (escalar) | Otimizar (repetir) | Stop (apenas orgânico) |
|------|-------------|--------------------|-----------------------|
| Fim mês 1 | D1 > 30%, 500+ signups org | D1 25-30% | D1 < 20% |
| Fim mês 2 | D7 > 15%, 5+ pagantes | D7 10-15% | D7 < 8% |
| Fim mês 3 | 25+ pagantes, D30 > 8% | 15-25 pagantes | < 15 pagantes |
| Cada mês M4+ | Unit economics positivo por cohort | Revenue estabiliza | Revenue cai 20%+ |

---

## 8. Estratégia de Aquisição (Orgânica + Paga)

### 8.1 Princípio Central

> "Eduque o mercado. Quem educa, captura." (Hormozi, "$100M Leads")

Prediction markets em LATAM é um conceito NOVO. Diferente de Burburinho (fofoca) ou GeoNews (notícias) onde o público já entende o produto, aqui precisamos EDUCAR antes de VENDER. A estratégia de aquisição é:

1. **Fase 1 (M1-3): Educação pura** — Conteúdo orgânico que ensina o que são prediction markets, por que funcionam, como participar
2. **Fase 2 (M4-6): Educação + conversão** — Conteúdo continua, agora com CTAs para a plataforma
3. **Fase 3 (M7+): Escala com UA pago** — Criativos baseados nos conteúdos orgânicos que mais performaram

### 8.2 Canais Orgânicos (Meses 1-3)

| Canal | Formato | Frequência | Persona | Meta |
|-------|---------|-----------|---------|------|
| **Twitter/X** | Threads de análise + screenshots de mercados | 2-3/dia | P1, P3 | Autoridade, seguidores, engajamento |
| **YouTube** | Vídeos educacionais (10-15min) + Shorts (60s) | 2 longos + 5 shorts/semana | P1, P2, P3 | Discovery, SEO, conversão |
| **TikTok/Reels** | Vídeos curtos provocativos ("A probabilidade de X é apenas Y%") | 5-7/semana | P2, P4 | Awareness, viralidade |
| **Substack/Newsletter** | "Augur Weekly" — análise semanal dos mercados mais quentes | 1/semana | P1, P3 | Retenção email, autoridade |
| **Reddit** | r/investimentos, r/brasil, r/farialimabets | 2-3 posts/semana | P1, P4 | Community, early adopters |
| **Discord/Telegram** | Comunidade Augur — discussão de mercados, sinais | Sempre ativo | P1, P2 | Retenção, NPS |

### 8.3 Pilares de Conteúdo

**Pilar 1: "O que o mercado realmente acha"**
Pega um evento quente (eleição, decisão do Fed, Copa) e mostra a probabilidade do mercado vs o que pesquisas/analistas dizem. Sempre com dados reais da Polymarket.
- Ex: "Pesquisa Datafolha: Lula 48%. Polymarket: 45%. Quem está certo?"
- Formato: thread Twitter, carrossel Instagram, vídeo curto

**Pilar 2: "Prediction Markets 101"**
Conteúdo educacional puro. O que são, como funcionam, por que são mais precisos que pesquisas. Baseado em Tetlock e Silver.
- Ex: "Por que 800.000 traders são melhores que 1 analista: a ciência por trás dos prediction markets"
- Formato: vídeo longo YouTube, artigo Substack

**Pilar 3: "Signal da Semana"**
Destaque o sinal mais interessante da semana (whale, convergência). Mostra o que aconteceu antes e depois.
- Ex: "Semana passada, 5 dos top 20 traders compraram YES em BTC $200k. O mercado subiu 12% em 3 dias."
- Formato: thread Twitter, short YouTube

**Pilar 4: "Versus"**
Compara prediction markets com alternativas familiares. Betting vs prediction markets. Pesquisa vs prediction markets. Analista vs mercado.
- Ex: "Bet365 vs Polymarket: por que prediction markets pagam mais e são mais inteligentes"
- Formato: vídeo comparativo, carrossel

**Pilar 5: "Real-time Commentary"**
Quando um evento importante acontece, postar em tempo real a reação do mercado. Velocidade > perfeição.
- Ex: "Putin acabou de anunciar X. Mercado moveu de 34% para 52% em 8 minutos. Baleias carregando YES."
- Formato: tweet + screenshot da plataforma

### 8.4 Estratégia de Paid UA (Meses 4+)

**Não começar UA pago antes de validar (Seufert):**
1. D7 retention > 15%
2. Free-to-paid > 3%
3. Pelo menos 1.000 organic signups como baseline
4. Ao menos 1 pilar de conteúdo orgânico com traction comprovada

**Canais de UA pago (priorizados):**

| Prioridade | Canal | Budget teste | CPI esperado | Persona | Tipo |
|-----------|-------|-------------|-------------|---------|------|
| 1 | **Google Ads (Search)** | R$3.000 | R$3-6 | P3 | Intent: "mercados de previsão", "prediction markets Brasil" |
| 2 | **Twitter/X Ads** | R$2.000 | R$5-10 | P1, P3 | Promoted threads (usar orgânico vencedor) |
| 3 | **Meta Ads** | R$3.000 | R$6-12 | P2 | Lookalike de engaged users |
| 4 | **YouTube Ads** | R$2.000 | R$4-8 | P1, P2 | Pre-roll em canais de finança/crypto |
| 5 | **Influencer Marketing** | R$5.000 | R$3-8 (estimado) | Todos | 3-5 micro-influencers crypto/finança (10K-100K) |

### 8.5 ASO (App/Web Store Optimization)

Como o Augur começa web-first, o SEO substitui o ASO tradicional:

**Keywords primárias (PT-BR):**
- mercados de previsão
- prediction markets brasil
- probabilidade eleições 2026
- polymarket em português
- sinais de trading
- apostas em eventos
- previsão de mercado IA

**Conteúdo SEO:**
- Landing pages otimizadas para cada keyword cluster
- Blog com análises de mercados (cada post ranqueia para long-tail keywords)
- Meta: Posição #1 para "mercados de previsão" em 90 dias (concorrência baixíssima em PT)

---

## 9. Growth Loops e Viralidade

### Loop 1: "Compartilhar Mercado" (Content Loop)

```
Usuário vê probabilidade surpreendente no dashboard
  → Compartilha via Twitter/WhatsApp ("Sabia que o mercado dá 34% pro BTC bater $200K?")
    → Amigo clica no link
      → Vê preview com probabilidade + CTA
        → Signup
          → Novo usuário descobre mais mercados → compartilha
```

**Implementação:**
- Botão "Compartilhar" em cada MarketCard com texto pré-formatado
- Preview OG com gráfico de probabilidade (visualmente chamativo)
- Deep link para o mercado específico (web, não exige app)
- **Meta:** K-factor > 0.2

### Loop 2: "Academy Leaderboard" (Social Loop)

```
Usuário completa missão na Academy
  → Sobe no leaderboard
    → Compartilha conquista ("Alcancei nível Analista no Augur 🔮")
      → Amigos veem + curiosidade
        → Signup para competir
          → Completa missões → convida mais
```

**Implementação (Yu-kai Chou, CD5 — Social Influence):**
- Badge compartilhável ao completar cada trilha
- "Desafiar amigo" — enviar quiz com link de referral
- Leaderboard semanal — reset cria urgência recorrente
- **Meta:** 1 em cada 5 usuários convida ao menos 1 amigo

### Loop 3: "Signal Viral" (FOMO Loop)

```
Sinal importante é detectado (whale comprou $100K)
  → Push para Pro members em tempo real
    → Pro member posta no Twitter: "Augur acabou de alertar whale de $100K em [mercado]"
      → Non-members veem → FOMO
        → Signup (free) → Upgrade para Pro para ter alertas em tempo real
```

**Implementação (Nir Eyal, "Hooked" — Variable Reward):**
- Sinais são imprevisíveis por natureza (variable reward perfeito)
- Push notifications com conteúdo real (não genérico)
- "Este sinal gerou X% de retorno" — prova social com dados reais
- **Meta:** 30% dos Pro members compartilham ao menos 1 sinal/semana

### Loop 4: "Previsão Correta" (Status Loop)

```
Usuário faz previsão correta (paper ou real)
  → Sistema notifica: "Parabéns! Sua previsão sobre [X] acertou!"
    → Usuário compartilha: "Acertei [evento] no Augur. Minha acurácia: 72%"
      → Amigos impressionados → curiosidade
        → Signup para competir/provar que também acertam
```

Este é o loop mais poderoso. Prediction markets são sobre **provar que você estava certo**. O ego humano é o melhor motor de viralidade.

---

## 10. Gamificação e Retenção (Academy)

### Framework: Octalysis (Yu-kai Chou)

A Academy do Augur é baseada no Octalysis Framework — 8 core drives que motivam comportamento humano. Prediction markets ativam naturalmente 6 deles:

| Core Drive | Aplicação no Augur | Implementação |
|-----------|-------------------|---------------|
| CD1 — Epic Meaning | "Você está entre os primeiros brasileiros a dominar prediction markets" | Onboarding narrative, badges exclusivos de early adopter |
| CD2 — Accomplishment | XP, níveis (Iniciante → Analista → Trader → Oráculo), badges | 20+ missões progressivas, 5 trilhas |
| CD3 — Empowerment | Criar suas próprias previsões, testar estratégias | Paper trading com portfolio virtual |
| CD4 — Ownership | "Seu portfolio", coleção de badges, track record pessoal | Profile page, estatísticas de acurácia |
| CD5 — Social Influence | Leaderboard, desafios entre amigos, ranking de acurácia | Leaderboard global + entre amigos |
| CD7 — Unpredictability | Quizzes com mercados reais que mudam todo dia, sinais surpresa | Quiz diário, sinal random |

### Dados Reais de Gamificação (Duolingo — transferíveis para Academy)

A pesquisa levantou dados internos do Duolingo sobre impacto de mecânicas de gamificação. Estes são os benchmarks mais relevantes para a Academy do Augur:

| Mecânica Duolingo | Equivalente no Augur | Impacto Medido |
|-------------------|---------------------|----------------|
| **Daily streak** | "Streak de Previsão Diária" — fazer 1 previsão/dia | **+60% commitment; 3.6x retenção D7** para holders de streak (Lenny's Newsletter / Jorge Mazal) |
| **Streak wager** | Apostar coins virtuais na manutenção do streak | **+14% retenção D14** |
| **Leaderboards semanais** | Ranking semanal de acurácia por liga (Bronze→Prata→Ouro) | **+40% completions por semana** |
| **Badges** | "Primeira Previsão Correta", "Streak 5 dias", "Top 10%" | **+30% taxa de completion** |
| **Promoção/rebaixamento de liga** | Tiers de analista: Iniciante → Analista → Trader → Oráculo | **+25% completion** (pressão competitiva) |

**⚠️ RECOMENDAÇÃO DE IMPLEMENTAÇÃO:** O streak diário é a mecânica com maior alavancagem (3.6x D7). Deve ser implementado na Academy como prioridade #1 — "Faça 1 previsão por dia e mantenha seu streak".

**Limitação:** Estes dados vêm de educação de idiomas (Duolingo). A transferência para educação financeira não foi validada independentemente. Usuários de prediction markets podem reagir de forma diferente a mecânicas competitivas se stakes financeiros criarem ansiedade em vez de motivação. Monitorar com A/B test.

### Hook Model (Nir Eyal) para Retenção Diária

| Estágio | Implementação no Augur |
|---------|----------------------|
| **Trigger** | Push: "Mercado de [evento] moveu 8% em 1 hora." / Email matinal: "3 mercados para ficar de olho hoje" |
| **Action** | Abrir o app, ver o que mudou, ler o sinal |
| **Variable Reward** | O sinal é diferente todo dia. "Whale comprou $50K" → o que vai acontecer? |
| **Investment** | Completar missão (XP), fazer previsão (stake pessoal), melhorar acurácia (identity) |

### Estrutura da Academy Expandida

**Trilha 1: Fundamentos (5 missões)**
1. O que são prediction markets? (Quiz: conceitos)
2. Probabilidade vs odds — a matemática que você precisa (Quiz: cálculos)
3. Por que prediction markets são mais precisos que pesquisas (Quiz: Tetlock)
4. Como ler um mercado: probabilidade, volume, liquidez (Quiz prático)
5. Expected value: a decisão racional (Quiz: EV calculation)

**Trilha 2: Leitura de Mercado (5 missões)**
6. Tipos de mercado: binário, categórico, escalar
7. O que volume alto/baixo significa
8. Bid-ask spread e liquidez
9. Calendário de eventos e timing
10. Primeiro paper trade! (Missão prática)

**Trilha 3: Sinais (4 missões)**
11. Whale tracking: por que importa
12. Convergência de traders: o que significa
13. Volume anômalo: detectando informação privilegiada
14. Divergência notícia/preço: quando o mercado discorda da manchete

**Trilha 4: Estratégia (3 missões)**
15. Portfolio management: diversificação de previsões
16. Risk management: quanto apostar em cada mercado
17. Timing: quando entrar e quando sair

**Trilha 5: Trader Real (3 missões)**
18. Como depositar via PIX
19. Seu primeiro trade real (com guardrails de proteção)
20. Construindo track record: seu perfil de previsor

---

## 11. Criativos e Copy

### Regra Geral de Copy

Sempre usar um **DADO REAL e ESPECÍFICO**. Nunca genérico. "Preveja o futuro" é fraco. "O mercado dá 34% pro BTC bater $200K — e 5 baleias acabaram de comprar YES" é forte. Número + fato concreto + implicação > frase bonita.

### Templates de Criativos por Canal

**Twitter/X — Thread (Pilar 1):**
```
Hook: "Pesquisa Datafolha: Lula tem 48% de intenção de voto.

Polymarket (onde pessoas PAGAM para provar): 45%.

Quem está certo?

🧵 Thread ↓"

[7-10 tweets com dados, prints, contexto]

Último: "Quer acompanhar isso em tempo real, em português, com sinais de IA?

Augur — O Futuro, Revelado.
[link]"
```

**YouTube — Vídeo educacional:**
```
Título: "Prediction Markets: por que 800.000 traders preveem melhor que a Datafolha"
Thumbnail: Split de "Datafolha" vs "Polymarket" com odds diferentes
Roteiro: Tetlock → exemplo real (eleição 2024) → como funciona → CTA
```

**TikTok/Reels — Curiosidade:**
```
[Pessoa olhando para o celular, surpresa]
"Sabia que existe um mercado onde você pode ganhar dinheiro prevendo se o Lula vai ganhar em 2026?"
[Mostra tela do Augur com probabilidade]
"Não é aposta esportiva. É prediction market. E o preço mostra a probabilidade REAL — não a opinião de analista."
[CTA: "Link na bio"]
```

**Campanha Específica: "As Odds Dizem"**
Série de conteúdos curtos (5-10/semana) cada um com um mercado real:
- "As odds dizem: 71% de chance do Fed cortar juros em junho"
- "As odds dizem: 34% de chance do BTC bater $200K"
- "As odds dizem: 23% de chance do Brasil ganhar a Copa"
Cada post termina com: "O que VOCÊ acha? Concorda ou discorda? → Augur"

---

## 12. Métricas e KPIs por Fase

### Fase 1: Validação (Meses 1-3)

**North Star:** Signups orgânicos

| KPI | Meta M1 | Meta M2 | Meta M3 | Como medir |
|-----|---------|---------|---------|-----------|
| Signups | 500 | 800 | 1.200 | Analytics |
| D1 retention | >25% | >28% | >30% | Cohort analysis |
| D7 retention | >10% | >12% | >15% | Cohort analysis |
| Academy M1 completion | >50% | >55% | >60% | Event tracking |
| Sinais vistos/user/dia | >2 | >3 | >3 | Event tracking |
| Twitter followers | 500 | 1.500 | 3.000 | Twitter analytics |
| YouTube subscribers | 200 | 600 | 1.200 | YouTube analytics |
| Pagantes | 5 | 12 | 25 | Stripe/RevenueCat |

### Fase 2: Aceleração (Meses 4-6)

**North Star:** Free-to-paid conversion rate

| KPI | Meta M4 | Meta M5 | Meta M6 |
|-----|---------|---------|---------|
| CPI blended (paid) | <R$10 | <R$9 | <R$8 |
| Free-to-paid CVR | 4% | 4.5% | 5% |
| D30 retention | 6% | 7% | 8% |
| MRR (Monthly Recurring Revenue) | R$1.650 | R$2.640 | R$3.960 |
| NPS | >40 | >45 | >50 |
| K-factor | 0.1 | 0.15 | 0.2 |

### Fase 3: Escala (Meses 7-12)

**North Star:** MRR (Monthly Recurring Revenue)

| KPI | Meta M7-9 | Meta M10-12 |
|-----|-----------|-------------|
| MRR | R$5K-11K | R$13K-18K |
| Premium users | 180-330 | 400-560 |
| DAU | 960-1.500 | 1.700-2.160 |
| Organic % of signups | >42% | >42% |
| Churn mensal | <10% | <8% |
| CAC Payback (paid cohorts) | <90 dias | <60 dias |

---

## 13. Orçamento e Alocação

### Budget Total Ano 1: ~R$156.000

| Categoria | M1-3 | M4-6 | M7-12 | Total Ano |
|----------|------|------|-------|-----------|
| **Infraestrutura** | R$4.500 | R$4.800 | R$11.800 | R$21.100 |
| **Paid UA** | R$15.000 | R$14.200 | R$82.000 | R$111.200 |
| **Conteúdo/Design** | R$3.000 | R$4.500 | R$9.000 | R$16.500 |
| **Influencers** | R$0 | R$2.000 | R$5.000 | R$7.000 |
| **Total** | **R$22.500** | **R$25.500** | **R$107.800** | **~R$155.800** |

**Nota:** O investimento de R$15K em UA nos meses 1-3 (R$5K/mês a CPI R$8) garante volume estatisticamente significativo para validação de retention e conversion em CADA um dos 3 meses (R$5K = 625 installs/mês + orgânico). Conforme R007: mínimo 500-1.000 installs para validar D7 retention.

**Nota:** Conteúdo/Design inclui ferramentas de edição de vídeo, design de thumbnails, e eventual freelancer para produção de vídeos (se o fundador não fizer tudo sozinho).

### Alocação de UA por Canal (M4+)

| Canal | % do budget UA | Justificativa |
|-------|---------------|---------------|
| Google Search | 30% | Maior intent. Quem busca "prediction markets" já quer |
| Twitter/X Ads | 20% | Público-alvo está no Twitter crypto/política |
| Meta (FB/IG) | 25% | Escala para P2 (apostadores), lookalike |
| YouTube Ads | 15% | Pre-roll em canais de finance/crypto |
| Influencers | 10% | Micro-influencers crypto/finance |

---

## 14. Cronograma de Execução — 90 Dias

### Semana 1-2: Preparação de Lançamento

- [ ] **URGENTE:** Resolver questão do nome/trademark (pesquisa INPI + consulta advogado PI)
- [ ] **URGENTE:** Consultar advogado sobre custódia de carteira Polygon + intermediação PIX→USDC (Lei 14.478/2022)
- [ ] Implementar autenticação (Supabase Auth — email + senha, sem jargão crypto)
- [ ] Implementar criação automática de carteira Polygon no onboarding (wallet-as-a-service ou SDK Polygon)
- [ ] Integrar parceiro regulado para conversão PIX → USDC (Mercado Bitcoin, Foxbit, ou Bitso API)
- [ ] Implementar sinais reais MVP (whale alerts, volume anomaly via Polymarket API)
- [ ] Integrar Polymarket API para execução de operações (comprar/vender YES/NO)
- [ ] Criar as 5 primeiras missões da Academy com dados reais
- [ ] Configurar analytics (Mixpanel/PostHog)
- [ ] Configurar Stripe para pagamentos de subscription

### Semana 3-4: Lançamento Soft

- [ ] Lançamento público da plataforma web
- [ ] Começar postagens Twitter/X (2-3/dia)
- [ ] Publicar primeiro vídeo YouTube longo ("O que são Prediction Markets — Guia Completo")
- [ ] Abrir canal Telegram/Discord da comunidade
- [ ] Primeira newsletter "Augur Weekly"
- [ ] SEO: publicar 5 artigos para keywords primárias
- [ ] Meta: 500 signups, 200 MAU

### Semana 5-6: Iteração

- [ ] Analisar D1/D7 retention do primeiro cohort
- [ ] A/B test onboarding (Academy-first vs Dashboard-first)
- [ ] Expandir Academy para 10 missões
- [ ] Começar série "As Odds Dizem" nas redes sociais
- [ ] Primeira colaboração com micro-influencer
- [ ] Meta: 800+ signups totais, 12+ pagantes

### Semana 7-8: Expansão Orgânica

- [ ] 5+ vídeos YouTube publicados (2 longos + 3 shorts/semana)
- [ ] Thread Twitter com >100 likes (validação de pilar de conteúdo)
- [ ] Leaderboard da Academy com 200+ participantes
- [ ] Implementar feature "Compartilhar Mercado" com OG preview
- [ ] Feedback loop: pesquisa NPS com primeiros 500 users
- [ ] Meta: 1.200+ signups, 25+ pagantes

### Semana 9-10: Preparação para Scale

- [ ] Analisar unit economics: CAC orgânico, LTV, free-to-paid CVR
- [ ] Se métricas OK: configurar campanha Google Ads (search)
- [ ] Se métricas OK: configurar campanha Twitter Ads (promoted threads)
- [ ] Academy expandida para 15+ missões
- [ ] Sinais expandidos (convergência, news sentiment)
- [ ] Meta: validar D7 >15%, free-to-paid >3%

### Semana 11-12: Decisão de Escala

- [ ] **Gate check:** Se D7 >15% E free-to-paid >3% E 25+ pagantes → GO para paid UA
- [ ] Se métricas abaixo: iterar onboarding, conteúdo, e product antes de escalar
- [ ] Lançar paid UA em 2 canais (Google Search + Twitter)
- [ ] Metas finais dos 90 dias: 2.500+ signups, 50+ pagantes, R$1.650+/mês MRR
- [ ] Post-mortem: o que funcionou, o que não, próximos 90 dias

---

## 15. Riscos e Mitigações

### Risco 1: Regulatório (CRÍTICO) — ATUALIZAÇÃO COM DADOS DE PESQUISA

**Risco:** O cenário regulatório brasileiro para prediction markets está **em fluxo ativo** (abril/2026). Existem DOIS trilhos regulatórios distintos com implicações opostas:

| Trilho | Regulador | Status | Implicação |
|--------|-----------|--------|------------|
| **Instrumento Financeiro** | CVM + B3 | ✅ APROVADO — CVM autorizou B3 a operar prediction markets como valores mobiliários. Contratos binários sobre USD, Ibovespa, Bitcoin. Apenas investidores profissionais (R$10M+) | Legitimação. Kalshi já opera via XP/Clear neste trilho |
| **Aposta/Betting** | SPA (Secretaria de Prêmios e Apostas) | ⚠️ ALERTA — SPA emitiu nota (09/03/2026) afirmando que NENHUM operador está autorizado a operar prediction markets como produto de aposta | Grey market operators (Previas, Palpitada, Futuriza) estão em risco |

**Dados adicionais:**
- Ministério da Fazenda está **ativamente estudando** framework regulatório para prediction markets (março/2026) — decisão definirá precedente para LATAM
- Operadores de sports betting estão **fazendo lobby contra** plataformas de prediction markets (alegam que oferecem produto equivalente sem pagar impostos/licenças)
- **Ordinance 615, Art. 3: crypto é PROIBIDO para transações B2C em betting regulado** — PIX, TED ou débito bancário são obrigatórios
- Grey market operators já existem (Previas, Palpitada, Futuriza) — provam demanda mas arriscam shutdown

**Impacto:** Alto — mas o cenário é MAIS FAVORÁVEL do que parecia. CVM/B3 já aprovaram o conceito.

**Mitigação (atualizada com pesquisa):**
- **Fase 1 (M1-6): Posicionamento como "Info Finance" (Buterin framework)**
  - NÃO operar com dinheiro real. Academy + sinais + paper trading = zero risco regulatório
  - Posicionar como plataforma de INFORMAÇÃO e EDUCAÇÃO, não como exchange/betting
  - Vantagem: alinha com como CVM/B3 já pensam sobre prediction markets (instrumento financeiro, não aposta)
- **Fase 2 (M7+): Avaliar opções com base na evolução regulatória:**
  - **Opção A (recomendada):** Operar como camada de inteligência sobre Kalshi/XP (affiliate/API) — terceiriza risco regulatório
  - **Opção B:** Buscar enquadramento via CVM como plataforma de análise/sinal (similar a TradingView)
  - **Opção C:** Se Ministério da Fazenda criar framework, buscar licenciamento no trilho financeiro (não betting)
  - **Evitar:** Trilho SPA/betting — operadores de sports betting farão lobby contra
- **Contingência:** O modelo "TradingView dos prediction markets" sobrevive INDEPENDENTE da regulação — sinais + educação + paper trading não exigem licença nenhuma
- **Vantagem estrutural:** PIX é o payment rail obrigatório. Plataformas crypto-native (Polymarket) estão PROIBIDAS de operar com dinheiro real no betting brasileiro. Uma plataforma PIX-native tem vantagem regulatória sobre todos os players globais

### Risco 2: Conflito de Nome/Trademark (CRÍTICO — elevado de ALTO)

**Risco:** Augur Protocol está sendo **ativamente rebootado** pela Lituus Foundation (2025 roadmap publicado, Lituus Labs desenvolvendo migração L2, site augur.net ativo com "Augur is Rebooting", token REP em exchanges). A marca tem entidade legal ativa custodiando-a.

**Impacto:** Crítico — rebrand provavelmente necessário.

**Mitigação:**
- **Ação imediata:** Pesquisa de trademark no INPI + USPTO + EUIPO ANTES de qualquer lançamento público
- **Cenário mais provável:** Conflito existe → renomear para nome alternativo (ver opções no §3, ⚠️ CRÍTICO #1)
- **Se por milagre livre:** Registrar "Augur" no INPI imediatamente para mercado brasileiro
- **Custo de rebrand agora vs depois:** Mudar nome antes do lançamento = custo zero. Mudar depois de ter marca estabelecida, domínio, SEO, materiais = custo altíssimo + perda de reconhecimento

### Risco 3: Dependência da Polymarket API (ALTO)

**Risco:** O Augur depende da API Gamma da Polymarket para dados de mercado. Se a Polymarket mudar a API, limitar acesso, ou cobrar, o core product quebra.

**Impacto:** Alto — sem dados, sem dashboard.

**Mitigação:**
- Diversificar fontes: Kalshi API, Manifold API, Metaculus
- Cache agressivo: armazenar dados históricos no próprio banco
- Build próprio: a longo prazo, construir pipeline de dados independente
- Monitorar ToS da Polymarket regularmente

### Risco 4: Educação Insuficiente (MÉDIO)

**Risco:** O público brasileiro não entende prediction markets e o conteúdo educacional não é suficiente para converter.

**Impacto:** Médio — afeta aquisição e retenção.

**Mitigação:**
- Academy como primeiro touch (não dashboard)
- Onboarding guiado com conceitos básicos
- Analogia constante com betting (que 30M+ de brasileiros já fazem): "É como Betfair Exchange, mas para TUDO"
- Conteúdo orgânico educacional massivo nos primeiros 3 meses

### Risco 5: Mercado Pequeno Demais (MÉDIO)

**Risco:** Prediction markets pode ser nicho demais para LATAM — talvez não haja 10K+ pessoas dispostas a pagar.

**Impacto:** Médio — limita revenue.

**Mitigação:**
- O mercado de betting comprova demanda para "apostar em eventos" (30M+ no Brasil)
- A barreira é educação e acesso, não interesse
- Se SOM for menor que esperado: expandir para espanhol (LATAM 2x o mercado), depois inglês
- Pivotar features: analytics para traders profissionais (B2B) como segunda receita

### Risco 6: Design Intimidador para Mass Market (BAIXO)

**Risco:** O design Zaun/Piltover é lindo mas pode intimidar usuários não-tech.

**Impacto:** Baixo — o público primário (P1, P2) é tech-savvy.

**Mitigação:**
- Default para Piltover (tema claro, mais acessível) para novos usuários
- Opção de mudar para Zaun após familiarização
- A/B test: onboarding Zaun vs Piltover para diferentes personas

---

## Apêndice: Resumo de Alterações Recomendadas

Para facilitar a revisão, todas as alterações sugeridas consolidadas:

| # | Criticidade | Alteração | Seção |
|---|-----------|-----------|-------|
| 1 | ⚠️ CRÍTICO | Resolver conflito de nome "Augur" (trademark research) | §3 |
| 2 | ✅ DEFINIDO | Modelo "MetaTrader": terminal de inteligência + execução via Polymarket (decisão do fundador) | §3 |
| 3 | ⚠️ ALTO | Avaliar se design Zaun é default correto ou se Piltover é mais acessível | §3 |
| 4 | ⚠️ ALTO | Expandir Academy de 4 para 20+ missões em 5 trilhas | §3, §10 |
| 5 | ⚠️ MÉDIO | Corrigir link "Markets" (inexistente) no Header | §3 |
| 6 | ⚠️ MÉDIO | Implementar "About" e "Como Funciona" (dead-ends) | §3 |
| 7 | ⚠️ MÉDIO | Trocar sinais mock por sinais reais MVP (Polymarket API) | §3 |
| 8 | ⚠️ BAIXO | Substituir emojis nos filtros por ícones SVG | §3 |
| 9 | ✅ Mantido | "Launch App" mantido — modelo MetaTrader confirma que faz sentido | §3 |
| 10 | ✅ Mantido | Portfolio balance mantido — será sincronizado com Polymarket real (Fase 2). Paper portfolio na Fase 1 | §3 |
| 11 | Novo | Implementar "Compartilhar Mercado" com OG preview | §9 |
| 12 | Novo | Adicionar onboarding guiado (Academy-first) | §10 |
| 13 | Novo | Implementar push notifications para sinais | §10 |
| 14 | Novo | Criar newsletter "Augur Weekly" | §8 |
| 15 | Novo | Criar canal Discord/Telegram da comunidade | §8 |

---

*Documento gerado pelo MarketingMind — Augur Marketing Strategy v1.0*
*Baseado em análise completa do protótipo (código-fonte, UX, API) e frameworks de Tetlock, Silver, Seufert, Hormozi, Yu-kai Chou, Nir Eyal, Andrew Chen, Brian Balfour*
