# Checklist înainte de publicare

Se parcurge integral pentru orice material, înainte de a cere aprobarea Anei. Rezultatul
se atașează la cererea de aprobare. Un punct nebifat nu se trece cu vederea: ori se
rezolvă, ori se scrie de ce rămâne așa.

## A. Adevăr și surse

- [ ] Nicio experiență personală a Anei inventată (poveste, client, emoție, amintire).
- [ ] Nicio cifră inventată: preț, statistică, număr de clienți, rezultate, volum de căutări.
- [ ] Prețurile corespund realității: 1.500 lei pachetul de 6 ședințe, 4 rate de 375 lei,
      ședința de cunoaștere gratuită, ~30 de minute.
- [ ] Teoriile citate au autor; statisticile au sursă, an și adresă.
- [ ] Nicio afirmație despre formare, acreditare sau apartenență profesională
      neconfirmată de Ana în scris.
- [ ] Trimiterile la Codul etic ICF verificate azi, în versiunea actuală de pe site-ul ICF —
      cu data verificării notată. *(Sau: nu există astfel de trimiteri.)*
- [ ] Marcajele `[DE COMPLETAT DE ANA: …]` sunt numărate și semnalate; niciunul rămas
      neintenționat într-un text propus spre publicare.

## B. Etică

- [ ] Niciun detaliu identificabil despre vreun client; exemplele sunt ipotetice sau
      compozite și marcate ca atare.
- [ ] Diferențierea coaching / terapie apare acolo unde ar putea exista confuzie.
- [ ] Nicio promisiune de vindecare, diagnostic sau rezultat garantat.
- [ ] Nicio etichetă clinică aplicată cititorului.
- [ ] Dacă tema atinge zona clinică sau de risc: trimiterea către specialistul potrivit
      este prezentă și vizibilă.
- [ ] Autonomia cititorului e respectată — nu i se spune ce „trebuie" să facă.
- [ ] Dacă materialul vizează adolescenți: comunicarea comercială merge către părinte;
      rolurile și confidențialitatea sunt clare; nicio promisiune despre comportamentul copilului.
- [ ] Nicio listă de persoane colectată, niciun contact nesolicitat pregătit.
- [ ] Dacă apare un mecanism nou de colectare a datelor: politica de confidențialitate
      acoperă situația, sau actualizarea ei e cerută explicit în cererea de aprobare.

## C. Voce și limbă

- [ ] Vocea se potrivește cu articolele existente (recitește un paragraf din `blog/`).
- [ ] Fără promisiuni exagerate, urgență artificială, frică, vinovăție, superlative.
- [ ] Fără jargon nedefinit și fără englezisme evitabile.
- [ ] **Diacritice complete**, peste tot: titlu, text, metadate, hashtag-uri, subtitrări,
      descrieri. Ș și Ț cu virgulă.
- [ ] Ghilimele românești „…"; cratimă lungă „—" pentru pauze.
- [ ] Genul gramatical e consecvent și potrivit audienței materialului.
- [ ] Text recitit cu voce tare — sună a om, nu a comunicat.

## D. Structură și utilitate

- [ ] Un singur subiect.
- [ ] Cititorul se recunoaște în primele trei fraze.
- [ ] Titlul promite exact ce livrează textul.
- [ ] Există o secțiune care nuanțează sau spune ce nu oferă coachingul.
- [ ] Cititorul pleacă cu un pas concret.
- [ ] Textul e util și pentru cineva care nu știe nimic despre coaching.
- [ ] Îndemnul la acțiune e unul singur, la final, blând.

## E. Tehnic (pentru site)

- [ ] `<html lang="ro">`; `<title>` de 50–60 de caractere + ` | Ana-Maria Brad`.
- [ ] `meta description` de 150–160 de caractere, cu diacritice.
- [ ] `canonical` și `hreflang="ro"` corecte și identice cu adresa reală.
- [ ] Toate `og:*` și `twitter:*` completate; `og:image` există la adresa indicată.
- [ ] JSON-LD `BlogPosting` și `BreadcrumbList` prezente, cu datele corecte.
- [ ] JSON-LD validat: `python3 -m json.tool` trece pe fiecare bloc.
- [ ] `datePublished` și `dateModified` corecte.
- [ ] Slug fără diacritice, cu cratime; nu se mai schimbă după publicare.
- [ ] CTA-ul final are `data-umami-event="calendly"` și `data-umami-event-loc="blog-<slug>-1"`.
- [ ] 2–4 legături interne, toate verificate că există.
- [ ] Cardul e adăugat în `blog/index.html`, în poziția stabilită de Ana.
- [ ] Intrarea e adăugată în `sitemap.xml` (`lastmod`, `priority` 0.7, `hreflang`).
- [ ] Antetul, navigația, bara de anunț și subsolul sunt identice cu ale celorlalte pagini.
- [ ] Pagina se deschide corect local și arată bine pe telefon.
- [ ] `git diff` verificat: **niciun fișier atins în afara celor aprobate**.

## F. Pentru rețele sociale

- [ ] Textul e gata de copiat, fără editări suplimentare.
- [ ] Formatul se potrivește canalului (lungime, hashtag-uri, legături).
- [ ] Instagram: trimiterea merge prin anamariabrad.ro/link (nu legături în descriere).
- [ ] LinkedIn: legătura e pregătită pentru primul comentariu, nu în corp.
- [ ] Imaginea sau clipul există și are formatul corect.
- [ ] Video: 30–60 s, vertical, **subtitrat**, subtitrarea corectată manual pentru diacritice.

## G. Pentru grupuri de Facebook

- [ ] Grupul e pe lista aprobată de Ana.
- [ ] Regulile grupului, citite azi.
- [ ] Au trecut cel puțin 7 zile de la ultima postare a Anei în acel grup.
- [ ] Postarea e utilă în sine, nativă, fără ofertă și fără legătură comercială.
- [ ] Se încheie cu o întrebare deschisă.
- [ ] Exemplele sunt anonimizate și compozite.
- [ ] Nu s-a colectat nicio listă de membri.
- [ ] Nu e același text folosit în alt grup.

## H. Pentru promovare plătită

- [ ] Bugetul, plafonul și criteriile de oprire sunt scrise explicit.
- [ ] Estimările sunt marcate ca estimări, cu ipotezele lor.
- [ ] Audiența nu e țintită pe criterii sensibile.
- [ ] Creațiile trec integral secțiunile A–D de mai sus.
- [ ] Destinația și eticheta UTM sunt stabilite.
- [ ] E clar că **Ana** pornește campania, nu agentul.

## I. Ultimul pas

- [ ] Cererea de aprobare e completată, cu materialul final atașat.
- [ ] Am scris ce nu am putut verifica.
- [ ] Am scris ce decizii îi rămân Anei.
- [ ] **Nu am publicat, nu am trimis, nu am pornit nimic.**
