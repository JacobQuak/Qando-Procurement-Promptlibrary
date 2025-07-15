# Inkoop Prompt Library

> **Doel & doelgroep**  
> Deze bibliotheek helpt inkoopprofessionals — van tactisch buyer tot CPO — om Large‑Language‑Models (LLM's) efficiënt toe te passen binnen het volledige inkoopproces. Vul alle `[placeholders]` vóór gebruik aan met jouw eigen context.

---

## 1 Prompt‑technieken (uitgebreid)

### 1.1 Kerntechnieken en waarom ze werken

* **Role‑Based Prompting** – Activeert gespecialiseerde domeinkennis zodra je de rol expliciet benoemt.  
  *Quick‑syntax:* `Je bent een [rol] …`
* **Polite Formulation** – Beleefde prompts geven ± 45 % betere coherentie.  
  *Quick‑syntax:* `…, alsjeblieft.`
* **Few‑Shot Examples** – Voorbeelden leren het model on‑the‑fly structuur & tone‑of‑voice.  
  *Quick‑syntax:* `Voorbeeld 1 …`
* **Placeholders** – Houd prompts herbruikbaar: `[productcategorie]`, `[leverancier]`, …
* **Chain‑of‑Thought (CoT)** – Stap‑voor‑stap redeneren vermindert hallucinatierisico.
* **Tree‑of‑Thought (ToT)** – Parallelle scenario's leveren breder perspectief.
* **Meta‑Prompting** – Het model voert een zelf‑check uit op eigen output.
* **Self‑Correction** – Eén prompt bevat draft → kritiek → revisie.
* **Analogical Prompting** – Leert van vergelijkbare cases uit andere sectoren.

---

## 2 Basis Prompt‑Packs per Inkooponderwerp

> Gebruik deze snelle, laagdrempelige prompts voor initiële analyses en beslissings­ondersteuning.

### 2.1 Leveranciersselectie

#### 1. Scorecard Ontwikkelaar
**Doel:** Bouw een gewogen leveranciers‑scorecard met criteriapunten.

**Voorbeeldprompts:**
```
Je bent een ervaren sourcing specialist. Ontwikkel een leveranciers-scorecard voor [productcategorie] met 8-10 evaluatiecriteria. Geef elk criterium een gewicht (totaal 100%) en definieer een 5-punts beoordelingsschaal. Voeg bij elk criterium praktische sub-vragen toe die een buyer kan gebruiken tijdens leveranciersgesprekken.
```

```
Creëer een scorecard-template voor het selecteren van [type leverancier] voor onze [industrie]. Includeer zowel harde criteria (prijs, kwaliteit, levertijd) als zachte criteria (innovatie, duurzaamheid, cultuur-fit). Zorg dat het totaal overzichtelijk blijft op maximaal 2 pagina's.
```

```
Ontwikkel een dynamische leveranciers-scorecard waarin criteria automatisch zwaarder wegen naarmate [specifieke business requirements] belangrijker worden. Maak onderscheid tussen must-haves en nice-to-haves, en voeg een risico-component toe.
```

#### 2. Audit‑Checklist Maker
**Doel:** Ontwikkel een ISO‑gebaseerde audit‑checklist.

**Voorbeeldprompts:**
```
Je bent een kwaliteitsauditor met 15 jaar ervaring. Maak een uitgebreide audit-checklist voor [leverancier type] gebaseerd op ISO 9001:2015 standaarden. Groepeer vragen per proces (management, productie, kwaliteitscontrole) en geef elke vraag een risico-score van 1-5.
```

```
Ontwikkel een pre-audit questionnaire voor [specifieke industrie] leveranciers. Focus op compliance, financiële stabiliteit, operationele capaciteit en ESG-aspecten. Maak het praktisch bruikbaar voor remote assessment voorafgaand aan een fysieke audit.
```

```
Creëer een audit-checklist die zowel geschikt is voor eerste leveranciers-kwalificatie als voor periodieke herbeoordelingen. Includeer specifieke aandachtspunten voor [productcategorie] en geef duidelijke go/no-go criteria per sectie.
```

#### 3. RFQ‑Template Architect
**Doel:** Genereer een gestandaardiseerd RFQ‑document.

**Voorbeeldprompts:**
```
Je bent een strategic sourcing manager. Ontwerp een professionele RFQ-template voor [productcategorie] inkoop. Includeer alle benodigde secties: company background, product specifications, commercial terms, evaluation criteria, timeline, en legal requirements. Zorg voor een heldere structuur die leveranciers gemakkelijk kunnen volgen.
```

```
Maak een RFQ-template specifiek voor [service type] met focus op performance indicators, SLA's, en prijsstructuur. Voeg een section toe voor leveranciers om hun toegevoegde waarde en differentiatie te beschrijven. Includeer een evaluatiematrix die we kunnen gebruiken voor objectieve vergelijking.
```

```
Ontwikkel een modulaire RFQ-template die we kunnen aanpassen voor verschillende productcategorieën. Maak standaard-secties voor algemene terms en aanpasbare secties voor product-specifieke requirements. Voeg een checklist toe voor buyers om te controleren of alle relevante punten zijn opgenomen.
```

### 2.2 Onderhandeling

#### 1. Win‑Win Scenario Creator
**Doel:** Bepaal gedeelde waarden en compromisruimtes.

**Voorbeeldprompts:**
```
Je bent een ervaren onderhandelaar. Analyseer de onderhandelingspositie met [leverancier] voor [product/service]. Identificeer 5 potentiële win-win scenario's waarin beide partijen voordeel behalen. Geef per scenario concrete voorbeelden van wat wij bieden versus wat zij bieden, en schat de waarde voor beide partijen in.
```

```
Ontwikkel een value-creation matrix voor onze onderhandeling met [leverancier naam]. Map alle mogelijke concessies (prijs, volumes, contractduur, betalingsvoorwaarden, exclusiviteit) tegen hun strategische waarde voor beide partijen. Identificeer de beste trade-offs die tot een optimaal resultaat leiden.
```

```
Creëer een onderhandelingsstrategie die verder kijkt dan alleen prijs. Analyseer hoe we [specifieke business needs] kunnen koppelen aan [leverancier capabilities] voor wederzijds voordeel. Geef concrete voorbeelden van non-monetary benefits die waardevol zijn voor beide partijen.
```

#### 2. Onderhandelings­Roadmap Builder
**Doel:** Stel een stappenplan inclusief BATNA op.

**Voorbeeldprompts:**
```
Je bent een strategic sourcing expert. Bouw een complete onderhandelingsroadmap voor [specifieke deal]. Start met stakeholder-mapping, definieer onze BATNA, stel een opening-stance op, en creëer een stap-voor-stap plan met timing, agenda-punten, en fall-back posities voor elke onderhandelingsronde.
```

```
Ontwikkel een gestructureerd stappenplan voor een multi-stakeholder onderhandeling met [leverancier]. Includeer pre-meeting preparation, opening statements, issue-by-issue aanpak, en closing strategy. Geef per stap concrete talking points en mogelijke leveranciers-reacties met onze responses.
```

```
Maak een onderhandelings-playbook voor [type contract] heronderhandelingen. Analyseer onze huidige positie, market alternatives, en set realistic targets. Ontwikkel een timing-strategy en identificeer de optimale momenten voor pressure en voor concessies.
```

#### 3. Concession Trade‑Off Planner
**Doel:** Visualiseer concessies versus tegenprestaties.

**Voorbeeldprompts:**
```
Je bent een ervaren commercial manager. Maak een concessie-matrix voor onze onderhandeling met [leverancier]. List alle mogelijke concessies die wij kunnen doen (betaling, volumes, contractduur, etc.) en map deze tegen mogelijke tegenprestaties. Geef elke trade-off een waarde-score en prioriteit.
```

```
Ontwikkel een trade-off calculator voor [specifieke onderhandeling]. Kwantificeer de financiële impact van onze mogelijke concessies versus de waarde van hun tegenprestaties. Includeer zowel directe kosten als indirecte voordelen, en geef een net present value berekening.
```

```
Creëer een concessie-planning tool waarin we verschillende scenario's kunnen doorrekenen. Voor elke mogelijke concessie van onze kant, definieer de minimum acceptable tegenprestatie. Maak dit visueel met een dashboard dat real-time de impact toont van verschillende combinaties.
```

### 2.3 Marktanalyse

#### 1. Markttrend Analist
**Doel:** Analyseer prijstrends en voorspel 12 maanden vooruit.

**Voorbeeldprompts:**
```
Je bent een marktanalist gespecialiseerd in [productcategorie]. Analyseer de huidige markttrends, prijsontwikkelingen, en supply-demand dynamics. Geef een forecast voor de komende 12 maanden met kwartaal-targets, en identificeer de top 5 risk factors die onze prijsprognose kunnen beïnvloeden.
```

```
Ontwikkel een marktanalyse voor [specifieke commodity/product] met focus op seizoenspatronen, geografische verschillen, en macro-economische drivers. Includeer een sensitivity analysis die toont hoe verschillende scenario's (inflatie, supply chain disruption, demand changes) onze costs beïnvloeden.
```

```
Maak een comprehensive market intelligence report voor [industrie sector]. Analyseer competitor strategies, nieuwe market entrants, technologische developments, en regulatory changes. Geef actionable insights over hoe we onze sourcing strategy kunnen aanpassen aan deze trends.
```

#### 2. Concurrentie Intelligence Expert
**Doel:** Benchmark inkoopstrategieën van concurrenten.

**Voorbeeldprompts:**
```
Je bent een competitive intelligence specialist. Analyseer de inkoopstrategieën van onze top 3 concurrenten in [industrie]. Onderzoek hun leveranciers-portfolio, contract-strategieën, en cost-optimization approaches. Identificeer best practices die we kunnen adopteren en competitive advantages die we kunnen uitbuiten.
```

```
Ontwikkel een benchmark-analyse van hoe [competitors] omgaan met [specifiek inkoopchallenge]. Vergelijk hun supplier relationship management, risk mitigation strategies, en innovation partnerships. Geef concrete recommendations voor hoe we onze approach kunnen verbeteren.
```

```
Creëer een competitive sourcing analysis voor [product category]. Map de supplier-bases van key competitors, analyseer hun pricing strategies, en identificeer market gaps of opportunities. Includeer een SWOT-analyse van onze positie versus competitors.
```

#### 3. Prijs‑Forecast Generator
**Doel:** Maak een eenvoudige prijsforecast op basis van historische data.

**Voorbeeldprompts:**
```
Je bent een pricing analyst. Gebaseerd op [historische data periode], maak een prijsforecast voor [product/service] voor de komende 6 maanden. Gebruik zowel quantitative analysis als qualitative factors. Geef confidence intervals en identificeer key assumptions die de forecast kunnen beïnvloeden.
```

```
Ontwikkel een pricing model voor [commodity/product] dat rekening houdt met seasonality, economic indicators, en supply chain factors. Maak scenario-analyses voor best case, worst case, en most likely case. Geef monthly price targets met actionable buying recommendations.
```

```
Creëer een price forecasting tool dat we kunnen gebruiken voor budget planning en contract negotiations. Includeer historical trend analysis, leading indicators, en market sentiment. Maak het simpel genoeg voor category managers om zelf te gebruiken, maar robuust genoeg voor strategic decisions.
```

### 2.4 Contractevaluatie

#### 1. Contract Risk Assessor
**Doel:** Identificeer en prioriteer contractrisico's.

**Voorbeeldprompts:**
```
Je bent een contract risk specialist. Analyseer het contract met [leverancier] voor [product/service] en identificeer alle potentiële risico's. Categoriseer deze in financiële, operationele, legal, en reputatie risico's. Geef elk risico een probability/impact score en prioriteer de top 10 die immediate attention nodig hebben.
```

```
Ontwikkel een contract risk matrix voor [type contract]. Evalueer clausules rond liability, force majeure, intellectual property, termination, en performance guarantees. Voor elk geïdentificeerd risico, geef mitigation strategies en suggested contract amendments.
```

```
Maak een comprehensive risk assessment voor ons [multi-year/strategic] contract met [leverancier]. Analyseer zowel commercial risks als compliance risks. Includeer een risk monitoring plan met KPI's en trigger points voor contract reviews of renegotiations.
```

#### 2. SLA Benchmark Specialist
**Doel:** Vergelijk SLA's met industriestandaarden.

**Voorbeeldprompts:**
```
Je bent een SLA benchmarking expert. Vergelijk onze huidige SLA's met [leverancier] tegen industry best practices voor [service type]. Analyseer performance metrics, penalty structures, en incentive mechanisms. Identificeer gaps en opportunities voor improvement in onze volgende contract negotiation.
```

```
Ontwikkel een SLA benchmarking framework voor [industrie sector]. Definieer key performance indicators, acceptable performance ranges, en escalation procedures. Vergelijk dit met what competitors typically achieve en geef recommendations voor realistic maar ambitieuze targets.
```

```
Creëer een SLA optimization plan voor onze [service contracts]. Analyseer current performance data, identify improvement opportunities, en design nieuwe SLA structures die better alignment creëren tussen onze business needs en supplier capabilities.
```

#### 3. Clause Improvement Suggestor
**Doel:** Herformuleer risicovolle clausules op een beleefde manier.

**Voorbeeldprompts:**
```
Je bent een contract negotiation specialist. Herformuleer de volgende risicovolle clausules uit ons contract met [leverancier] op een professionele en constructieve manier: [specificeer clausules]. Geef voor elke clausule de original text, identified risks, en improved language die acceptable is voor beide partijen.
```

```
Ontwikkel diplomatieke language voor het aanpassen van [specific problematic clauses] in onze contract negotiations. Focus op win-win formulations die onze concerns addresseren zonder de leverancier te alieneren. Includeer rationale die we kunnen gebruiken tijdens discussions.
```

```
Maak een clausule improvement toolkit voor veel voorkomende contract issues in [industrie]. Voor elke problematic clause type, geef standard improved language, implementation suggestions, en talking points voor smooth negotiations met leveranciers.
```

### 2.5 Kostenbesparing

#### 1. Value Engineering Expert
**Doel:** Vind technische kostenreducties zonder kwaliteitsverlies.

**Voorbeeldprompts:**
```
Je bent een value engineering specialist. Analyseer [product/service] en identificeer 10 concrete opportunities voor cost reduction zonder kwaliteitsverlies. Voor elke opportunity, geef technical feasibility, estimated savings, implementation timeline, en potential risks. Prioriteer op basis van impact en ease of implementation.
```

```
Ontwikkel een value engineering workshop plan voor [productcategorie]. Definieer de methodology, required stakeholders, en structured approach om samen met [leverancier] cost optimization opportunities te identificeren. Includeer templates voor idea evaluation en business case development.
```

```
Creëer een systematic value analysis voor onze [high-spend category]. Break down de cost structure, identify non-value-adding elements, en develop alternatives. Geef een roadmap voor implementation inclusief stakeholder buy-in strategies en risk mitigation plans.
```

#### 2. TCO Optimization Specialist
**Doel:** Breng verborgen kosten in kaart.

**Voorbeeldprompts:**
```
Je bent een TCO specialist. Ontwikkel een complete total cost of ownership analyse voor [product/service category]. Identificeer alle direkte en indirekte kosten over de gehele lifecycle: acquisition, operation, maintenance, training, disposal. Geef een TCO model dat we kunnen gebruiken voor supplier comparisons.
```

```
Maak een TCO optimization plan voor onze [current major purchase]. Analyseer hidden costs zoals inventory carrying costs, quality costs, administrative burden, en opportunity costs. Quantificeer deze en geef actionable recommendations voor cost reduction.
```

```
Ontwikkel een TCO calculator tool voor [department/category] dat category managers kunnen gebruiken voor informed decision making. Maak het user-friendly maar comprehensive, en includeer sensitivity analysis voor key variables. Geef guidance over wanneer TCO analysis meer important is dan initial price.
```

#### 3. Volume Consolidation Planner
**Doel:** Bundel volumes en bereken schaalvoordeel.

**Voorbeeldprompts:**
```
Je bent een strategic sourcing manager. Analyseer onze huidige spend in [productcategorie] over alle business units/locaties. Identificeer consolidation opportunities, bereken potential savings door volume bundeling, en ontwikkel een implementation roadmap. Addresseer ook potential risks van consolidation.
```

```
Ontwikkel een volume consolidation strategy voor [meerdere gerelateerde categorieën]. Analyseer supplier capabilities, identify preferred suppliers die multiple categories kunnen bedienen, en create a phased approach voor consolidation. Includeer stakeholder management plan voor smooth transition.
```

```
Creëer een consolidation business case voor [specific opportunity]. Quantificeer savings potential, implementation costs, en payback period. Analyseer impact op supplier relationships, internal stakeholders, en operational efficiency. Geef een risk-adjusted NPV calculation.
```

### 2.6 Risicoanalyse

#### 1. Supply Chain Risk Analyst
**Doel:** Bouw een risicomatrix met mitigatieplan.

**Voorbeeldprompts:**
```
Je bent een supply chain risk specialist. Ontwikkel een comprehensive risk matrix voor onze [productcategorie] supply chain. Identificeer alle mogelijke risico's (geopolitical, natural disasters, supplier financial issues, quality problems, etc.), geef elk een probability/impact score, en ontwikkel detailed mitigation strategies voor high-priority risks.
```

```
Maak een supply chain resilience assessment voor onze [critical supplier/category]. Analyseer single points of failure, supplier dependencies, geographic concentrations, en alternative sources. Ontwikkel een risk monitoring dashboard met early warning indicators en response protocols.
```

```
Creëer een crisis management plan voor [specific supply chain scenario]. Definieer roles & responsibilities, communication protocols, alternative sourcing strategies, en recovery procedures. Maak het actionable met concrete steps, timelines, en escalation procedures.
```

#### 2. Financial Stability Assessor
**Doel:** Monitor de financiële gezondheid van leveranciers.

**Voorbeeldprompts:**
```
Je bent een financial analyst gespecialiseerd in supplier assessment. Ontwikkel een financial health monitoring system voor onze [critical suppliers]. Definieer key financial ratios, warning indicators, en assessment frequency. Creëer een scoring model die we kunnen gebruiken voor ongoing monitoring en early intervention.
```

```
Analyseer de financiële stabiliteit van [specifieke leverancier] gebaseerd op hun financial statements, market position, en industry trends. Identificeer red flags, assess creditworthiness, en geef recommendations voor risk mitigation (guarantees, payment terms, alternative suppliers).
```

```
Maak een financial due diligence checklist voor nieuwe supplier onboarding. Includeer required financial documents, ratio analysis, external credit checks, en assessment criteria. Geef guidance over hoe financial risks te weighen tegen commercial benefits.
```

#### 3. Compliance Checklist Generator
**Doel:** Maak een checklist voor wet‑ & regelgeving.

**Voorbeeldprompts:**
```
Je bent een compliance specialist. Ontwikkel een comprehensive compliance checklist voor [industrie/productcategorie] suppliers. Includeer alle relevante regulations (safety, environmental, labor, data privacy, etc.), required certifications, audit requirements, en monitoring procedures. Maak het praktisch bruikbaar voor supplier management teams.
```

```
Creëer een regulatory compliance matrix voor onze [international/multi-location] supply chain. Map alle applicable regulations per country/region, identify compliance gaps, en ontwikkel remediation plans. Includeer ongoing monitoring requirements en update procedures.
```

```
Ontwikkel een compliance risk assessment tool voor [specific regulation/standard]. Definieer assessment criteria, scoring methodology, en reporting format. Maak het geschikt voor zowel initial supplier qualification als periodic compliance reviews.
```

---

## 3 Advanced Prompt‑Packs (alle inkooponderwerpen)

> Pas deze prompts toe zodra de basisinformatie beschikbaar is en je diepere analyse of zelf‑validatie wilt.

### 3.1 Leveranciersselectie (Advanced)

#### A1 CoT Leveranciers‑Evaluator
**Doel:** Stap‑voor‑stap analyse van marktcontext tot aanbeveling.

**Voorbeeldprompts:**
```
Je bent een senior sourcing strategist. Voer een Chain-of-Thought analyse uit voor leveranciersselectie in [productcategorie]. Stap 1: Analyseer de marktcontext en competitive landscape. Stap 2: Definieer onze business requirements en success criteria. Stap 3: Evalueer elke leverancier tegen deze criteria. Stap 4: Weeg strategic fit versus operational performance. Stap 5: Geef een onderbouwde aanbeveling met rationale voor elke beslissing.
```

```
Ontwikkel een systematic evaluation methodology voor [complex sourcing decision]. Walk through each step: market research → supplier identification → RFI process → detailed evaluation → risk assessment → strategic alignment → final recommendation. Voor elke stap, documenteer je reasoning, assumptions, en trade-offs.
```

```
Creëer een leverancier-evaluatie framework dat expliciete reasoning toont voor elke beslissing. Start met business context, define evaluation criteria, assess each supplier systematically, consider long-term implications, en arrive at a recommendation. Maak je thought process transparent en challengeable.
```

#### A2 ToT Leveranciers‑Strategist
**Doel:** Parallelle scenario's (kosten, kwaliteit, innovatie, risico).

**Voorbeeldprompts:**
```
Je bent een strategic sourcing expert. Ontwikkel vier parallelle sourcing scenarios voor [productcategorie]: 1) Cost-optimization focus, 2) Quality-excellence focus, 3) Innovation-partnership focus, 4) Risk-minimization focus. Voor elk scenario, definieer de optimal supplier mix, commercial strategy, en expected outcomes. Synthesize deze tot een balanced recommendation.
```

```
Maak een Tree-of-Thought analysis voor onze [strategic sourcing decision]. Exploreer verschillende paths: single vs. multiple sourcing, local vs. global suppliers, established vs. emerging suppliers, en long-term vs. short-term contracts. Evalueer elke path op business impact, risk, en strategic alignment.
```

```
Ontwikkel een scenario-based sourcing strategy voor [product/service]. Consider verschillende toekomst-scenarios (economic downturn, supply shortages, technology disruption, regulatory changes) en design flexible sourcing approaches die optimal performance geven in elk scenario. Integrate deze tot een resilient overall strategy.
```

#### A3 Meta‑Optimized RFQ‑Generator
**Doel:** Draft RFQ → zelf‑check → verbeterde versie.

**Voorbeeldprompts:**
```
Je bent een procurement excellence specialist. Maak eerst een draft RFQ voor [product/service]. Daarna voer je een kritische self-assessment uit: zijn alle requirements duidelijk? Is de evaluation methodology fair? Zijn timelines realistic? Zijn legal terms balanced? Genereer vervolgens een improved version die deze issues addresseert.
```

```
Ontwikkel een RFQ voor [complex purchase] met built-in self-correction. Stap 1: Create initial draft. Stap 2: Review from supplier perspective - is het duidelijk en fair? Stap 3: Review from internal stakeholder perspective - worden alle needs geaddresseerd? Stap 4: Optimize voor best response quality. Stap 5: Finalize improved version.
```

```
Creëer een meta-optimized RFQ process voor [category]. Generate initial RFQ, then systematically review en improve: clarity of requirements, fairness of evaluation, completeness of commercial terms, realism of timelines, en quality of supplier experience. Iterate until optimal.
```

### 3.2 Onderhandeling (Advanced)

#### B1 Analogical Negotiation Strategist
**Doel:** Trek lessen uit drie vergelijkbare deals.

**Voorbeeldprompts:**
```
Je bent een negotiation expert met toegang tot deal databases. Analyseer drie vergelijkbare onderhandelingen in [industrie/productcategorie]: één zeer succesvolle, één gemiddelde, en één problematische. Identificeer success factors, failure points, en best practices. Pas deze lessen toe op onze huidige onderhandeling met [leverancier] voor [product/service].
```

```
Ontwikkel een negotiation strategy gebaseerd op analogical learning. Bestudeer hoe andere companies in [vergelijkbare situatie] hebben onderhandeld. Wat waren hun opening positions, concession patterns, en final outcomes? Welke tactics werkten well en welke backfired? Adapt deze insights voor onze specifieke context.
```

```
Creëer een lessons-learned framework voor onze [upcoming negotiation]. Analyseer case studies van succesvolle deals in similar circumstances. Identify common patterns in supplier behavior, effective negotiation techniques, en value creation opportunities. Develop actionable strategies gebaseerd op these analogies.
```

#### B2 Self‑Correcting Negotiation Planner
**Doel:** Strategie met ingebouwde risico‑ en stakeholder‑check.

**Voorbeeldprompts:**
```
Je bent een senior negotiation strategist. Ontwikkel een negotiation plan voor [deal], daarna voer je een self-check uit: Zijn onze positions realistic? Hebben we alle stakeholders geïnformeerd? Zijn risico's adequaat geaddresseerd? Is de timeline feasible? Adjust je strategy based op deze analysis en create een robust final plan.
```

```
Maak een negotiation strategy voor [complex deal] met built-in validation. Stap 1: Develop initial approach. Stap 2: Stress-test tegen mogelijke supplier responses. Stap 3: Validate met internal stakeholders. Stap 4: Assess regulatory/legal implications. Stap 5: Refine strategy. Stap 6: Create contingency plans.
```

```
Ontwikkel een self-correcting negotiation framework. Start met je preferred strategy, then systematically challenge elke assumption: Are we being too aggressive? Too conservative? Are we missing win-win opportunities? Do we have adequate alternatives? Iterate tot een balanced, defensible approach.
```

#### B3 Dynamic BATNA Optimizer
**Doel:** Genereer en kwantificeer alternatieve BATNA's.

**Voorbeeldprompts:**
```
Je bent een strategic sourcing expert. Ontwikkel meerdere BATNA's voor onze onderhandeling met [leverancier]: 1) Alternative suppliers, 2) In-house production, 3) Substitute products, 4) Delayed purchase, 5) Modified requirements. Kwantificeer elk alternatief (costs, timeline, risks, capabilities) en rank ze. Use dit voor optimal negotiation positioning.
```

```
Creëer een dynamic BATNA optimization system voor [ongoing negotiation]. Continuously evaluate onze alternatives als market conditions change, nieuwe suppliers emerge, of internal priorities shift. Develop een framework voor real-time BATNA assessment en strategic adjustment.
```

```
Ontwikkel een comprehensive alternatives analysis voor [strategic deal]. Beyond obvious alternatives, exploreer creative options: partnerships, joint ventures, technology solutions, process changes, of market repositioning. Quantify each option en create een decision tree die onze negotiation power maximizes.
```

### 3.3 Marktanalyse (Advanced)

#### C1 CoT Market Intelligence
**Doel:** Vier logische stappen: structuur → drivers → trends → projectie.

**Voorbeeldprompts:**
```
Je bent een market intelligence specialist. Voer een Chain-of-Thought analyse uit voor [productcategorie] market. Stap 1: Map de market structure (players, relationships, value chain). Stap 2: Identify key drivers (economic, technological, regulatory, social). Stap 3: Analyze current trends en emerging patterns. Stap 4: Project future scenarios met actionable implications voor onze sourcing strategy.
```

```
Ontwikkel een systematic market analysis voor [industrie sector]. Walk through: market segmentation → competitive dynamics → supply/demand analysis → price formation mechanisms → trend identification → scenario development → strategic implications. Maak elk step logical en verifiable.
```

```
Creëer een structured market intelligence framework. Start met market fundamentals, analyze driving forces, identify trend patterns, project future developments, en translate insights into procurement recommendations. Ensure each step builds logically op de previous one.
```

#### C2 ToT Competitive Intelligence
**Doel:** Parallelle markt‑scans & integratie.

**Voorbeeldprompts:**
```
Je bent een competitive intelligence expert. Voer parallelle analyses uit vanuit vier perspectieven: 1) Supplier perspective (their strategies, capabilities, challenges), 2) Customer perspective (market demands, trends, alternatives), 3) Competitor perspective (their sourcing strategies, supplier relationships), 4) Technology perspective (innovations, disruptions, opportunities). Synthesize these views into comprehensive market intelligence.
```

```
Ontwikkel een multi-dimensional market scan voor [productcategorie]. Simultaneously analyze: market structure, competitive dynamics, supplier landscape, technology trends, regulatory environment, en customer behavior. Integrate deze perspectives into actionable intelligence voor strategic sourcing decisions.
```

```
Creëer een comprehensive competitive intelligence system using Tree-of-Thought methodology. Explore different analytical paths: quantitative analysis, qualitative insights, trend analysis, scenario planning, en strategic implications. Combine these approaches for complete market understanding.
```

#### C3 Scenario‑Driven Forecast Synthesizer
**Doel:** Drie scenario's met risico‑hitlist & triggers.

**Voorbeeldprompts:**
```
Je bent een scenario planning expert. Ontwikkel drie distinct scenarios voor [market/productcategorie]: 1) Optimistic scenario, 2) Base case scenario, 3) Pessimistic scenario. Voor elk scenario, define key assumptions, price impacts, supply availability, en procurement implications. Create een risk hitlist met early warning indicators en trigger points voor scenario transitions.
```

```
Maak een scenario-based forecasting system voor [commodity/product]. Develop plausible future scenarios based op verschillende combinations van key variables. Voor elk scenario, quantify impact op costs, availability, en supplier relationships. Create monitoring dashboards met leading indicators.
```

```
Ontwikkel een dynamic scenario planning framework. Start met baseline forecast, then create alternative scenarios based op different assumptions about market drivers. Integrate these into een probabilistic forecast met confidence intervals. Include risk assessment en mitigation strategies voor each scenario.
```

### 3.4 Contractevaluatie (Advanced)

#### D1 Analogical Contract Risk Assessor
**Doel:** Leer van succesvolle en problematische contracten.

**Voorbeeldprompts:**
```
Je bent een contract risk specialist met toegang tot contract databases. Analyseer drie vergelijkbare contracten: één die excellent performance leverde, één met gemiddelde resultaten, en één met significante problemen. Identificeer de contractclausules, risk allocation, en governance structures die het verschil maakten. Pas deze lessen toe op onze nieuwe [type contract] met [leverancier].
```

```
Ontwikkel een contract risk assessment gebaseerd op analogical learning. Bestudeer hoe vergelijkbare deals in [industrie] zijn gestructureerd. Welke risk allocation patterns werkten well? Welke clausules veroorzaakten disputes? Welke governance mechanisms waren effectief? Integreer deze insights in onze contract strategy.
```

```
Creëer een lessons-learned framework voor contract risk management. Analyseer case studies van contracten met similar scope, complexity, en risk profile. Identify common failure modes, successful risk mitigation strategies, en best practices voor contract structuring. Develop actionable recommendations voor onze [upcoming contract].
```

#### D2 Self‑Correcting SLA Optimizer
**Doel:** Iteratieve verbetering met benchmark‑ en stakeholder‑checks.

**Voorbeeldprompts:**
```
Je bent een SLA optimization expert. Ontwikkel eerst een draft SLA structure voor [service type], daarna voer je een multi-perspective review uit: 1) Supplier feasibility check, 2) Business stakeholder validation, 3) Industry benchmark comparison, 4) Legal/compliance review, 5) Performance measurement practicality. Itereer tot een optimized SLA structure.
```

```
Maak een self-correcting SLA framework voor [service category]. Stap 1: Define initial performance metrics. Stap 2: Stress-test against operational realities. Stap 3: Validate with service recipients. Stap 4: Benchmark against industry standards. Stap 5: Optimize voor balanced performance incentives. Stap 6: Create monitoring and adjustment mechanisms.
```

```
Ontwikkel een iterative SLA improvement process. Start met current SLA structure, systematically evaluate effectiveness, identify improvement opportunities, design enhanced metrics, validate with stakeholders, en implement changes. Include feedback loops voor continuous optimization.
```

#### D3 ML Clause Checker
**Doel:** Detecteer riskante patronen en valideer met zelf‑check.

**Voorbeeldprompts:**
```
Je bent een contract analysis specialist met machine learning capabilities. Analyseer het [type contract] voor patterns die vaak leiden tot disputes of performance issues. Identificeer problematic language patterns, missing protective clauses, en unbalanced risk allocation. Voer daarna een self-validation uit: zijn mijn assessments accurate? Are recommendations practical? Geef een final optimized contract structure.
```

```
Ontwikkel een systematic contract clause analysis voor [contract type]. Scan for common risk patterns: ambiguous language, one-sided terms, inadequate protections, unrealistic commitments. Cross-reference tegen known problematic clauses from similar contracts. Validate findings en propose improvements.
```

```
Creëer een contract risk detection system met self-validation. Identify potentially problematic clauses based op pattern recognition, assess risk probability and impact, propose alternative language, validate recommendations against legal standards, en optimize for balanced risk allocation.
```

### 3.5 Kostenbesparing (Advanced)

#### E1 CoT Value Engineering
**Doel:** Functie‑analyse → kosten‑decompositie → alternatieven → business‑case.

**Voorbeeldprompts:**
```
Je bent een value engineering specialist. Voer een Chain-of-Thought analyse uit voor [product/service]. Stap 1: Decompose into functional elements. Stap 2: Analyze cost drivers voor each function. Stap 3: Generate alternative approaches voor each function. Stap 4: Evaluate alternatives on cost, quality, en risk. Stap 5: Develop business case voor recommended changes. Stap 6: Create implementation roadmap.
```

```
Ontwikkel een systematic value engineering methodology voor [high-cost item]. Walk through: functional analysis → cost breakdown → alternative identification → feasibility assessment → impact quantification → risk evaluation → implementation planning. Ensure each step builds logically op previous analysis.
```

```
Creëer een comprehensive value engineering framework. Start met understanding customer needs, decompose current solution, identify cost components, generate alternatives, evaluate options, develop business cases, en create implementation plans. Maak reasoning transparent en verifiable.
```

#### E2 Meta‑Optimized TCO Calculator
**Doel:** Verbeter TCO‑analyse met zelf‑kritiek en gevoeligheids­analyse.

**Voorbeeldprompts:**
```
Je bent een TCO specialist. Ontwikkel een comprehensive TCO model voor [product/service category], daarna voer je een self-critique uit: Are all cost elements included? Are assumptions realistic? Is the time horizon appropriate? Are indirect costs properly captured? Refine je model based op deze analysis en add sensitivity testing voor key variables.
```

```
Maak een meta-optimized TCO framework voor [purchase decision]. Stap 1: Build initial TCO model. Stap 2: Validate cost assumptions. Stap 3: Test model sensitivity. Stap 4: Benchmark against industry standards. Stap 5: Refine calculation methodology. Stap 6: Create decision support tools.
```

```
Ontwikkel een self-correcting TCO analysis system. Start met comprehensive cost identification, build calculation model, validate assumptions, test sensitivity to key variables, compare with benchmarks, identify improvement opportunities, en optimize for decision accuracy.
```

#### E3 Dynamic Cost Benchmark Builder
**Doel:** Real‑time benchmarks en scenario's.

**Voorbeeldprompts:**
```
Je bent een cost benchmarking expert. Ontwikkel een dynamic benchmarking system voor [product/service category] dat real-time market data integreert. Include multiple scenario analyses (volume changes, specification modifications, market shifts), create automated alerts voor significant cost movements, en develop actionable recommendations voor procurement strategy adjustments.
```

```
Creëer een adaptive cost benchmarking framework. Continuously monitor market prices, supplier costs, alternative solutions, en competitive positions. Develop scenario-based cost projections, identify cost optimization opportunities, en create dynamic procurement strategies that adapt to changing conditions.
```

```
Ontwikkel een comprehensive cost intelligence system. Integrate multiple data sources, create real-time benchmarks, develop predictive models, generate scenario analyses, en provide decision support voor procurement actions. Include automated monitoring en alerting voor significant changes.
```

### 3.6 Risicoanalyse (Advanced)

#### F1 ToT Risk Assessment
**Doel:** Parallelle scenario‑analyse met geïntegreerde mitigatie.

**Voorbeeldprompts:**
```
Je bent een risk assessment specialist. Voer een Tree-of-Thought analyse uit voor [supply chain/supplier] risks. Ontwikkel parallel scenarios: 1) Operational risks (capacity, quality, delivery), 2) Financial risks (stability, pricing, cashflow), 3) Strategic risks (alignment, dependency, alternatives), 4) External risks (market, regulatory, geopolitical). Integrate these analyses into comprehensive risk management strategy.
```

```
Ontwikkel een multi-dimensional risk assessment voor [critical supplier/category]. Simultaneously analyze different risk categories, assess interdependencies, develop mitigation strategies voor each dimension, create integrated response plans, en establish monitoring systems. Synthesize into holistic risk management approach.
```

```
Creëer een comprehensive risk evaluation framework using parallel analysis paths. Explore risks from multiple perspectives: probability/impact analysis, scenario planning, stress testing, en stakeholder assessment. Integrate findings into actionable risk management strategy.
```

#### F2 Analogical Supply Chain Resilience
**Doel:** Strategieën afleiden uit andere sectoren.

**Voorbeeldprompts:**
```
Je bent een supply chain resilience expert met cross-industry experience. Analyseer hoe andere sectoren [automotive, electronics, pharmaceuticals] hebben gedealt met vergelijkbare supply chain challenges. Identificeer successful resilience strategies, adaptation mechanisms, en recovery approaches. Pas deze lessen toe op onze [industrie/category] context.
```

```
Ontwikkel een resilience strategy gebaseerd op analogical learning. Bestudeer hoe companies in different industries hebben overcome supply chain disruptions. Wat waren hun preparation strategies, response mechanisms, en recovery approaches? Adapt these insights voor onze specific vulnerabilities en context.
```

```
Creëer een cross-industry resilience framework. Analyze successful supply chain transformations in andere sectoren, identify transferable strategies, assess applicability to our situation, en develop customized resilience solutions. Include implementation roadmap en success metrics.
```

#### F3 Stress‑Test Simulation Designer
**Doel:** Simuleer disrupties en toets mitigaties.

**Voorbeeldprompts:**
```
Je bent een supply chain simulation expert. Ontwikkel een comprehensive stress-test scenario voor onze [product/service category]. Simuleer verschillende disruptive events: natural disasters, geopolitical tensions, supplier failures, demand shocks, regulatory changes. Voor elk scenario, test onze current mitigation strategies, identify vulnerabilities, en develop improved response plans.
```

```
Maak een supply chain stress-testing framework voor [critical category]. Design realistic disruption scenarios, model impact on operations, test current contingency plans, identify failure points, develop enhanced mitigation strategies, en create improved response protocols. Include quantitative impact assessment.
```

```
Ontwikkel een dynamic supply chain simulation system. Create multiple stress scenarios, model cascade effects, test different response strategies, quantify business impacts, identify optimal mitigation approaches, en develop adaptive response capabilities. Include real-time monitoring en adjustment mechanisms.
```

---

## 4 Zo gebruik je deze bibliotheek

### 4.1 Stappenplan voor optimaal gebruik

1. **Begin met de Basis‑packs** voor snelle inzichten en eerste analyses
2. **Vul alle placeholders** (`[product]`, `[leverancier]`, `[industrie]`, etc.) vóór verzending
3. **Schakel over naar Advanced‑packs** voor diepte‑analyse, validatie, of complexe beslissingen
4. **Evalueer en itereer**: pas gewichten, voorbeelden of rolbeschrijvingen aan op basis van resultaten
5. **Integreer AI‑output** in bestaande tools (scorecards, contracten, BI‑dashboards)
6. **Onderhoud**: actualiseer voorbeelden elk kwartaal en deel best‑practices

### 4.2 Wanneer welke prompt te gebruiken

**Basis‑packs:** Ideaal voor dagelijkse procurement activiteiten, snelle analyses, en eerste verkenning van nieuwe onderwerpen.

**Advanced‑packs:** Gebruik voor strategische beslissingen, complexe situaties, validatie van belangrijke analyses, of wanneer je meerdere perspectieven nodig hebt.

**Combinatie‑strategie:** Begin met basis‑prompts voor foundation, gebruik advanced‑prompts voor verdieping, en combineer resultaten voor comprehensive insights.

---

## 5 Pro Tips voor Maximale Effectiviteit

### 5.1 Prompt‑optimalisatie
* **Combineer prompts** – Marktanalyse → Onderhandeling → Contractevaluatie levert een end‑to‑end sourcetraject
* **Parameter‑tuning** – Vraag om gevoeligheids‑analyses of alternatieve wegingsfactoren
* **Style‑transfer** – Laat het model schrijven "in de stijl van" je huisstijl of consultancy‑format
* **Structuur voor export** – Vraag output in CSV‑ of JSON‑vorm voor snelle import in BI‑tools

### 5.2 Kwaliteitscontrole
* **Valideer altijd** AI‑output met domeinexpertise en marktkennis
* **Cross‑check** belangrijke analyses met multiple prompts of approaches
* **Gebruik** advanced self‑correcting prompts voor kritische beslissingen
* **Documenteer** assumptions en limitations in alle AI‑gegenereerde analyses

### 5.3 Organisatie & Governance
* **Standaardiseer** prompt‑usage binnen teams voor consistente resultaten
* **Train** team members in effective prompt engineering techniques
* **Creëer** feedback loops voor continuous improvement van prompts
* **Etablish** governance voor AI‑supported procurement decisions

### 5.4 Integratie in Workflow
* **Embed** prompts in procurement tools en templates
* **Automate** routine analyses waar mogelijk
* **Customize** prompts voor specifieke product categories en suppliers
* **Scale** successful prompt patterns across de organisatie

---

## 6 Troubleshooting & Best Practices

### 6.1 Common Issues & Solutions

**Problem:** Generieke of oppervlakkige output  
**Solution:** Voeg meer context toe, gebruik specifieke voorbeelden, en definieer duidelijke output‑requirements

**Problem:** Inconsistente resultaten  
**Solution:** Standardize prompt formats, use consistent placeholders, en voeg role‑based context toe

**Problem:** Incomplete analyses  
**Solution:** Gebruik advanced CoT of ToT prompts, vraag explicit om completeness check, en combine multiple perspectives

### 6.2 Quality Assurance Checklist

- [ ] Alle placeholders correct ingevuld
- [ ] Role‑based context toegevoegd
- [ ] Specifieke output‑format requested
- [ ] Relevante constraints en requirements gespecificeerd
- [ ] Validation criteria gedefinieerd
- [ ] Timeline en deliverables duidelijk
- [ ] Stakeholder perspective geïncludeerd

---

## 7 Appendix: Placeholder Reference

### 7.1 Standaard Placeholders

**Product/Service Related:**
- `[productcategorie]` - Specifieke product category
- `[product/service]` - Specifiek product of service
- `[specificatie]` - Technische specificaties
- `[volume]` - Inkoopvolume

**Leverancier Related:**
- `[leverancier]` - Specifieke leverancier naam
- `[leverancier type]` - Type leverancier (manufacturer, distributor, etc.)
- `[leverancier capabilities]` - Leverancier mogelijkheden

**Organisatie Related:**
- `[industrie]` - Industrie sector
- `[bedrijf]` - Bedrijfsnaam
- `[business unit]` - Specifieke business unit
- `[stakeholder]` - Relevante stakeholders

**Process Related:**
- `[periode]` - Tijdsperiode
- `[budget]` - Budget constraints
- `[deadline]` - Project deadline
- `[prioriteit]` - Prioriteitsniveau

### 7.2 Advanced Placeholders

**Strategic:**
- `[business strategy]` - Overkoepelende business strategy
- `[competitive advantage]` - Gewenste competitive advantage
- `[market position]` - Huidige marktpositie
- `[growth objectives]` - Groeidoelstellingen

**Risk & Compliance:**
- `[risk tolerance]` - Organisatie risk tolerance
- `[compliance requirements]` - Specifieke compliance eisen
- `[regulatory environment]` - Regulatoire context
- `[audit requirements]` - Audit vereisten

**Financial:**
- `[cost target]` - Kosten doelstelling
- `[savings target]` - Besparingsdoelstelling
- `[budget constraints]` - Budget beperkingen
- `[financial criteria]` - Financiële criteria

---

© 2025 Qando • Vragen / feedback? **[jacob.quak@qando.nl](mailto:jacob.quak@qando.nl)**

---

*Laatste update: Juli 2025 | Versie: 2.0 Definitieve Uitgave*
