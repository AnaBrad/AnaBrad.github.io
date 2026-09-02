# Playbook — Conținut de blog

Un articol pe săptămână. Articolul e piesa centrală: din el ies postările, clipurile și,
uneori, resursa. Se scrie întâi articolul, apoi restul.

## Înainte să scrii

1. Citește 2 articole existente pe teme apropiate — pentru voce și pentru a nu repeta.
2. Verifică ce instrument de pe `/instrumente-coaching/` se leagă de temă.
3. Stabilește: **cine** citește, **ce întrebare** își pune, **cu ce pleacă** după lectură.
4. Dacă tema atinge zona clinică, recitește `../context/etica-si-limite.md`.

## Structura care funcționează pe site

Modelul se vede clar în `blog/cat-costa-coaching.html`:

1. **Deschidere prin recunoaștere** — cititorul se regăsește în primele 2–3 fraze.
   Nu începe cu „În ziua de azi…" și nici cu o definiție.
2. **Întrebarea firească** — pusă exact cum și-o pune el.
3. **Corpul** — secțiuni cu `<h2>` formulate ca întrebări. 3–6 secțiuni.
4. **Nuanțarea** — ce nu oferă coachingul, ce nu promitem, când nu e potrivit.
   Această secțiune e semnătura Anei. Nu o sări.
5. **Adolescenți / părinți**, dacă tema o cere — secțiune separată, nu propoziții
   strecurate.
6. **Un pas concret** — întrebări de reflecție, un exercițiu, un instrument.
7. **Închidere caldă** + CTA către ședința de cunoaștere.

Lungime: 900–1.500 de cuvinte. Sub 700 rareori e util; peste 2.000 nu se citește.
Paragrafe de 2–4 rânduri. Citate izolate cu `<p class="say">` pentru frazele care merită
respirație.

## Livrabilul

Fișier în `../drafturi/`, numit `AAAA-LL-ZZ-blog-<slug>.md`, cu antet:

```markdown
---
tip: articol de blog
slug: cat-costa-coaching
titlu_pagina: "Cât costă coaching-ul: ce plătești, de fapt, într-o ședință | Ana-Maria Brad"
titlu_articol: "Cât costă coaching-ul și ce cumperi, de fapt, când plătești o ședință"
subtitlu: "Ce plătești într-o ședință de coaching, și ce nu cumperi"
meta_description: "…"   # 150–160 de caractere, cu diacritice
cuvinte_cheie: "…"      # pentru JSON-LD
audienta: femei / bărbați / părinți de adolescenți / mixt
cuvant_cheie_principal: "…"
legaturi_interne:
  - /blog/…
  - /instrumente-coaching/…
data_propusa: 2026-…
stadiu: schiță
marcaje_de_completat: 0
---
```

Scrii articolul în Markdown. **Nu genera HTML până când Ana nu aprobă textul** — altfel
se pierde timp la fiecare revizuire.

## De la Markdown la HTML (numai după aprobare)

1. Copiază un articol recent ca schelet: `cp blog/cat-costa-coaching.html blog/<slug>.html`.
2. Înlocuiește, în ordine: `<title>`, `meta description`, `author` rămâne, `canonical`,
   `hreflang`, toate `og:*`, `twitter:image`, JSON-LD `BlogPosting` (headline,
   description, url, mainEntityOfPage, datePublished, dateModified, keywords), JSON-LD
   `BreadcrumbList` (poziția 3).
3. Înlocuiește corpul: `<h1>`, `.subtitle`, data publicării, secțiunile.
4. `data-umami-event-loc` de la CTA-ul final devine `blog-<slug>-1`.
5. Adaugă cardul în `blog/index.html`, în poziția indicată de Ana.
6. Adaugă intrarea în `sitemap.xml` (`priority` 0.7, `lastmod` = data publicării).
7. Parcurge `../sabloane/checklist-inainte-de-publicare.md`.

Toți acești pași sunt „publicare pe site" → cer aprobarea explicită a Anei.

## Reguli de scriere

- Titlul promite exact ce livrează textul. Fără „secretul", fără „nimeni nu-ți spune".
- Un singur subiect per articol.
- Fiecare afirmație generală e urmată de un exemplu sau de o consecință concretă.
- Teoriile se citează cu autor (așa cum se face deja: Whitmore, Oettingen, Byron Katie,
  Covey, Plutchik, Marcia Reynolds).
- Fără povești personale inventate. Unde ar fi nevoie:
  `[DE COMPLETAT DE ANA: …]`, numărate în antet la `marcaje_de_completat`.
- Diacritice peste tot, inclusiv în metadate.

## Teme deja acoperite (nu le repeta)

momente decisive · a spune nu · motivație durabilă · conflict de valori · fereastra de
toleranță · ce e coachingul · cât costă · ședința de cunoaștere · povestea începutului.

**„Etica în coaching" este temă obligatorie în planul editorial următor** — vezi
`../plan/plan-editorial-curent.md`. Când o scrii, aplică regula de verificare a Codului
etic ICF din `../context/etica-si-limite.md`, punctul 5.
