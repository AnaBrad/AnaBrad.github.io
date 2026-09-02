# Contradicții între materialele existente și cerințele agentului

Constatate la **2 septembrie 2026**, prin citirea materialelor din depozit.

**Niciuna nu a fost rezolvată și niciun material existent nu a fost modificat.** Fiecare
are nevoie de o decizie a Anei. Până atunci, agentul lucrează cu regula scrisă la fiecare
punct și **nu presupune** nimic.

Când o contradicție se rezolvă, se notează aici decizia și data, apoi se actualizează
fișierele din `context/`.

---

## C1. Site-ul se adresează exclusiv femeilor; briefingul cere femei, bărbați și adolescenți

**Ce spun materialele.** Poziționarea „pentru femei" e peste tot, nu doar în titlu:

- `index.html`: `<title>` „coaching pentru femei care își doresc mai mult de la viață";
  `<h1>` + subtitlu identice; JSON-LD `ProfessionalService`: „Coaching individual pentru
  femei…"; „Ofer câteva locuri pentru **clientele** care vor să înceapă acum";
  „să însoțesc **femeile** care aleg să își regăsească vocea".
- Subsolul de pe fiecare pagină: „Coaching pentru femei aflate la un moment decisiv" /
  „Coaching pentru femei · online și în Iași".
- `link/index.html`: „Coaching pentru femei într-un moment de schimbare."
- Secțiunea de testimoniale: „Ce spun **clientele**".
- Acorduri la feminin în tot textul („pierdută", „singură", „redirecționată").

**Ce cere briefingul.** Serviciu: coaching general pentru adulți în tranziție.
Audiență: femei, bărbați și adolescenți.

**De ce contează.** Conținutul pentru bărbați sau pentru părinți de adolescenți ar duce
oamenii pe un site care le spune, din primul rând, că nu e pentru ei. Se pierde și
efortul, și încrederea.

**Regula până la decizie.** Se produce conținut pentru toate audiențele, dar:
materialele adresate bărbaților sau publicului mixt se scriu neutru ca gen și **nu se
publică pe canale care trimit către paginile actuale**, până când Ana decide. Nu se
modifică niciun text existent.

**Ce decide Ana.**
- (a) Rămâne poziționarea „pentru femei" și celelalte audiențe se servesc doar prin
  instrumente și articole, fără campanii; sau
- (b) Se lărgește poziționarea — ceea ce înseamnă rescrierea paginii principale, a
  subsolurilor, a paginii de linkuri și a metadatelor; sau
- (c) Se creează pagini separate pe audiență, păstrând pagina principală așa cum e.

---

## C2. Bara de anunț și prețul special sunt legate de o dată deja trecută

**Ce spun materialele.** Bara de anunț de pe fiecare pagină: „Se lansează pe 1 septembrie
2026". Pe pagina principală: „Preț special pentru clientele care încep programul la
1 septembrie 2026." Formularul Tally e prezentat ca listă de așteptare („Vrei să te mai
gândești? Lasă-mi datele și îți rezerv eu un loc"), iar politica de confidențialitate
descrie tot o listă de așteptare, „ca să te anunț când se deschid înscrierile".

**Situația.** Astăzi e 2 septembrie 2026. Lansarea s-a produs.

**De ce contează.** Un vizitator citește „se lansează" la trecut și nu știe dacă oferta e
activă; nu e clar dacă prețul special mai e valabil; lista de așteptare nu mai are obiect
dacă înscrierile sunt deschise. Orice campanie ar amplifica această confuzie.

**Regula până la decizie.** Nu se face nicio campanie plătită și nicio distribuire
susținută către pagina principală până când mesajul nu e clarificat. Textele noi nu
repetă „se lansează".

**Ce decide Ana.** Ce înlocuiește bara de anunț; dacă prețul special rămâne și până când;
dacă formularul Tally rămâne listă de așteptare sau devine altceva.

---

## C3. Adolescenții au instrumente, dar nu au ofertă și nu au pagină pentru părinți

**Ce spun materialele.** Există 9 instrumente pentru adolescenți și o secțiune despre
adolescenți în articolul „Cât costă coaching-ul". Nu există: o ofertă pentru adolescenți,
un preț, o pagină pentru părinți, o descriere a cadrului (rolurile, ce rămâne confidențial,
cum se implică părintele).

**Ce cere briefingul.** Adolescenții sunt audiență, iar comunicarea către părinți se
tratează distinct. Grupul-pilot aprobat, „Părinți pe sârmă", este exact un grup de părinți.

**De ce contează.** Traseul „postare utilă în grup → resursă → conversație → ședință de
cunoaștere" duce către o destinație care nu există. Un părinte interesat ajunge pe un site
despre coaching pentru femei adulte.

**Regula până la decizie.** Se pregătește conținut util pentru părinți (fără ofertă),
dar nu se promite un serviciu pentru adolescenți și nu se comunică vreun preț pentru el.

**Ce decide Ana.** Dacă există serviciu pentru adolescenți; ce preț și ce format are;
dacă apare o pagină pentru părinți; cum se descrie cadrul.

---

## C4. Traseul din grupuri presupune un ghid care nu există

**Ce spun materialele.** Nicăieri pe site nu există un ghid, o resursă descărcabilă sau
un mecanism de livrare a uneia. Există doar instrumentele interactive (care rulează local,
în browser) și formularul Tally pentru lista de așteptare.

**Ce cere briefingul.** Traseul e „postare utilă → **resursă** → conversație reală →
invitație → ședință", iar după trimiterea ghidului se pune întrebarea „Care dintre
situațiile din ghid îți este cea mai familiară?".

**De ce contează.** Fără ghid, traseul nu poate fi parcurs. Iar felul în care e livrat
schimbă obligațiile legale: un fișier trimis direct într-o conversație e altceva decât un
formular care colectează adrese de e-mail — al doilea cere actualizarea politicii de
confidențialitate **înainte** de lansare și consimțământ separat pentru orice altă
folosire a adresei.

**Regula până la decizie.** Nu se promite niciun ghid în conținut și nu se construiește
niciun mecanism de colectare a adreselor.

**Ce decide Ana.** Dacă se face ghidul, pe ce temă, pentru care audiență, în ce format,
cum se livrează, și dacă politica de confidențialitate trebuie actualizată.

---

## C5. `sitemap.xml` e incomplet și învechit

**Ce spun materialele.** `sitemap.xml` conține 2 din cele 9 articole de blog
(`cum-am-ajuns-sa-creez-spatiul` și `motivatie-care-dureaza`), toate cu `lastmod`
2026-07-19. Lipsesc 7 articole, între care cele mai recente și cele mai potrivite pentru
căutare: `cat-costa-coaching`, `prima-sedinta-de-cunoastere`, `ce-e-coaching`,
`5-semne-moment-decisiv`, `cum-sa-spun-nu-nevoi-sociale`, `fereastra-de-toleranta`,
`cand-valorile-personale-intra-in-conflict`.

**De ce contează.** Sunt exact articolele care ar trebui să aducă trafic din căutare.
E cea mai ieftină îmbunătățire disponibilă azi.

**Regula până la decizie.** Fișierul **nu a fost modificat** — e material existent, iar
modificarea lui înseamnă publicare. Se propune ca acțiune separată.

**Ce decide Ana.** Dacă aprobă completarea `sitemap.xml` cu cele 7 articole lipsă.

---

## C6. Nu există convenție de măsurare pentru sursele de trafic

**Ce spun materialele.** Umami e instalat, cu evenimente pentru `calendly` și pentru
contacte. Nu există etichete UTM și nicio convenție pentru ele. Legăturile din postări
ar ajunge nediferențiate în statistici.

**De ce contează.** Fără ele nu se poate răspunde la întrebarea „de unde au venit
ședințele de cunoaștere?", iar analiza săptămânală rămâne o listă de cifre fără cauze.
Fără această convenție nu are sens nicio campanie plătită.

**Regula până la decizie.** Se propune o convenție simplă (`utm_source`, `utm_medium`,
`utm_campaign`) înainte de prima distribuire susținută, ca decizie separată a Anei.

---

## C7. Ritmul editorial cerut e mai rapid decât ritmul de până acum

**Ce spun materialele.** 9 articole publicate; ultimele două, pe 31 august 2026.
**Ce cere briefingul.** Un articol pe săptămână.

**De ce contează.** E realizabil, dar numai dacă schițele vin gata și Ana rămâne cu
revizuirea. Bugetul de timp din `plan/plan-editorial-curent.md` pleacă de la asta.

**Regula.** Dacă într-o săptămână calitatea ar avea de suferit, se propune sărirea
articolului, nu publicarea unuia slab. Se semnalează din timp, nu în ziua publicării.

---

## C8. Detalii mai mici, de confirmat

- **LinkedIn** — există doar profil personal, nu pagină de companie. Postările sunt
  personale, la persoana I. De confirmat că așa rămâne.
- **Blog în engleză** — a fost eliminat; `blog/en/` și `instrumente-coaching/en/` sunt
  redirecționări. Două pagini din `instrumente-coaching/en/` (WOOP, OSKAR) există încă.
  De confirmat că engleza rămâne închisă.
- **Stripe** — apare în politica de confidențialitate ca procesator de plăți, dar nu are
  niciun buton pe site. De confirmat cum se încasează, de fapt.
- **„coaching-ul" vs. „coachingul"** — ambele forme apar în materiale. De ales una pentru
  textele noi (regula actuală: se păstrează forma din pagina pe care o completezi).
