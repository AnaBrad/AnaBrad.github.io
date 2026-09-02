# Playbook — Pregătirea publicării

Când textul e aprobat de Ana, mai rămâne stratul care decide dacă îl găsește cineva.
Aici se pregătește, **fără** ca ceva să fie publicat.

## 1. Titlu

- **Titlul paginii** (`<title>`): 50–60 de caractere + ` | Ana-Maria Brad`. Conține
  expresia după care caută omul.
- **Titlul articolului** (`<h1>`): poate fi mai lung și mai uman decât cel al paginii —
  așa se face deja pe site.
- **Subtitlul** (`.subtitle`): o propoziție care spune ce ia cititorul din text.

Propune 3 variante de titlu și recomandă una, cu un rând de motivare.

## 2. Introducere

Primele 2–3 fraze fac două lucruri: cititorul se recunoaște și înțelege ce urmează.
Nu începe cu definiții, cu „în ziua de azi", cu „mulți dintre noi".

## 3. Metadate

| Element | Regulă |
| --- | --- |
| `meta description` | 150–160 de caractere, cu diacritice, cu verb la persoana a II-a, fără clickbait |
| `canonical` | `https://anamariabrad.ro/blog/<slug>.html` |
| `hreflang="ro"` | aceeași adresă |
| `og:title` | poate fi titlul articolului, nu al paginii |
| `og:description` | de regulă identică cu `meta description` |
| `og:image` | `https://anamariabrad.ro/assets/og-capitolul-urmator.png` dacă nu există imagine dedicată |
| `og:type` | `article` · `og:locale`: `ro_RO` · `og:site_name`: `Capitolul următor` |
| JSON-LD `BlogPosting` | headline, description, url, mainEntityOfPage, image, datePublished, dateModified, inLanguage, keywords, author, publisher |
| JSON-LD `BreadcrumbList` | Acasă → Blog → titlul articolului |

Verifică JSON-ul cu `python3 -m json.tool` înainte să-l consideri gata — un JSON-LD stricat
e invizibil pentru motoare și greu de observat cu ochiul.

## 4. Îndemnul la acțiune

- Unul singur, la final, către ședința de cunoaștere.
- `data-umami-event="calendly"` și `data-umami-event-loc="blog-<slug>-1"`.
- Sub el, fraza scurtă de liniștire („gratuită, ~30 de minute, fără nicio obligație").
- Dacă articolul e pe o temă unde CTA-ul comercial ar fi nepotrivit (temă grea, zonă
  clinică), propune în loc o trimitere către un instrument și spune de ce.

## 5. Legături interne

- 2–4 legături către articole sau instrumente existente, în corpul textului, cu ancoră
  descriptivă („instrumentul Harta energiei"), nu „aici".
- Verifică fiecare adresă: `ls blog/<slug>.html` sau
  `grep -o 'href="/instrumente-coaching/[^"]*"' instrumente-coaching/index.html | sort -u`.
- Propune și 1–2 articole existente în care ar merita adăugată o legătură **către** noul
  text. Modificarea lor e tot publicare → aprobare separată.

## 6. Variante de distribuire

Pentru fiecare articol, pregătește pachetul complet:

- 1 postare Facebook (pagină)
- 1 carusel Instagram (5–8 cadre) + descriere
- 1 postare LinkedIn + primul comentariu
- 1 scenariu video de 30–60 s
- 1 idee de postare nativă pentru un grup aprobat, **fără legătură comercială** și
  numai dacă intervalul de 7–14 zile permite (vezi `comunitati-facebook.md`)
- 1 variantă scurtă pentru story / mesaj de răspuns

## 7. Înainte de a cere aprobarea

Parcurge integral `../sabloane/checklist-inainte-de-publicare.md` și atașează rezultatul
la cererea de aprobare. Un „am verificat tot" fără listă bifată nu ajută pe nimeni.
