# LULLPET — Pattern Tecnico Pagine HTML (v13 — VALIDATO ✓)

Pattern CSS/HTML provato e funzionante per pagine Shopify Custom HTML
sul theme Shrine. Tutte le pagine Lullpet seguono ESATTAMENTE questo schema.

## REGOLE THEME-LEVEL (solo 2, sicure)

```css
/* 1. Nascondi il titolo auto-renderizzato da Shopify Page */
.template-page .page__title,
.template-page .page-title,
.template-page .page__heading,
.page-template__title,
.main-page-title,
.section-page-title { display: none !important; }

/* 2. Neutralizza il background del wrapper contenuto (elimina la peach
      sopra E sotto). #MainContent contiene SOLO il contenuto pagina —
      header e footer sono fratelli FUORI, quindi mai toccati. */
#MainContent,
.main-content,
main#MainContent { background-color: #fafaf7 !important; }
```

## REGOLE DA NON USARE MAI (rompono il theme)

- ❌ `margin-bottom` negativo sul container → rompe il footer
- ❌ `box-shadow: 0 Npx 0 0 color` per coprire → dipinge SOPRA il footer
- ❌ `width: 100vw` + `position: relative` + `left: 50%` → fragile
- ❌ `overflow-x: hidden` sul container → clippa contenuto
- ❌ SVG inline come `url("data:image/svg+xml,...")` → si corrompe in Shopify

## REGOLE SICURE (sempre usare)

- ✅ Full-bleed orizzontale: `margin-left: calc(50% - 50vw); margin-right: calc(50% - 50vw);`
- ✅ `margin-top: -60px` per coprire il padding superiore del theme
- ✅ `margin-bottom: 0` — mai negativo
- ✅ Tutte le classi scopate con prefisso univoco per pagina (`.lp-about`, `.lp-faq`, ...)
- ✅ CSS variables scopate dentro il wrapper (`--c-bg`, `--c-sage`, ecc.)
- ✅ Reset scopato: `.lp-PAGE, .lp-PAGE * { box-sizing: border-box; }`
- ✅ Bottoni CTA con `!important` su background/color/text-decoration (il theme
     Shrine sovrascrive i colori dei link `<a>`)
- ✅ Immagini placeholder = card text-based (quote editoriale), MAI SVG inline
- ✅ `@media (prefers-reduced-motion: reduce)` per accessibilità

## PALETTE LULLPET (token validati)

```
--c-bg:          #fafaf7   (off-white pagina)
--c-bg-pearl:    #f3ece0   (perlato — sezioni staccate)
--c-bg-white:    #ffffff   (card / sezioni alternate)
--c-bg-dark:     #1a1a1a   (sezioni accent scure)
--c-text:        #1a1a1a   (testo primario)
--c-text-soft:   #3a3a3a   (body copy)
--c-text-muted:  #5a5a5a   (testo secondario)
--c-sage:        #87968a   (accent calmo)
--c-taupe:       #b08968   (accent caldo su scuro)
--c-border:      #ececea   (bordi)
--c-border-soft: #e6dfd2   (bordi tenui)
```

## TIPOGRAFIA

- Headings: `'Cormorant Garamond', 'Playfair Display', Georgia, serif`
- Body: `'Inter', -apple-system, BlinkMacSystemFont, sans-serif`
- Eyebrow: 11px, letter-spacing 0.36em, uppercase, weight 600

## STRUTTURA SEZIONE TIPO

```
<div class="lp-PAGE">
  <section class="lp-PAGE-hero">...</section>      hero compatto
  <section class="lp-PAGE-...">...</section>        sezioni alternate bg
  <section class="lp-PAGE-cta">...</section>        CTA finale, padding 90px 0 100px
</div>
```

- Padding sezioni: 90px 0 (desktop) / 60px 0 (mobile <980px)
- Container: max-width 1320px, padding 0 40px (desktop) / 0 24px (mobile)
- Breakpoint: 980px e 540px

## STATO FILE — Our Story

VERSIONE FINALE VALIDATA: `about-us-v13.html`
Le versioni v1-v12 sono iterazioni superate, non usare.
