# PIANO META ADS — DALLA A ALLA Z
## Strategia completa per Shopify Fashion USA (Trendsi + alternative)

> **Documento operativo** — segui passo dopo passo. Non saltare step.
> Versione: Maggio 2026

---

## INDICE

1. [Tabella Master — Ordine di Lancio Campagne](#tabella-master)
2. [Step 0 — Setup Tecnico](#step-0)
3. [Campagna #1 — ASC+ Broad Main](#campagna-1)
4. [Campagna #2 — ABO Interest Testing](#campagna-2)
5. [Campagna #3 — Catalog Retargeting Warm](#campagna-3)
6. [Campagna #4 — Catalog Retargeting Hot](#campagna-4)
7. [Campagna #5 — Advantage+ Catalog Broad](#campagna-5)
8. [Campagna #6 — ASC+ Scaling Winner](#campagna-6)
9. [Campagna #7 — Creative Testing Lab](#campagna-7)
10. [Quadro Budget per Fasi](#budget-fasi)
11. [Roadmap 90 Giorni](#roadmap-90)
12. [KPI Target Fashion USA 2026](#kpi)
13. [Regole d'Oro](#regole-oro)
14. [Errori da Evitare](#errori)
15. [Stack Tools Raccomandato](#stack)

---

## TABELLA MASTER — ORDINE DI LANCIO CAMPAGNE <a name="tabella-master"></a>

| # | Campagna | Quando lanciarla | Budget iniziale | Obiettivo | Quando passare alla successiva |
|---|----------|------------------|-----------------|-----------|-------------------------------|
| 0 | Setup tecnico (Pixel, CAPI, Catalog) | Giorno 0 | $0 | Tracking funzionante | Quando vedi eventi in Events Manager |
| 1 | **ASC+ Broad — TOF Main** | Giorno 1 | $50/day | Trovare freddi che comprano | Sempre attiva, mai spenta |
| 2 | **ABO Interest Testing** | Giorno 7-10 | $50/day ($10×5 ad set) | Validare prodotti diversi | Dopo aver trovato 1 winner |
| 3 | **Catalog Retargeting Warm (DPA)** | Giorno 14 (≥500 VC) | $15/day | Recuperare chi ha visto il sito | Sempre attiva |
| 4 | **Catalog Retargeting Hot (DPA)** | Giorno 14 | $10/day | Chiudere ATC e Initiate Checkout | Sempre attiva |
| 5 | **Advantage+ Catalog Broad** | Giorno 21-30 | $30-50/day | DPA su freddo (scala il catalogo) | Sempre attiva |
| 6 | **ASC+ Scaling Winner** | Quando trovi un winner | $100/day → scala | Spingere il winner al massimo | Mai chiudere finché ROAS regge |
| 7 | **ASC+ Creative Testing Lab** | Mese 2 | $30-50/day | Testare creative nuove isolate | Sempre attiva da mese 2 |

---

## STEP 0 — SETUP TECNICO (giorno 0) <a name="step-0"></a>

### Senza questo step, le tue ads non sanno cosa succede sul sito.

| # | Azione | Dove | Note |
|---|--------|------|------|
| 1 | Creare Business Manager | business.facebook.com | Account business, no personale |
| 2 | Creare Ad Account USA | BM → Business Settings → Ad Accounts | Valuta USD, fuso EST |
| 3 | Creare Pixel | Events Manager → Connect Data Sources → Web | Nome: "Pixel_NomeStore" |
| 4 | Installare Pixel su Shopify | Shopify → Sales Channels → Facebook → Connect | Auto via app Meta |
| 5 | Attivare **Conversion API (CAPI)** | Shopify app Meta → Settings | OBBLIGATORIO 2026 |
| 6 | Verificare dominio | Events Manager → Brand Safety → Domains | DNS o meta tag |
| 7 | Aggregated Events: 8 eventi prioritari | Events Manager → AEM | Purchase, ATC, IC, VC, AddPaymentInfo, Lead, Search, CompleteRegistration |
| 8 | Caricare Catalog | Commerce Manager → Catalogs → Create | Source: Shopify (auto-sync) |
| 9 | Creare 6 Product Set base | Commerce Manager → Sets | All_Products, Dresses, Sets, Tops, Bottoms, Bestsellers |
| 10 | Test eventi | Events Manager → Test Events | Apri sito, fai ATC, verifica arrivo |

**REGOLA:** Non procedere finché Test Events non mostra eventi in tempo reale.

---

## CAMPAGNA #1 — ASC+ BROAD MAIN <a name="campagna-1"></a>

### Perché lanciarla per prima
ASC+ è la campagna principale del 2026. Meta usa AI per trovare i tuoi compratori. Farà l'**80% delle vendite**. Lanciala giorno 1 e lasciala accesa per sempre.

### Struttura
```
Campaign:   ASC_Main_Broad_USA_0511
└── Ad Set:  (ASC ha 1 solo ad set, gestito da Meta)
    └── Ads: 6-10 ads diversi (UGC + statici + carousel)
```

### Setup — Livello CAMPAGNA
| Campo | Valore |
|-------|--------|
| Obiettivo | Sales |
| Tipo | Advantage+ Shopping Campaign (ASC+) |
| Nome | `ASC_Main_Broad_USA_0511` |
| Budget | $50/day CBO |
| Bid strategy | Highest Volume |
| Attribution | 7-day click, 1-day view |

### Setup — Livello AD SET
| Campo | Valore |
|-------|--------|
| Country | United States only |
| Età | 18-65+ |
| Existing customer budget cap | 20% |
| Placement | Advantage+ Placements (tutti) |
| Optimization event | Purchase |

### Setup — Livello AD (caricare 6-10 ads dall'inizio)

| Slot | Tipo creative | Esempio |
|------|---------------|---------|
| 1 | UGC video 15-20s | Mirror selfie try-on |
| 2 | UGC video 15-20s | POV "outfit per matrimonio" |
| 3 | UGC video 15-20s | Try-on haul 3 prodotti |
| 4 | Statico foto prodotto + prezzo | "Linen set $58 — ships USA" |
| 5 | Statico social proof | "4.8★ — 2,341 reviews" + foto |
| 6 | Carousel 5 prodotti hero | Bestseller con prezzo |
| 7 | Statico comparison/dupe | "$300 designer vs our $65" |
| 8 | Slideshow auto da catalog | Auto Shopify |

### Copy formula universale
```
HOOK (1 riga) + BENEFIT (1-2 righe) + SOCIAL PROOF (1 riga) + CTA chiara
```

### Esempio copy reale
```
The matching set every girl on TikTok is wearing 💛

Linen-blend, breathable, designed in LA.
Wear it to brunch, to the beach, or with sneakers.

⭐ 4.8/5 — 2,341 happy customers
🇺🇸 Ships from USA in 2-4 days
✨ Free shipping over $75

Shop now → [link]
```

### Budget
| Fase | Budget/day | Durata |
|------|------------|--------|
| Lancio | $50 | Giorni 1-7 |
| Validazione | $70-100 | Se ROAS Day-7 > 1.5 |
| Scaling | +20% ogni 3 giorni | Solo se ROAS regge |

### Kill rules (singoli ads dentro ASC)
| Condizione | Azione |
|------------|--------|
| Ad con spend > $30 e 0 ATC | Spegni quell'ad |
| Ad con CTR < 0.8% dopo $25 spend | Spegni |
| Ad con CPATC > 3× target dopo $40 | Spegni |
| Frequency > 4 + CTR cala >25% | Refresh |

**MAI spegnere campagna ASC+ intera nei primi 7 giorni** — è in learning phase.

### KPI Day-7 check
| Metrica | Soglia per continuare |
|---------|-----------------------|
| CTR link | > 1.4% |
| CPC link | < $1.50 |
| CPATC | < $10 |
| ROAS | > 1.3 |

---

## CAMPAGNA #2 — ABO INTEREST TESTING <a name="campagna-2"></a>

### Perché lanciarla seconda (giorno 7-10)
ASC+ è broad — non ti dice quale prodotto piace a quale pubblico. ABO testing valida prodotti diversi su pubblici diversi. È la "macchina del trovare winner".

### Struttura
```
Campaign: TEST_ABO_Sales_USA_0511 (ABO, NON CBO)
├── Ad Set 1: Interest "Fashion + Boutique" → Prodotto A (3 ads)
├── Ad Set 2: Interest "Wedding + Bridesmaid" → Prodotto B (3 ads)
├── Ad Set 3: Interest "Yoga + Wellness" → Prodotto C (3 ads)
├── Ad Set 4: Broad no-interest → Prodotto D (3 ads)
└── Ad Set 5: LAL 1-3% Purchase (quando ≥100 purchase) → Prodotto E (3 ads)
```

### Setup — Livello CAMPAGNA
| Campo | Valore |
|-------|--------|
| Obiettivo | Sales |
| Tipo | Manual (non ASC) |
| Budget level | **Ad Set Budget (ABO)** — NON CBO |
| Bid | Highest Volume |
| Conversion event | Purchase (o ATC se <50 purchase/sett) |

### Setup — Livello AD SET (per ogni prodotto)
| Campo | Valore |
|-------|--------|
| Budget | $10/day per ad set (totale 5 = $50/day) |
| Audience | 1 interest specifico per ad set (NO stacking) |
| Geo | USA only |
| Età | 22-45 |
| Placement | Advantage+ |
| Optimization | Purchase |

### Esempi interest puliti (uno per ad set)
- "Shein"
- "Princess Polly"
- "Reformation"
- "Lulus"
- "Bridesmaid dresses"
- "Boutique" + behavior "Engaged shoppers"

### Setup — Livello AD (3 ads/ad set, stesso prodotto, angoli diversi)
- Ad A: UGC try-on
- Ad B: Statico prezzo + social proof
- Ad C: Video editato con prezzo on-screen

### Decision rules
| Spend per ad set | Decisione |
|------------------|-----------|
| $0-15 | "Wait" — non toccare |
| $15-25 | "Early signals" — guarda CTR + CPATC |
| $25-40 | "Statistical relevance" — scale o kill |
| $40+ con 0 ATC | KILL ad set |
| ROAS > 1.5 a $30 spend | Lascia girare altri $20 |
| ROAS > 2 a $50 spend | **WINNER** → sposta in Campagna #6 |

---

## CAMPAGNA #3 — CATALOG RETARGETING WARM <a name="campagna-3"></a>

### Quando lanciarla (giorno 14)
Non lanciare prima di avere **≥500 ViewContent** accumulati. Retargeting con poco traffico = spreco budget.

### Struttura
```
Campaign: RT_Catalog_Warm_USA_0511 (Sales + DPA)
└── Ad Set: Warm audience (VV180 + Engagement 90d + IG-FB Engagers 90d + Web visitors 180d)
    └── Ad: Dynamic Product Ad (catalog feed)
```

### Setup — CAMPAGNA
| Campo | Valore |
|-------|--------|
| Obiettivo | Sales |
| Tipo | Manual |
| Catalog | Tuo catalog Shopify |
| Budget | $15/day Ad Set Budget |

### Setup — AD SET
| Campo | Valore |
|-------|--------|
| Audience | Custom: VV 75% 180d + IG Engagers 90d + FB Page Engagers 90d + Website Visitors 180d (NO purchasers) |
| Exclusion | Purchasers 180d, ATC 7d |
| Product set | "All_Products" o "Bestsellers" |
| Geo | USA |
| Placement | Advantage+ |
| Optimization | Purchase |

### Setup — AD (DPA dinamico)
| Campo | Valore |
|-------|--------|
| Format | Carousel dinamica da catalog |
| Template testo | "You loved this 👀 — still available, ships fast 🇺🇸" |
| Pricing overlay | ON |
| Discount overlay | OFF |

### KPI target
- ROAS > 4 (warm deve fare ROAS alto)
- CPM più alto del TOF è normale ($35-50)
- CTR > 2%

---

## CAMPAGNA #4 — CATALOG RETARGETING HOT <a name="campagna-4"></a>

### Perché serve separata
Chi ha messo nel carrello (ATC) o avviato checkout (IC) ha intenzione 10× più alta. Trattali con incentivo (codice sconto).

### Struttura
```
Campaign: RT_Catalog_Hot_USA_0511
├── Ad Set 1: ATC 30d (no purchase) → DPA con codice "COMEBACK10"
└── Ad Set 2: IC 7d (no purchase) → DPA con codice "FINAL15"
```

### Setup — AD SET 1 (ATC)
| Campo | Valore |
|-------|--------|
| Budget | $7/day |
| Audience | ATC 30 days |
| Exclusion | Purchase 60d |
| Product set | "All_Products" |

### Setup — AD SET 2 (Initiate Checkout)
| Campo | Valore |
|-------|--------|
| Budget | $5/day |
| Audience | InitiateCheckout 7 days |
| Exclusion | Purchase 30d |
| Product set | "All_Products" |

### Copy esempi
**ATC:**
```
Forgot something? 👀
Your cart is still waiting.
Use code COMEBACK10 for 10% off — expires in 24h.
```

**IC:**
```
Last chance — your checkout expires soon.
Code FINAL15 for 15% off. Today only.
```

### KPI target
- ROAS > 6-8 (hot audience deve esplodere)
- Spend basso, no scaling — set & forget

---

## CAMPAGNA #5 — ADVANTAGE+ CATALOG BROAD <a name="campagna-5"></a>

### Perché lanciarla dopo le retargeting (giorno 21-30)
DPA su pubblico freddo. Serve abbastanza dati pixel (~500 purchase + 5.000 ATC) per ottimizzare. Lanciarla troppo presto = spreca budget.

### Struttura
```
Campaign: ASC_Catalog_Broad_USA_0511
└── Ad Set: Advantage+ broad (no audience definita)
    └── Ad: DPA dynamic dal catalogo
```

### Setup
| Campo | Valore |
|-------|--------|
| Obiettivo | Sales |
| Tipo | Manual o Advantage+ Catalog |
| Catalog | Shopify catalog |
| Product set | "Bestsellers_30d" (auto-aggiornato) |
| Audience | NO custom audience — broad totale |
| Exclusion | Purchasers 60d |
| Budget | $30/day → $80-100 quando funziona |
| Optimization | Purchase |

### Perché è potente
DPA broad scala da sola: pesca i prodotti winner dal catalog automaticamente. La campagna più "lazy" e redditizia del 2026.

---

## CAMPAGNA #6 — ASC+ SCALING WINNER <a name="campagna-6"></a>

### Quando lanciarla
Quando un singolo prodotto ha:
- 20+ vendite in 7 giorni
- ROAS > 2.5 stabile
- CR > 3%
- Return rate < 8%

### Struttura
```
Campaign: ASC_Scaling_LinenSet_USA_0511
└── Ad Set: ASC+ broad
    └── Ads: 8-12 ads tutti su QUEL prodotto
```

### Setup
| Campo | Valore |
|-------|--------|
| Obiettivo | Sales |
| Tipo | ASC+ |
| Audience | Default ASC (broad) |
| Budget | $100/day iniziale, +20% ogni 3 giorni |
| Ads | 8-12 creative TUTTE sul prodotto winner |
| Existing customer budget cap | 15% |

### Regola scaling
| Giorno | Budget | Condizione |
|--------|--------|------------|
| 1-3 | $100 | Lancio |
| 4-6 | $130 | ROAS > 2.5 |
| 7-9 | $170 | ROAS > 2.3 |
| 10-12 | $220 | ROAS > 2.2 |
| 13-15 | $290 | ROAS > 2.0 |
| 16+ | +20% ogni 3 giorni | Stop quando ROAS < target -20% |

**Se ROAS scende:** torna al budget precedente, aspetta 4 giorni, riprova.

---

## CAMPAGNA #7 — CREATIVE TESTING LAB <a name="campagna-7"></a>

### Perché esiste (mese 2 in poi)
Account maturo (60+ giorni): il problema diventa trovare nuove creative che scalano. Test rapidi, isolati.

### Struttura
```
Campaign: TEST_ASC_CreativeLab_USA_0511
└── Ad Set: ASC+ broad
    └── 3-5 NUOVE creative ogni 7 giorni
```

### Setup
| Campo | Valore |
|-------|--------|
| Tipo | ASC+ |
| Budget | $30-50/day fisso |
| Audience | Broad |
| Rotazione | Ogni lunedì: aggiungi 3-5 ads, kill quelli con CTR < 1% dopo $25 spend |
| Winner | CTR > 2.5% + ROAS > 2 → sposta in ASC Main (#1) |

---

## QUADRO BUDGET PER FASI <a name="budget-fasi"></a>

| Fase | Spese mensili | Campagne attive | Revenue obiettivo |
|------|---------------|-----------------|-------------------|
| Settimana 1-2 | ~$700-1.000 | #1 ASC Main | $1.5-2.5k |
| Settimana 3-4 | ~$1.500-2.500 | #1 + #2 + #3 + #4 | $4-7k |
| Mese 2 | ~$3.000-6.000 | #1 + #2 + #3 + #4 + #5 + #6 | $9-18k |
| Mese 3 | ~$6.000-15.000 | Tutte + #7 + scaling x2 winner | $20-50k |
| Mese 4+ | ~$15.000-50.000+ | Tutte + più ASC Scaling | $50-200k+ |

---

## ROADMAP 90 GIORNI <a name="roadmap-90"></a>

| Giorno | Cosa fai | Budget giornaliero |
|--------|----------|--------------------|
| 0 | Setup Pixel + CAPI + Catalog | $0 |
| 1 | Lancia Campagna #1 ASC Main | $50 |
| 2-6 | Non toccare. Aggiungi 2 nuovi creative/giorno in #1 | $50 |
| 7 | Check KPI #1. Se OK, $70. Lancia #2 ABO Testing | $120 |
| 8-13 | Monitora ABO: kill ad set morti dopo $40 | $120-150 |
| 14 | Lancia #3 Retargeting Warm + #4 Hot | $150-180 |
| 15-20 | Stabilizza. ROAS > 2 → +20% su #1 ogni 3 giorni | $200-260 |
| 21-30 | Lancia #5 Catalog Broad | $280-350 |
| 31-45 | Identifica primo winner → Lancia #6 Scaling | $400-600 |
| 46-60 | Scala winner. Cerca secondo winner in ABO | $700-1.200 |
| 60+ | Lancia #7 Creative Lab. Pipeline UGC strutturata | $1.500+ |

---

## KPI TARGET FASHION USA 2026 <a name="kpi"></a>

| Metrica | Minimo | Buono | Eccellente |
|---------|--------|-------|------------|
| CPM | <$32 | $20-28 | <$18 |
| CTR link | >1.5% | 2.2-3.5% | >4% |
| CPC link | <$1.40 | $0.70-1.10 | <$0.60 |
| CR sito | >1.8% | 2.8-4% | >5% |
| AOV | >$58 | $75-95 | >$110 |
| ROAS blended | 1.8 | 2.5-3.5 | >4 |
| Contribution margin | >25% | 35-45% | >50% |
| Return rate | <12% | <9% | <6% |

---

## REGOLE D'ORO <a name="regole-oro"></a>

1. **Una campagna alla volta.** Non lanciare tutto insieme il giorno 1.
2. **Non toccare niente nei primi 3 giorni** di ogni nuova campagna (learning phase).
3. **Mai cambiare budget +50% di colpo.** Max +20% ogni 3 giorni.
4. **6-10 ads minimo dentro ogni ASC.** Mai 1 solo.
5. **Kill ad set ABO dopo $40 spend con 0 ATC.** Niente pietà.
6. **CAPI obbligatorio.** Senza, attribuzione perde 25%.
7. **No sconto nelle ads TOF (#1 #2 #5).** Sconto solo in retargeting hot (#4).
8. **Email/SMS Klaviyo da subito** — raddoppia ROAS blended.
9. **Refresh creative ogni 14-21 giorni** — fashion brucia ads veloce.
10. **Misura su 7-day click + dashboard Shopify**, non solo Ads Manager.

---

## ERRORI DA EVITARE (top 10) <a name="errori"></a>

1. Testare 50 prodotti in parallelo
2. Spegnere ad set durante learning phase
3. Lookalikes 1% come acquisition primaria (morti nel 2026)
4. Discount 40% off day 1 (brand dead)
5. Catalog feed con immagini diverse dalla landing
6. Landing PDP lenta (ogni 1s = -7% CR)
7. Solo broad senza creative diversification
8. SKU "China-direct" (return rate 25%+)
9. Ignorare email/SMS (25% revenue gratis se fatto)
10. Cambiare tutto ogni 3 giorni invece di aspettare significance

---

## STACK TOOLS RACCOMANDATO 2026 <a name="stack"></a>

| Funzione | Tool |
|----------|------|
| Tracking server-side | TripleWhale o Northbeam |
| CAPI Meta | Elevar (best in class) |
| Email/SMS | Klaviyo + Postscript |
| Reviews UGC | Loox o Judge.me |
| Upsell/Bundle | Rebuy + ReConvert |
| Landing/PDP builder | Replo o Shogun |
| UGC sourcing | Insense + Billo + Trend.io |
| Creative editing | CapCut Pro + Pebblely (statici AI) |
| Analytics ads | Motion (creative analytics) |
| AI creative | Arcads / Creatify |
| Inventory sync Trendsi | App Trendsi nativa + Stocky |
| Customer service | Gorgias |

---

## SUPPLIER MIX RACCOMANDATO

```
60% catalog → Trendsi (SOLO US warehouse filter ON)
25% catalog → Bloom Wholesale (prodotti viral/trendy hero)
15% catalog → MyOnlineFashionStore (occasion wear ad alto AOV)
```

**REGOLA:** Mai usare overseas/China-direct SKU per ads scaling.

---

## CHECKLIST OPERATIVA SETTIMANALE

### Lunedì
- [ ] Review KPI weekend (CPM, CTR, ROAS, CPATC)
- [ ] Aggiungi 3-5 creative nuovi in Campagna #7 (Creative Lab)
- [ ] Brief 3 nuovi UGC per la settimana

### Mercoledì
- [ ] Check ABO testing: kill ad set morti
- [ ] Verifica budget scaling Campagna #6
- [ ] Refresh ad fatigue check (frequency >4)

### Venerdì
- [ ] Promote winner da Creative Lab → ASC Main
- [ ] Update product set "Bestsellers_30d"
- [ ] Pianifica creative weekend

### Domenica sera
- [ ] Report settimanale: spend / revenue / ROAS / CPA / nuovi customer
- [ ] Pianifica budget settimana successiva (+20% se ROAS regge)

---

## NOTE FINALI

- Questo piano funziona se applicato **rigorosamente per 90 giorni**.
- I primi 14 giorni sono i più difficili: poco data, ROAS instabile. Resisti.
- Il vero scaling parte dal mese 2: non aspettarti $50k/mese a settimana 3.
- **Creative > Audience > Budget**. Ricorda sempre questo ordine.
- Se ROAS non parte dopo 30 giorni di applicazione corretta: il problema è il prodotto o la landing, non le ads.

---

**Fine documento.**
Versione: 1.0 — Maggio 2026
Strategia: Meta Ads completa per Shopify Fashion USA Womens
