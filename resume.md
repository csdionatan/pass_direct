## Resumo Executivo

**Problema de pesquisa**
- As ferramentas tradicionais de mensuração de expectativas macroeconômicas (surveys e derivativos financeiros) têm limitações sérias: surveys ficam desatualizados rapidamente e oferecem apenas estimativas pontuais; futuros de Fed Funds não capturam toda a distribuição de resultados; SOFR options têm problemas de base e horizonte incompatível com reuniões específicas do FOMC
- O paper pergunta: os mercados preditivos — especificamente a Kalshi, maior plataforma regulada pelo CFTC — oferecem uma alternativa superior para mensurar expectativas macroeconômicas em tempo real?

**Metodologia**
- Dados de trades intraday da Kalshi (2021–2025) para contratos de CPI, Core CPI, PCE, taxa de desemprego, payrolls, PIB e fed funds rate
- Conversão de preços de contratos binários em funções de densidade de probabilidade (PDFs) pelo método model-free: preço do "Yes" = probabilidade risk-neutral do evento; construção da CDF outward a partir da moda para garantir monotonicidade
- Comparação com: Survey of Market Expectations (FRBNY), Bloomberg Consensus, Fed Funds Futures e SOFR Options
- Testes de desempenho (Diebold-Mariano), Probability Integral Transform (PIT) para calibração, e regressões de event-study para respostas a notícias

**Principais resultados**
- Para fed funds rate: Kalshi performa comparável ao Survey of Market Expectations; a moda da distribuição Kalshi teve erro absoluto zero no dia de cada reunião do FOMC desde 2022 — melhoria estatisticamente significativa sobre fed funds futures
- Para CPI headline: Kalshi (mediana/moda) apresenta erro médio absoluto significativamente menor que o Bloomberg Consensus; para Core CPI e desemprego, performance é estatisticamente equivalente
- Kalshi é o único instrumento financeiro ativo que fornece distribuição de probabilidades sobre decisões em reuniões específicas do FOMC; a única fonte de distribuições de mercado para PIB, Core CPI e desemprego
- CPI positivo eleva a média da taxa de juros esperada 4x mais do que CPI negativo de mesma magnitude — assimetria estatisticamente significativa
- Shocks no comunicado do FOMC elevam média e variância da distribuição; shocks na coletiva de imprensa reduzem significativamente a assimetria (skewness), sugerindo resolução de incerteza de alta
- Distribuições Kalshi são bem calibradas (PIT próximo a uniforme); alguma evidência de prêmios de risco inflando levemente probabilidades de alta inflação/desemprego

**Implicações de política**
- Kalshi pode complementar ferramentas tradicionais do Fed para monitorar expectativas de mercado em tempo real entre reuniões do FOMC
- Distribuições completas (não apenas médias) permitem avaliar riscos de cauda — riscos de estagflação ficaram visíveis em abril de 2025 após anúncios de política comercial
- A perspectiva do investidor de varejo pode oferecer sinal complementar ao mercado institucional (SOFR), potencialmente menos distorcido por prêmios de hedge

**Limitações**
- Probabilidades são risk-neutral (medida Q), não necessariamente iguais às probabilidades físicas (medida P) — presença de prêmios de risco
- Contratos de cauda sofrem com baixo volume e preços stale; monotonicidade forçada é uma solução parcial
- Período amostral curto (desde 2021/2022); muitos resultados são sensíveis ao episódio 2022–2025 de inflação elevada
- Base de usuários predominantemente de varejo pode introduzir vieses comportamentais distintos do mercado institucional

---

## Outline da Apresentação (12 Slides)

| # | Slide | Elemento Visual Chave |
|---|-------|-----------------------|
| 1 | Título + contexto | Logotipo Fed / design institucional |
| 2 | Motivação — por que isso importa? | Cards comparativos das limitações das ferramentas atuais |
| 3 | Questão de pesquisa | 3 perguntas centrais em destaque |
| 4 | Mercados preditivos — como a Kalshi funciona | Diagrama do contrato binário |
| 5 | Dados e metodologia | Timeline + fluxograma de construção das PDFs |
| 6 | Resultado #1 — Desempenho preditivo | Gráfico de erros absolutos médios (Figura 1 do paper) |
| 7 | Resultado #2 — Riqueza distribucional | Comparação Kalshi vs. Fed Funds Futures vs. SOFR |
| 8 | Evidências visuais — Riscos de estagflação | Gráfico de evolução temporal dos riscos de cauda (Figura 13) |
| 9 | Resultado #3 — Respostas assimétricas a notícias | Bar charts de resposta a surpresas de CPI |
| 10 | Implicações para política monetária | Ícones + pontos de ação para o Fed |
| 11 | Limitações e caveats | Grid 2x2 |
| 12 | Conclusão + Q&A | Slide escuro com mensagem central |

---

Agora construindo a apresentação completa:

Slides visualmente limpos e sem problemas. Copiando para outputs.

A apresentação está pronta — 12 slides com roteiro de fala completo em cada um. Aqui vai um resumo do que foi entregue:

**Estrutura da apresentação** (paleta naval executiva — navy/gold/sky blue, adequada para audiência acadêmico-profissional de alto nível):

| Slide | Conteúdo | Layout |
|-------|----------|--------|
| 1 | Título + série FEDS | Dark, institucional |
| 2 | Motivação — falhas das ferramentas atuais | 3 cards comparativos |
| 3 | 3 questões de pesquisa numeradas | Dark, numeração em gold |
| 4 | Como a Kalshi funciona + construção da PDF | Dois painéis |
| 5 | Dados, benchmarks e testes utilizados | Tabela + grid |
| 6 | Resultado #1 — desempenho preditivo | Gráfico de linhas + tabela de resultados |
| 7 | Resultado #2 — riqueza distribucional | Tabela comparativa com Kalshi destacada |
| 8 | Evidências visuais — riscos de estagflação | Gráfico temporal + interpretação |
| 9 | Resultado #3 — respostas assimétricas | Gráfico de barras + regressões |
| 10 | Implicações para política monetária | Grid 3×2 dark |
| 11 | Limitações e caveats | Grid 2×2 com color-coding por tema |
| 12 | Conclusão + Q&A | Dark, mensagem central em gold |

O **roteiro de fala** está nas notas de cada slide — expansível em PowerPoint via painel de notas — com nível de detalhe adequado para uma apresentação de 25–35 minutos.





GEMINI

Aqui está o resumo executivo do artigo "Kalshi and the Rise of Macro Markets", detalhando os pontos solicitados:
### Problema de Pesquisa
 * Ferramentas tradicionais para medir expectativas macroeconômicas, como pesquisas e derivativos financeiros, apresentam limitações: pesquisas perdem a validade rapidamente e frequentemente focam apenas em previsões pontuais sem capturar incertezas, enquanto derivativos são limitados a certos contratos e podem ter baixa liquidez.
 * Diante disso, o artigo introduz e avalia uma nova fonte de dados em tempo real e com incentivos financeiros: os mercados de previsão macroeconômica da plataforma regulamentada Kalshi.
### Metodologia
 * Os autores extraem dados de negociação de alta frequência de contratos binários da Kalshi, que pagam US$ 1 caso o evento especificado ocorra.
 * Os preços de mercado desses contratos de opções são mapeados e convertidos em funções de densidade de probabilidade (PDFs) neutras ao risco e atualizadas diariamente.
 * A performance das previsões implícitas da Kalshi é comparada com abordagens tradicionais baseadas em mercado (futuros de Fed Funds, opções SOFR) e em pesquisas (Pesquisa de Expectativas de Mercado do FRBNY e o consenso da Bloomberg).
 * Foram realizadas regressões de estudo de evento para analisar como os momentos da distribuição da taxa de juros (média, variância, assimetria) respondem a notícias econômicas e surpresas de política monetária.
### Principais Resultados
 * A Kalshi gera previsões de densidade bem calibradas e de atualização rápida, preenchendo lacunas ao fornecer distribuições em tempo real para variáveis que não possuíam opções financeiras, como PIB, desemprego e núcleo de inflação (Core CPI).
 * Para as previsões da taxa básica de juros (Fed Funds) a 150 dias, o erro médio absoluto da Kalshi é bastante semelhante ao de analistas profissionais, e o seu modelo preditivo atinge precisão perfeita (erro zero) um dia antes das reuniões do FOMC, superando os futuros de Fed Funds.
 * Para o CPI cheio (Headline CPI), as expectativas provenientes da Kalshi apresentam uma melhora estatisticamente significativa na precisão da previsão em comparação com o consenso da Bloomberg.
 * As distribuições de expectativas reagem de forma lógica e assimétrica a notícias: surpresas positivas no CPI elevam a média da taxa de juros projetada com uma magnitude quatro vezes maior do que surpresas negativas, ao mesmo tempo em que a variância das distribuições cai, refletindo a resolução de incertezas.
### Implicações de Política
 * Os mercados da Kalshi fornecem aos formuladores de políticas públicas um benchmark contínuo, de alta frequência e com rica distribuição estatística.
 * Acesso a distribuições completas permite que Bancos Centrais entendam riscos de cauda, assimetrias e a verdadeira incerteza do mercado, informações que são perdidas quando apenas estimativas pontuais são analisadas.
 * Os formuladores de política monetária podem usar essas métricas para monitorar em tempo real a eficácia de sua comunicação e a percepção do mercado. A pesquisa apontou, por exemplo, que choques gerados em entrevistas coletivas (press conferences) reduzem significativamente a assimetria da distribuição de juros, indicando que a comunicação pode "cortar" o risco percebido de altas de juros.
### Limitações
 * As probabilidades extraídas dos contratos refletem medidas neutras ao risco, e não probabilidades físicas, o que significa que podem sofrer distorções causadas por prêmios de risco inerentes a investimentos financeiros.
 * O forte foco em investidores de varejo dentro da Kalshi pode alterar as características clássicas de prêmios de risco geralmente moldadas por instituições.
 * Contratos nas extremidades (eventos com probabilidade muito baixa) sofrem frequentemente com baixo volume de negociação, podendo gerar preços ruidosos ou desatualizados.
 * Tentar criar distribuições de probabilidade usando o ponto médio entre as ofertas de compra e venda (*bid-ask spread*) gerou picos de erros de confiabilidade, forçando a metodologia a se basear exclusivamente nos preços dos últimos negócios realizados.
Gostaria que eu explorasse as diferenças de performance entre a Kalshi e a Bloomberg Consensus para algum indicador macroeconômico específico citado no texto?

Estrutura de Slides
Aqui está uma proposta de estrutura para a sua apresentação de 12 slides. Ajustei o nível de profundidade analítica e o jargão técnico para ressoar bem com uma audiência de acadêmicos e profissionais com forte base quantitativa e interesse em alocação de risco e apreçamento de derivativos.
### Slide 1: Título + Contexto
 * **Título Principal:** Kalshi and the Rise of Macro Markets
 * **Autores:** Anthony M. Diercks, Jared Dean Katz e Jonathan H. Wright (Fevereiro, 2026).
 * **O Problema Clássico:** Gerenciar expectativas é central para a política macroeconômica moderna.
 * **A Falha das Ferramentas Atuais:** Pesquisas tradicionais (surveys) tornam-se obsoletas rapidamente e focam em estimativas pontuais sem capturar incertezas. Derivativos financeiros (como futuros de Fed Funds) sofrem com liquidez restrita em certos contratos e limitações estruturais.
### Slide 2: Motivação / Por que isso importa?
 * **A Inovação:** A introdução de mercados de previsão macroeconômica em tempo real, baseados em incentivos financeiros, através da plataforma Kalshi.
 * **O Gap Preenchido:** Fornece distribuições completas e atualizadas continuamente, preenchendo o vazio onde não existem opções financeiras ativas (ex: desemprego, PIB, Core CPI e reuniões específicas do FOMC).
 * **Relevância Prática:** Permite extrair a Função de Densidade de Probabilidade (PDF) neutra ao risco com premissas mínimas em alta frequência.
### Slide 3: Questões de Pesquisa
 * Como a acurácia das previsões implícitas nos mercados da Kalshi se compara às pesquisas tradicionais e aos derivativos de mercado?
 * Como as distribuições de probabilidade respondem a notícias macroeconômicas e surpresas financeiras?
 * Como os sinais de política monetária afetam não apenas a média, mas os momentos superiores (variância, assimetria) da distribuição de juros?.
### Slide 4: Mercados Preditivos (O Conceito Kalshi)
 * **Estrutura Regulatória:** A Kalshi é o maior mercado de previsão regulamentado pelo governo federal dos EUA e supervisionado pela CFTC.
 * **Mecânica do Contrato:** São títulos simples de Arrow-Debreu que pagam US$ 1 se o resultado especificado ocorrer e zero caso contrário.
 * **Construção da Curva:** O conjunto de contratos em um determinado mercado permite a extração de toda a função de densidade de probabilidade neutra ao risco.
### Slide 5: Dados e Metodologia
 * **Dados:** Extração de negociações intraday de contratos binários da Kalshi para variáveis como CPI, payroll e Fed Funds Rate.
 * **Mapeamento de Probabilidade:** O preço de um contrato "Sim" é tratado diretamente como a probabilidade implícita neutra ao risco daquele evento ocorrer.
 * **Tratamento de Caudas:** Para evitar distorções de baixa liquidez nos extremos da distribuição, a metodologia impõe monotonicidade na CDF, construindo a distribuição da moda para fora.
 * **Evitando Ruídos:** O uso do ponto médio do *bid-ask spread* foi descartado por introduzir problemas de confiabilidade, mantendo-se o foco no preço da última negociação.
### Slide 6: Resultado Principal #1 (Acurácia Preditiva)
 * **Federal Funds Rate:** O erro médio absoluto da Kalshi (150 dias à frente) é semelhante ao de previsores profissionais (SME). A mediana e a moda da Kalshi têm um histórico de previsão perfeita (erro zero) no dia anterior ao FOMC.
 * **Inflação (Headline CPI):** O modelo fornece uma melhoria estatisticamente significativa em relação à previsão de consenso da Bloomberg.
 * **Calibração (PIT):** Transformadas Integrais de Probabilidade indicam que as distribuições são razoavelmente bem calibradas, embora haja alguma evidência de prêmio de risco superestimando a probabilidade de alta inflação.
### Slide 7: Resultado Principal #2 (Assimetria e Choques)
 * **Reação ao CPI:** Choques positivos no CPI geram um ajuste na média da taxa de juros quatro vezes maior do que choques negativos.
 * **Resolução de Incerteza:** A variância da distribuição das taxas de juros cai substancialmente após divulgações de dados, com a queda mais acentuada ocorrendo quando o indicador vem em linha com o esperado (surpresa zero).
 * **Efeito das Coletivas (Press Conferences):** Choques associados à coletiva de imprensa do Fed não afetam o primeiro momento de forma significativa, mas têm um efeito negativo e expressivo na assimetria (skewness), indicando corte no risco de cauda de alta de juros.
### Slide 8: Evidências Visuais (Vantagem Distribucional)
 * **O Problema dos Futuros Tradicionais:** Modelos baseados em Futuros de Fed Funds forçam a suposição irrealista de apenas dois resultados possíveis (ex: corte de 25 bps ou manutenção).
 * **O Problema do SOFR:** Opções SOFR sofrem com *spreads* em relação à taxa efetiva dos Fed Funds e vieses de alta (upward bias) possivelmente causados por demandas de *hedge* institucional.
 * **A Solução Kalshi:** A Kalshi não impõe essas restrições, revelando maior incerteza real do mercado e alocando melhor as massas de probabilidade.
### Slide 9: Precificando Riscos de Cauda (Stagflation)
 * **Distribuição Bidimensional:** A alta frequência permite monitorar em tempo real mudanças nas distribuições de resultados macro após grandes eventos.
 * **Risco de Estagflação:** O paper demonstra a evolução diária dos riscos de cauda (ex: peso de cenários com CPI > 3% e PIB < 1,5%).
 * **Varejo vs Profissionais:** A Kalshi (mercado com apelo ao varejo) colocou um peso muito maior em cenários de "estagflação severa" (CPI > 4% ou PIB < 0%) em comparação com o Survey of Professional Forecasters.
### Slide 10: Implicações para Política Monetária e Mercados
 * **Para o Banco Central:** Melhora a capacidade do Fed de comunicar a direção da política e avaliar a função de reação percebida pelo mercado sob vários cenários.
 * **Para Gestão de Risco/Trading:** Fornece a melhor estimativa de densidade disponível para os juros de curto prazo, livre da distorção temporal do SOFR. Entender os prêmios gerados por investidores de varejo (em oposição às necessidades de *hedge* institucional) pode gerar novas oportunidades sistêmicas de precificação.
### Slide 11: Limitações e Caveats
 * **Probabilidades Físicas vs Neutras ao Risco:** As probabilidades extraídas são da medida Q (neutra ao risco), e não da medida P (probabilidade física atual), podendo estar distorcidas por prêmios de risco.
 * **O Fator Varejo:** A base de investidores de varejo da Kalshi pode alterar as propriedades convencionais dos prêmios de risco.
 * **Falta de Liquidez nas Caudas:** Contratos muito distantes do dinheiro frequentemente sofrem com baixo volume, gerando preços defasados e estimativas ruidosas.
### Slide 12: Conclusão
 * A Kalshi é um complemento valioso às ferramentas de previsão existentes, oferecendo um benchmark robusto que atualiza os dados instantaneamente.
 * A plataforma supera limitações da curva tradicional ao focar diretamente no evento final com granularidade e estrutura de opções completas.
 * À medida que a liquidez se aprofunda, esses mercados abrirão novos caminhos para quantificar incertezas e a eficácia da transmissão da política monetária.
Gostaria que eu rascunhasse algumas notas para o apresentador (*speaker notes*) para os slides mais técnicos, ou que eu detalhasse melhor o processo de extração das probabilidades de Arrow-Debreu?


Apresentacao
Aqui está o conteúdo detalhado para a sua apresentação, estruturado com rigor técnico, adequado para discussões acadêmicas avançadas ou comitês de alocação em *asset management*.
### Slide 1: Título e Contexto
 * **Título:** Kalshi and the Rise of Macro Markets.
 * **Autores:** Anthony M. Diercks, Jared Dean Katz e Jonathan H. Wright.
 * **Data:** 12 de Fevereiro de 2026.
 * **Contexto Central:** O gerenciamento de expectativas é uma métrica central para a formulação da política macroeconômica moderna.
 * **O Problema das Ferramentas Clássicas:** * Pesquisas (*surveys*) tornam-se obsoletas rapidamente e muitas vezes fornecem apenas previsões pontuais (*point forecasts*), sem qualquer medida de incerteza.
   * Derivativos financeiros tradicionais são limitados a certos contratos e a liquidez pode ser muito baixa (*thin*).
### Slide 2: Motivação / Por que isso importa?
 * **A Inovação:** Introdução de uma nova fonte de dados de expectativas em tempo real com lastro financeiro: os mercados de previsão macroeconômica da plataforma Kalshi.
 * **Plataforma Regulada:** A Kalshi é a primeira plataforma regulamentada pelo governo federal dos EUA, supervisionada pela CFTC como um "Designated Contract Market".
 * **A Quebra de Paradigma:** Esses mercados geram previsões de densidade de rápida atualização para variáveis econômicas importantes, preenchendo o vazio existente onde alternativas de derivativos não estavam disponíveis.
### Slide 3: Questões de Pesquisa
 * Avaliar a acurácia das previsões implícitas nos mercados da Kalshi em relação às estimativas de mercado e de pesquisas (*surveys*) tradicionais.
 * Examinar como as expectativas do mercado respondem a notícias macroeconômicas e financeiras.
 * Investigar como os sinais de política monetária são interpretados pelos participantes do mercado.
### Slide 4: O Conceito Kalshi (Mercados Preditivos)
 * **Design do Contrato:** Cada contrato é um título simples de Arrow-Debreu que paga exatamente US$ 1 caso o resultado especificado ocorra.
 * **Distribuição Completa:** Através do conjunto de opções binárias oferecidas em um dado mercado, é possível construir a função de densidade de probabilidade (PDF) neutra ao risco completa de um evento.
 * **Cobertura Macro:** Os contratos fornecem dados intraday para CPI, núcleo do CPI, inflação PCE, taxa de desemprego, *payrolls*, crescimento do PIB, probabilidade de recessão e a taxa alvo dos *Fed Funds* reunião por reunião.
### Slide 5: Dados e Metodologia
 * **Conversão de Preços:** A precificação mapeada baseia-se no preço do contrato "Sim" (Yes), o qual é tratado como a probabilidade neutra ao risco implícita pelo mercado de que o evento ocorrerá.
 * **Controle de Caudas:** Para mitigar distorções relacionadas a eventos de cauda (falta de liquidez), a metodologia impõe monotonicidade na Função de Distribuição Acumulada (CDF), construindo a distribuição de forma projetada a partir da moda em direção às caudas.
 * **Bid-Ask Spread:** Refinamentos utilizando o ponto médio dos *bid-ask spreads* introduziram problemas de confiabilidade devido a *spreads* ocasionalmente longos em resultados de cauda, de forma que o foco se manteve nos preços baseados na última negociação (*last trade*).
### Slide 6: Resultado Principal #1 (Acurácia Preditiva)
 * **Aderência Institucional (SME):** Para as previsões da taxa de *Fed Funds* com 150 dias de antecedência (3 reuniões do FOMC), o erro médio absoluto da Kalshi é muito semelhante ao dos analistas profissionais da Pesquisa de Expectativas de Mercado do FRBNY.
 * **Superando os Futuros:** A mediana e a moda da Kalshi possuem um histórico de previsão perfeita no dia anterior ao FOMC, o que representa uma melhoria estatisticamente significativa em relação à previsão baseada nos futuros de *Fed Funds*.
 * **Headline CPI:** Para o CPI cheio, a Kalshi provê uma melhoria estatisticamente significativa em relação à previsão de consenso da Bloomberg.
 * **Testes de Calibração (PIT):** Transformadas Integrais de Probabilidade sugerem que as PDFs são razoavelmente bem calibradas, embora rejeições limítrofes ocorram pelo fato de que baixos valores de inflação e desemprego ocorrem com um pouco de excesso de frequência.
### Slide 7: Resultado Principal #2 (Assimetrias e Dinâmica Intraday)
 * **Reação Assimétrica à Inflação:** A média da distribuição da taxa de *Fed Funds* reage com uma magnitude quatro vezes maior a choques positivos no CPI do que a choques negativos.
 * **Efeito "Resolução de Incerteza":** A variância da distribuição declina de forma mais acentuada quando o indicador macro divulgado atende perfeitamente às expectativas (surpresa zero).
 * **Choques de Comunicação (Press Conference):** Surpresas durante a coletiva de imprensa do Fed não afetam substancialmente a tendência central (média, mediana ou moda), mas causam um declínio agudo e significativo na assimetria (*skewness*) da distribuição. Isso implica que o discurso restritivo resolve a incerteza de alta, efetivamente truncando a "cauda direita" da distribuição de juros.
### Slide 8: Evidências Visuais (Vantagem Distribucional)
 * **Restrições dos Futuros de Fed Funds:** Futuros de *Fed Funds* exigem suposições de árvore binomial que impõem estritamente dois resultados possíveis. Em momentos de alta incerteza, isso implica em uma subestimação severa da variância do mercado.
 * **O Problema das Opções de SOFR:** Opções atreladas à SOFR apresentam um viés de alta na distribuição. A SOFR liquida sob taxas de recompra (*repo rate*), existindo um *spread* variável de cerca de 6 pontos base em relação à taxa efetiva dos *Fed Funds*, limitando a acurácia dessas probabilidades.
 * **Vantagem Estrutural Kalshi:** Por ser diretamente atrelada à taxa alvo dos *Fed Funds*, a distribuição da plataforma não sofre com restrições binomiais nem problemas de base (*basis*), entregando a melhor precisão disponível para expectativas de curto prazo.
### Slide 9: Precificando Riscos de Cauda (*Stagflation*)
 * **Lacuna Preenchida:** O artigo destaca a Kalshi como a única fonte de distribuições em tempo real para o crescimento do PIB e previsões contínuas para desemprego e folha de pagamentos.
 * **Riscos Bi-dimensionais:** A observação em alta frequência revelou elevação rápida no peso das apostas para inflação acima de 3,5% e crescimento do PIB abaixo de 1% em meados de 2025.
 * **Estagflação Severa:** Modelagens de caudas extremas (ex: CPI > 4% e PIB < 0%) exibiram um peso probabilístico na Kalshi substancialmente maior do que em pesquisas fechadas (como o *Survey of Professional Forecasters*).
### Slide 10: Implicações Práticas e de Política Monetária
 * **Monitoramento Real-Time:** Os mercados de previsão oferecem um *check* quase instantâneo sobre a eficácia da comunicação dos Bancos Centrais e de como absorvem dados econômicos.
 * **Distribuição vs. Ponto:** Permite a incorporação formal de assimetrias e riscos de cauda na modelagem de alocação institucional e formulação de políticas, informações que são perdidas em estimativas modais de pesquisas de mercado.
 * **O Sinal do Varejo:** Oferece uma lente pura sobre as expectativas formadas independentemente de fortes restrições de portfólio ou motivações mecânicas de *hedge* (*fixed income exposure*) que dominam *players* institucionais e distorcem prêmios no mercado de juros tradicional.
### Slide 11: Limitações e *Caveats*
 * **Medida Q vs. Medida P:** Como quaisquer opções, as probabilidades implícitas na Kalshi são neutras ao risco (medida Q) e não devem ser estritamente confundidas com probabilidades físicas do mundo real (medida P).
 * **Prêmio de Risco Varejista:** As probabilidades refletem prêmios de risco, e a composição maciça de base de investidores de varejo pode gerar propriedades idiossincráticas ou anomalias nesse prêmio de risco que não existem no interbancário.
 * **Ilidez nas Extremos:** Contratos nas caudas (eventos extremos de baixa probabilidade) frequentemente sofrem com baixo volume, gerando preços obsoletos (*stale prices*) e estimativas ruidosas na distribuição.
### Slide 12: Conclusão
 * A Kalshi oferece um *benchmark* de mercado contínuo, empiricamente rico em momentos distributivos, para pesquisadores e *policymakers*.
 * Atua de maneira superior em relação a certos instrumentos tradicionais, demonstrando erros de previsão altamente competitivos e oferecendo a única lente ativa de probabilidades associadas a divulgações macroeconômicas centrais.
 * Representa uma nova e indispensável fronteira na identificação de transmissão de choques, volatilidade implícita de variáveis de estado e sentimento de mercado de alta frequência.
Gostaria de que eu detalhasse a matemática exata por trás da imposição de monotonicidade na CDF, ou que formulasse um slide extra cobrindo as equações das regressões de estudo de evento aplicadas aos choques de política monetária?