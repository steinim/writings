<!--
# Fra prosjekt til produkt

Et prosjekt er en arbeidsform som er avgrenset fra de aktivitetene en organisasjon vanligvis gjennomfører. Det er avgrenset i tid og har et mål for hva man vil ha oppnådd når prosjektperioden er over. Typisk etableres det som en midlertidig organisasjon med personer som enten skal ut eller tilbake til linja. Formålet er å styrke virksomhetens evne til suksess i tiden som kommer. Det er arbeidsformen dessverre lite egnet til.
-->

Det er flere årsaker til at prosjekter er lite egnet som arbeidsform. Eksempler er at det er vanskelig å måle realisering av gevinst, konflikt mellom prosjektets mål og virksomhetens mål, silo-tankegang, stor avstand mellom prosjekt- og linjeorganisasjon, en kortsiktig finansieringsmodell, manglende kommunikasjon og utfordringer med overlevering og kunnskapsoverføring.  

Alternativet er å behandle leveransene som kontinuerlige produktutviklingsløp i linja. Det vil da være enklere å måle gevinster kontinuerlig, justere initiativene opp mot virksomhetens mål, tettere samarbeid, nedbryting av siloer, løpende finansiering, bedre kommunikasjon og kunnskapsbygging istedenfor kunnskapsoverlevering.

## "You Build It, You Run It"
Prosjektmedlemmer er avgrenset fra linjeorganisasjonen, og deres involvering med produktene de lager er tidsbegrenset. De slipper å leve med de langsiktige resultatene av deres egne arkitektur- og designbeslutninger. Linjeorganisasjonen er som regel underbemannet og har knappe ressurser og liten evne til å håndtere overleveringer fra prosjekter. De må dessuten administrere, overvåke og supportere eksisterende IT-systemer. Dette medfører som regel dårligere utviklingspraksiser og gradvis forverret kvalitet. Dette forsterkes ofte av at man har dårlig tid i prosjekter. Prosjektmedlemmene er som regel skjermet fra analyse og gjenoppretting ved produksjonsproblemer. De tvinges ikke til å legge inn nødvendig overvåkning og nødvendig logging for analyse av rot-årsaker. Teamet gjør ofte et begrenset antall produksjonssettinger og har derfor få insentiver til å investere i automatisering og produksjonslike miljøer.

I Amazon.com, hvor de fokuserer på produkter fremfor prosjekter, er det et viktig prinsipp at de som lager systemene også skal drifte systemene og leve med dem i lang tid. Helt til de dør. "You Build It, You Run It" - Werner Vogels (CTO Amazon). I Amazon.com har de ikke egne driftsteam. Teamet håndterer både drift og utvikling. Det er dette som kalles DevOps. Da Kent Bekk besøkte DevOps Norway Meetup ble han bedt om å definere hva han legger i begrepet DevOps. Hans umiddelbare svar var: "Developers carry beepers". Når utviklingsteamet får ansvar for å ha beredskap selv, er insentivene på plass for å lage skikkelig driftbare produkter. Forvaltning og drift flyttes til starten av utviklingsløpet. Teamet organiseres som en forvaltningsorganisasjon fra dag én.

## Feature teams vs. Component teams
Når man setter sammen langlevde team rundt produkter som understøtter forretningen forsterkes forståelsen og ansvarsfølelsen for forretningens visjon. Teamene vet hvor man vil med produktene som lages og eierskapet, ansvarsfølelsen og stoltheten styrkes. Produktene man lager bør ha sitt opphav i et ønske om å realisere noe verdifullt for virksomheten. Derfor bør det ikke fokuseres på systemer (components), men på funksjoner (features). Dersom man tar utgangspunkt i å lage en ny funksjon, og denne skal lages i et bestemt system, så har man allerede lagt unødvendige begrensninger for hvordan funksjonen kan realiseres. Å fordele oppgaver basert på team som har ansvar for et bestemt system (component) vil som regel medføre at teamet med ansvar for komponenten implementerer funksjonen i sitt eget system som de kjenner godt. At funksjonen bedre kan implementeres i et annet system eller på tvers av flere systemer forsvinner fort med et navlebeskuende fokus. Om man organiserer teamene rundt funksjoner eller forretningsområder, slik det gjøres i for eksempel Spotify, vil systemarkitekturen automatisk speile forretningen bedre. Conway's lov fra 1968 sier at strukturen på IT-systemene speiler organisasjonens struktur. For å oppnå systemer som speiler forretningsstrukturen må man derfor la team organisere seg rundt funksjoner og ikke systemer.

## DevOps, Kontinuerlige Leveranser og Sky

Det blir vanskeligere og vanskeligere å se at denne klassiske prosjektmodellen er godt egnet for IT-leveranser som innebærer et stykke skreddersøm. Over tid tror vi denne gjennomføringsmodellen vil forsvinne. MVP-/Lean Startup-tankegang, i kombinasjon med No-/DevOp'sy applikasjonsdrift, flytter forvaltningsfasen til starten av utviklingsløpet. Det er derfor enklere å betrakte leveranseteamet som en forvaltningsorganisasjon fra dag én, og heller håndtere prosjektaktige problemstillinger som spesialtilfeller.

## Kill all the unnecessary roles


## Smart budgeting
This approach is not easy – it introduces new challenges particularly around balancing priorities and budgeting. I’ve observed that the benefits in terms of long term system health definitely outweigh the drawbacks. Like everything – hire good people who care, and give them the right incentives, good things will happen.

## Oppsummering

Dersom man skal begynne på nye ting anbefaler vi å ikke gjennomføre disse endringene som et prosjekt, men heller se på de alternative gjennomføringsmodellene nevnt over. Vi anbefaler å fase ut den klassiske prosjektorganisasjonen og erstatte denne med flere, mindre enheter med større autonomi. Fokuset bør være på å starte i det små og levere kontinuerlige forbedringer gradvis, og å etablere en voksende organisasjon gradvis - ut fra erfarte behov. 



