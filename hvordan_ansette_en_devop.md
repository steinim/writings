# Hvordan ansette en DevOp?

Puristene hevder det ikke går an å være en DevOp, DevOps-utvikler, DevOps-drifter, DevOps-teknolog, DevOps-ingeniør eller lignende. [DevOps er ikke en jobb, det er en filosofi](http://www.midvision.com/resources-blog/bid/336536/There-s-no-such-thing-as-a-DevOps-Engineer). Vel og bra, men i og med at [jeg tror på denne filosofien](http://open.bekk.no/usrbizdevops) så ønsker jeg også å jobbe med mennesker som i likhet med meg ønsker å leve etter denne filosofien. Hvilke egenskaper skal jeg se etter?

---

Carlos Bueno i Facebook beskriver i artikkelen [full stack](https://www.facebook.com/note.php?note_id=461505383919) hva en full-stack utvikler er.

> A "full-stack programmer" is a generalist, someone who can create a non-trivial application by themselves.

Facebook skal vistnok ha ansatt *kun* denne typen utviklere i en periode. Hva en full-stack utvikler er har siden vært diskutert i et antall bloggposter og forum. De fleste hevder at dette er enhjørninger. Laurence Gellert har laget en [liste over hva en slik utvikler må kunne](http://www.laurencegellert.com/2012/08/what-is-a-full-stack-developer/), men den er neppe uttømmende om man skal ta hele stacken i betraktning. Generalister som har bred ekspertise i hele stacken og som enkelt kan sette seg inn i nye ting er definitivt verdifulle, men det er ikke denne typen teknologer jeg ser etter. Jeg har mye større tro på riktig sammensetning av mennesker som utfyller hverandre i kryssfunksjonelle team.

En god defnisjon av DevOps kommer fra Jez Humble via en [bloggpost](http://theagileadmin.com/what-is-devops/) skrevet av en gruppe mennesker under pseudonymet The Agile Admin.

> a cross-disciplinary community of practice dedicated to the study of building, evolving and operating rapidly-changing resilient systems at scale

Denne definisjonen forteller meg at det handler om å se etter folk som mestrer praksiser som bidrar til å kunne bygge, viderutvikle og drifte fleksible systemer i stor skala fort. Den forteller meg også at det er en kryssfunksjonell disiplin. Vi ser ikke etter *en* type mennesker, men heller folk med ulike egenskaper som utfyller hverandre.

Ser jeg da etter "tradisjonelle" driftere og utviklere som samarbeider om å lage systemene? Jeg tror ikke det. De kan gjerne ha jobbet som det, men kompetansen som kreves for å jobbe etter DevOps-filosofien har endret seg betydelig. I kjølvannet av DevOps-bevegelsen har det oppstått en rekke nye praksiser og verktøy som endrer måten vi bygger, viderutvikler og drifter fleksible systemer i stor skala.

De fleste endringene er knyttet til hvordan vi drifter systemene vi lager. Drift har blitt en disiplin som har tatt til seg mange av de samme teknikkene utviklere bruker. Eksempler er versjonskontroll, kontinuerlig integrasjon og automatisering av bygg, testing og utrulling. I tillegg kreves kompetanse om ting som monitorering utover ressursutnyttelse, nettverk, virtualisering og sannsynligvis nettsky. Det er nødvendig at "tradisjonelle" utviklere lærer seg mer om drift, men enda viktigere er det at det er personer på teamet som *virkelig* kan drift på den "nye måten". Det er denne typen mennesker jeg ser etter. Hva må de så kunne? Her er min liste.

## 1. Basis driftskompetanse
Kompetanse om basisdrift er fremdeles viktig selv om engangsinfrastruktur (engelsk: immutable infrastructure), containere og skyinfrastruktur blir normen. Fornuftig bruk av filsystemer, os, lagring, nettverk, brannvegger, backup, patching, databaser, virtualisering og feilsøking er nødvendig kompetanse å ha på et team som har ansvar for hele stacken.

## 2. Utvikler-skills
Som nevnt over har moderne drift utvidet sin verktøykasse med verktøy og teknikker vi kjenner igjen fra utviklerverdenen. Automatisert testing, kontinuerlig integrasjon, bygging, utrulling, konfigurasjon og dokumentasjon som kode og versjonskontroll er alle eksempler på dette. Man må kunne anvende disse også for infrastruktur.

## 3. Infrastruktur som kode
Oppsett av infrastruktur fra hardware og opp skal være automatisert, definert i programkode og versjonskontrollert. Det er mange provisjoneringsrammeverk å [velge mellom](https://open.bekk.no/choosing-a-provisioning-framework).

## 4. Skripting/Programmering 
Man må kunne skrive kode for å automatisere gjentakende oppgaver. Det holder ikke med skript som kjører lokalt på servere eller over ssh. Man må også kunne kode mot RESTful APIer. GUI-konfigurasjon er ut.

## 5. Offentlig Nettsky
Erfaring med offentlig nettsky er essensielt. Virtualisering av servere med VMware eller lignende er ikke tilstrekkelig (selv om det er viktig å forstå hvordan virtualisering fungerer). Erfaring med privat nettsky er heller ikke nok. Josh Stella sin bloggpost [Minimum Viable Cloud](https://blog.fugue.co/2014-08-11-minimum_viable_cloud.html) beskriver forskjellene godt. Offentlig nettsky er [i ferd med å bli industristandard](http://open.bekk.no/hvem-kan-konkurrere-med-amazon-web-services) og det blir dermed viktig å ha denne typen kompetanse.

## 6. Smidige metoder
DevOps-filosofien er kraftig inspirert av [Smidig](http://www.agilemanifesto.org/iso/no/) og [Lean](https://en.wikipedia.org/wiki/Lean_IT). Evnen til å jobbe innenfor organisasjoner som har adoptert disse metodologiene må således være på plass.

## 7. Soft-skills
Jobber man Smidig er samarbeid med personer med andre roller veldig viktig. Tett kontakt med reelle brukere likeså. Samarbeid med forretningsfolk, UX-eksperter, selgere, markedsfolk, andre utviklere og mange fler krever at man må kunne kommunisere godt og samarbeide med disse på daglig basis.

# Oppsummert
Det kan kanskje virke som om dette er alt for mye å be om. Det tror jeg ikke om man sammenligner det med hva andre teknologer generelt kan. Om du ber en utvikler eller drifter om å sette seg ned og skrive om alt hun kan, så vil hun sitte lenge. Listen med hva man bør kunne er ikke en sammenslåing av alt utviklere kan og alt driftere kan. Vi snakker om en ny type teknolog som kan mye om det beste fra to verdener. Det er dessuten slik at at man jobber i kryssfunksjonelle team hvor det finnes flere spesialister som har spisskompetanse på ulike områder som utfyller hverandre. Teknologen jeg ser etter har spisskompetansen jeg har beskrevet i denne bloggposten.


Og by the way. [BEKK ser etter mennesker med disse egenskapene](link til jobbannonse).

---
[Forsidebilde](https://www.flickr.com/photos/lovelornpoets/6034634225) av [Lovelorn Poets](http://www.lovelornpoets.com/) er lisensiert under CC BY 2.0 og modifisert av forfatteren av bloggposten.
