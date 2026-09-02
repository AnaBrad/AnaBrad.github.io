# Copilot de marketing digital — mod de utilizare

Aici locuiește agentul de marketing al Anei-Maria Brad: instrucțiunile lui, contextul de
lucru, procedurile, șabloanele și materialele pe care le produce.

**Agentul este un copilot, nu un agent autonom.** Cercetează, analizează, propune și
pregătește. Nu publică, nu trimite mesaje, nu pornește campanii. Fiecare acțiune cu efect
public are nevoie de aprobarea explicită a Anei.

---

## Cum îl pornești

Agentul e definit în `.claude/agents/marketing-digital.md` și e disponibil în Claude Code
din acest depozit. Îl chemi cerându-i, pur și simplu, ce ai nevoie:

```
Folosește agentul marketing-digital ca să pregătești articolul săptămânii despre etica în coaching.
```
```
marketing-digital: fă analiza săptămânii trecute. Datele din Umami și Calendly sunt aici: …
```
```
marketing-digital: pregătește o postare pentru „Părinți pe sârmă", pe tema …
```

Merge și fără să-l numești, dacă ceri limpede o sarcină de marketing.

## Ce îi dai la început

Agentul nu are acces la Umami, Calendly, Tally sau la conturile de rețele. Când ai nevoie
de analiză, dă-i datele — copiate ca text e suficient. Când lipsesc, o scrie ca atare;
nu inventează cifre.

## Ce primești înapoi

Un fișier în `drafturi/`, plus un rezumat în conversație: ce a făcut, ce decizii îți
rămân, ce nu a putut verifica. Dacă urmează o acțiune externă, primești și o **cerere de
aprobare** — și agentul se oprește acolo.

---

## Structura

```
.claude/
├── agents/
│   └── marketing-digital.md        instrucțiunile agentului (fișierul principal)
└── marketing/
    ├── README.md                   acest fișier
    ├── CONTRADICTII-DE-CLARIFICAT.md   ce contrazice ce, și ce aștepți să decizi
    ├── context/
    │   ├── profil-oferta-audiente.md
    │   ├── voce-si-limbaj.md
    │   ├── etica-si-limite.md
    │   └── canale-si-conventii-tehnice.md
    ├── playbooks/
    │   ├── strategie-si-planificare.md
    │   ├── cercetare.md
    │   ├── continut-blog.md
    │   ├── continut-social.md
    │   ├── video-scurt.md
    │   ├── pregatire-publicare.md
    │   ├── promovare-platita.md
    │   ├── conversatii-si-potentiali-clienti.md
    │   ├── analiza-saptamanala.md
    │   └── comunitati-facebook.md
    ├── sabloane/
    │   ├── raport-saptamanal.md
    │   ├── cerere-aprobare.md
    │   └── checklist-inainte-de-publicare.md
    ├── plan/
    │   └── plan-editorial-curent.md
    ├── drafturi/                   materiale în lucru
    ├── aprobari/                   cereri de aprobare + răspunsurile tale
    └── rapoarte/                   rapoarte săptămânale
```

## Cum se numesc fișierele

| Unde | Formă | Exemplu |
| --- | --- | --- |
| `drafturi/` | `AAAA-LL-ZZ-<tip>-<subiect>.md` | `2026-09-09-blog-etica-in-coaching.md` |
| `aprobari/` | `AAAA-LL-ZZ-<subiect>.md` | `2026-09-16-publicare-etica-in-coaching.md` |
| `rapoarte/` | `AAAA-SS.md` (an, săptămână ISO) | `2026-37.md` |

Tipuri folosite în `drafturi/`: `blog`, `social`, `video`, `grup`, `cercetare`, `campanie`,
`conversatii`.

---

## Ce nu face niciodată fără aprobarea ta

1. Publicare pe site (fișiere HTML, `blog/index.html`, `sitemap.xml`, orice pagină).
2. Publicare pe Facebook, Instagram, LinkedIn sau oriunde altundeva.
3. Mesaje private, comentarii, cereri de conectare, orice contactare a unei persoane.
4. Postări sau comentarii în grupuri, inclusiv în cele aprobate.
5. Pornirea, oprirea sau modificarea promovării plătite și a bugetelor.
6. Orice altă schimbare cu efect public sau extern.

Agentul scrie fișiere **doar** sub `.claude/marketing/`. Fișierele site-ului le citește,
dar nu le atinge decât după o aprobare explicită, dată în acea conversație, pentru acel
material. O aprobare nu se transferă la data următoare.

## Cum aprobi

Agentul îți dă un fișier în `aprobari/`, completat, cu materialul final atașat. Tu
completezi secțiunea „Răspunsul Anei": aprobi, aprobi cu modificări, amâni sau refuzi.
Agentul execută **exact** ce ai aprobat, nimic în plus.

Poți răspunde și scurt, în conversație („aprob publicarea articolului X exact așa cum e"),
dar dosarul din `aprobari/` rămâne urma scrisă a ce s-a hotărât.

---

## Ritmul săptămânal propus

| Zi | Ce faci tu | Ce face agentul |
| --- | --- | --- |
| Luni | îi dai datele săptămânii, validezi calendarul | raport săptămânal + calendar |
| Marți | revizuiești și aprobi articolul | schița articolului, gata de revizuit |
| Miercuri | publici articolul și îl distribui | pachetul de distribuire, gata de copiat |
| Joi | filmezi în lot | scenarii, text pe ecran, subtitrări, descrieri |
| Vineri | răspunzi în comunitate | propuneri de răspunsuri și trasee de conversație |

Aproximativ 4–5 ore pe săptămână din cele ~40.

## Înainte de orice publicare

Se parcurge `sabloane/checklist-inainte-de-publicare.md`, integral. Rezultatul se atașează
la cererea de aprobare.

## Primul lucru de făcut

Citește `CONTRADICTII-DE-CLARIFICAT.md`. Sunt opt puncte în care materialele de pe site
și cerințele de marketing nu se potrivesc. Nimic nu a fost schimbat; toate așteaptă
decizia ta. Cele mai importante: poziționarea site-ului (C1), bara de anunț rămasă la
„se lansează pe 1 septembrie" (C2) și ghidul care lipsește din traseul din grupuri (C4).

---

## De ce stă totul sub `.claude/`

GitHub Pages publică rădăcina depozitului. Un folder obișnuit numit `marketing/` ar
deveni public la `anamariabrad.ro/marketing/`. Folderele care încep cu punct sunt ignorate
de Jekyll, procesarea implicită a GitHub Pages (depozitul nu are un fișier `.nojekyll`).
Așa, materialele de lucru sunt versionate în git, dar rămân private.
**Nu muta aceste fișiere în rădăcina depozitului.**
