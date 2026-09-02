# Canale și convenții tehnice

## Site — cum e construit

Site static, HTML scris de mână, publicat prin GitHub Pages din rădăcina depozitului
(`CNAME` → anamariabrad.ro). **Nu există generator de site, nu există Markdown pe site.**
Un articol nou înseamnă un fișier HTML complet.

```
/                          index.html — pagina principală (ofertă, FAQ, testimoniale, formular Tally)
/blog/                     index.html + un fișier .html per articol
/instrumente-coaching/     26 de instrumente interactive + index
/link/                     hub de linkuri pentru bio Instagram
/confidentialitate.html    politica de confidențialitate
/assets/                   fonturi self-hosted, imagini, og-image
/sitemap.xml               harta site-ului
/robots.txt
```

### Convenția unui articol de blog

Copiază structura dintr-un articol recent — `blog/cat-costa-coaching.html` e cel mai
bun model. Un articol are:

- `<html lang="ro">`, `<title>` de forma `Titlu | Ana-Maria Brad`;
- `<meta name="description">` (~150–160 de caractere), `<meta name="author">`;
- `<link rel="canonical">` și `<link rel="alternate" hreflang="ro">`;
- meta Open Graph: `og:type=article`, `og:site_name=Capitolul următor`, `og:url`,
  `og:title`, `og:description`, `og:image`, `og:locale=ro_RO`;
- `twitter:card=summary_large_image` și `twitter:image`;
- JSON-LD `BlogPosting` (headline, description, url, mainEntityOfPage, image,
  datePublished, dateModified, inLanguage, keywords, author, publisher);
- JSON-LD `BreadcrumbList` (Acasă → Blog → titlul articolului);
- fonturile și CSS-ul inline, identice cu ale celorlalte articole;
- bara de anunț, antetul de brand, navigația, butonul Calendly din navigație;
- corpul: `<a class="back" href="/blog/">`, `<h1>`, `<p class="subtitle">`, data
  publicării, secțiuni cu `<h2>`, citate cu `<p class="say">`, liste `<ul>`;
- final: CTA Calendly cu `data-umami-event="calendly"` și
  `data-umami-event-loc="blog-<slug>-1"`, apoi `.cta-sub` și `.write-me`;
- subsolul standard.

Numele fișierului: slug fără diacritice, cu cratime — `cat-costa-coaching.html`.
Slugul nu se schimbă după publicare (rupe legăturile și SEO).

### Ce se atinge la publicarea unui articol (doar cu aprobare)

1. `blog/<slug>.html` — fișierul nou;
2. `blog/index.html` — cardul nou, în poziția editorială stabilită de Ana
   (`<a class="post" href="…"><h2>…</h2><p>…</p><span class="more">Citește →</span></a>`);
3. `sitemap.xml` — intrare `<url>` cu `<loc>`, `<lastmod>`, `<priority>0.7</priority>`
   și `xhtml:link hreflang="ro"`.

Ordinea cardurilor pe `blog/index.html` e **editorială, nu cronologică** — o decide Ana.
Nu o rearanja din proprie inițiativă.

### Legături interne

Fiecare articol nou ar trebui să trimită către 2–4 pagini existente și să fie, la rândul
lui, o candidatură pentru legături din articolele înrudite. Inventarul actual:

**Articole:** `5-semne-moment-decisiv`, `cum-sa-spun-nu-nevoi-sociale`,
`motivatie-care-dureaza`, `cand-valorile-personale-intra-in-conflict`,
`fereastra-de-toleranta`, `ce-e-coaching`, `cat-costa-coaching`,
`prima-sedinta-de-cunoastere`, `cum-am-ajuns-sa-creez-spatiul`.

**Instrumente (26).** Adulți: roata vieții, roata încrederii, valori, credințe limitative,
cercul de control, harta energiei, GROW, WOOP, roata emoțiilor. Adolescenți: aceleași,
în variantă adaptată. Echipă: roata echipei, roata proiectului, GRPI, GRIT, PDCA, SPIN,
OSKAR. Autori: „De ce scriu această carte", „Ce mă blochează".

Un articol despre valori trimite la instrumentul „Valorile personale". Unul despre
epuizare trimite la „Harta energiei". Așa se leagă conținutul de instrumente.

## Măsurare

- **Umami** (`cloud.umami.is`, fără cookie-uri, fără identificare). Evenimente definite
  azi: `calendly` (cu `data-umami-event-loc`), `contact-email`, `contact-whatsapp`,
  `contact-tel`, `contact-instagram`, `contact-facebook`, `contact-linkedin`.
- **Calendly** — sursa de adevăr pentru ședințele programate.
- **Tally** — lista de așteptare de pe pagina principală.
- Nu există pixel Meta, Google Analytics sau alt tracking. Instalarea oricăruia e o
  schimbare externă și cere aprobare (plus actualizarea politicii de confidențialitate).
- Nu există încă o convenție de etichete UTM pentru legăturile din postări. Propune una
  Anei înainte de prima campanie (vezi contradicția C6).

## Rețele sociale

| Canal | Cont | Rol | Format |
| --- | --- | --- | --- |
| Instagram | @anamariabrad.coaching | vizibilitate, video scurt | Reels 30–60 s subtitrate, carusel 5–8 cadre, story |
| Facebook (pagină) | anamariabrad.ro | acoperire, articole | text 80–150 de cuvinte + legătură sau imagine |
| Facebook (grupuri) | grupuri aprobate | conversații reale | postare nativă, fără legătură comercială — vezi playbook |
| LinkedIn | profil personal | credibilitate profesională, tranziții de carieră | text 150–250 de cuvinte, fără legătură în corp |

- Instagram nu permite legături în descriere → toate trimiterile merg prin
  <https://anamariabrad.ro/link/>. Dacă o campanie are nevoie de o destinație nouă, se
  propune adăugarea ei pe pagina de linkuri (schimbare de site → aprobare).
- LinkedIn scade acoperirea postărilor cu legături externe în corp; pune legătura în
  primul comentariu, ca acțiune a Anei.
- Nu există pagină de companie pe LinkedIn. Postările sunt personale, la persoana I.

## Video

- Filmare cu telefonul, **fără microfon extern** → mediu liniștit, telefonul aproape,
  fără vânt, fără ecou. Se compensează prin subtitrare obligatorie.
- 30–60 de secunde, vertical 9:16.
- Filmare **în lot, o dată pe săptămână**: aceeași ținută sau ținute schimbate între
  clipuri, aceeași lumină, mai multe scenarii la rând.
- Subtitrări obligatorii, cu diacritice, verificate manual — generatoarele automate
  greșesc constant diacriticele românești.
- Detalii în `../playbooks/video-scurt.md`.

## Ce NU se atinge fără aprobare

`index.html`, `blog/**`, `instrumente-coaching/**`, `assets/**`, `sitemap.xml`,
`robots.txt`, `CNAME`, `confidentialitate.html`, `link/index.html` — plus orice cont,
platformă sau formular din afara depozitului.

## De ce trăiește totul sub `.claude/`

GitHub Pages publică rădăcina depozitului. Un folder obișnuit (de exemplu `marketing/`)
ar deveni public la `anamariabrad.ro/marketing/`. Folderele care încep cu punct sunt
ignorate de Jekyll, procesarea implicită a GitHub Pages (depozitul nu conține un fișier
`.nojekyll`). Materialele de lucru stau, deci, sub `.claude/marketing/` — sunt versionate
în git, dar nu ajung pe site. **Nu muta aceste fișiere în rădăcină** și, dacă cineva
adaugă vreodată un `.nojekyll`, verifică din nou dacă folderul a rămas neexpus.
