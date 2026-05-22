# LULLPET — Stato lavori (revisione onesta del sito)

Ultimo aggiornamento: 2026-05-22
Branch git: `claude/ecommerce-strategy-analysis-38V5T`

## Contesto

Lullpet = brand di pet wellness (prodotti calmanti per cani/gatti ansiosi), nuovo,
dropshipping con Zendrop (magazzino USA, consegna ~5-8 giorni), società UK (Lullpet LTD),
store Shopify per il mercato USA. Obiettivo: contenuto del sito ONESTO ma comunque premium,
senza claim inventati, pronto per le ads Meta senza creare dubbi/contestazioni.

## Dati chiave

- Store: Lullpet — lullpet.com — piano Basic — USD — società in UK
- Theme live: "chug-template" (base Shrine). NB: le modifiche al tema live sono BLOCCATE via API.
- Blog: "Pet Care Guide" — id `gid://shopify/Blog/89496846544` — 8 articoli
- Email usate: hello@lullpet.com (principale), press@lullpet.com
- Pattern tecnico delle pagine: vedi `PATTERN_TECNICO_PAGINE.md`

## FATTO

### Contenuto reso onesto — rimossi tutti i claim inventati
Team fittizio, sedi Brooklyn/Ohio, magazzino di proprietà, spedizione 24h/3-5gg,
statistiche donazioni ($12.400 / 14 rifugi / 4.247 ordini), partner rifugi (ASPCA ecc.),
"4.247 verified reviews" + recensioni inventate, panel/claim veterinari, certificazioni
(carbon-neutral, OEKO-TEX, B Corp), date, press "as featured in", impact report PDF,
"team of six", risposta in 12 ore, programmi inesistenti (subscribe&save, refill).

### 8 pagine oneste pubblicate live (incollate manualmente dall'utente)
Our Story, Press, Why Lullpet, Shelter Donation, Sustainability, FAQ, Shipping, Contact.

### 6 pagine corrette via API (22-05-2026)
Track Your Order, Pet Sizing Guide, Refund Policy, Care Instructions,
Pet Care Guide, Affiliate Program — fix "12 ore"→"24 ore", "vet-reviewed/vet-approved"
→ onesto, "from our warehouse"→"from dispatch", rimosso "dashboard"/partners@ su Affiliate.

### Schema markup (JSON-LD) aggiornato e reso onesto
- FAQ → schema `FAQPage` ricostruito con le 17 Q&A oneste.
- Our Story → schema `Organization` onesto (name, legalName "Lullpet LTD", url, email,
  contactPoint). Niente foundingDate / dipendenti / indirizzo inventato.
- Care Instructions → schema `HowTo` già onesto, mantenuto.

### 8 articoli blog corretti via API (22-05-2026)
Tutti e 8 gli articoli del blog "Pet Care Guide": autore "Dr. Elena Russo, DVM"
→ "The Lullpet Team"; badge "Vet-reviewed" → "Researched with care"; callout
"Vet-reviewed" → "Health note"; rimossi i claim veterinari nei prodotti; titolo
8° articolo "...15 Vet-Backed Ways" → "...15 Practical Ways".

### File locali
File `*-honest.html` (versioni oneste) + file `*-v13.html` corretti, su git nel branch sopra.

## DA FARE

1. **Pagina legale "Contact information"** — inserire indirizzo registrato UK reale +
   numero Companies House (l'utente li manderà appena pronti).
2. **Reviews page** — consigliato metterla offline / toglierla dal footer: contiene
   "4.247 verified reviews" finte; ripubblicarla con un'app reviews quando ci saranno
   recensioni vere.
3. **Affiliate page** — pubblicarla solo se si attiva davvero un'app affiliate
   (tracking link, payout); altrimenti tenerla offline.
4. **Organization schema** — aggiungere `logo` (URL del logo) e confermare che il nome
   legale esatto sia "Lullpet LTD" (come da Companies House).
