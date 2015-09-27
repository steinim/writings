<!--
# Slutt med IT-prosjekter!

[De store IT-prosjektenes tid er kanskje forbi](http://www.cw.no/artikkel/tiden-store-it-anskaffelser-over), men hva med de "små"? Selv "smidige" prosjekter forventes å bli ferdige på en eller annen dato i fremtiden, og når systemet er levert, skal det overleveres til linja. Er det virkelig størrelsen som er problemet, eller er det selve arbeidsformen som ikke fungerer? 

-->

Et prosjekt er en arbeidsform som er avgrenset fra de aktivitetene en organisasjon vanligvis gjennomfører. Det er avgrenset i tid og har et mål for hva man vil ha oppnådd når prosjektperioden er over. Typisk etableres det som en midlertidig organisasjon med personer som enten skal ut, eller tilbake til linja. Formålet er å styrke virksomhetens evne til suksess i tiden som kommer. Det er arbeidsformen dessverre lite egnet til.

Det er flere årsaker til at prosjekt som arbeidsform er lite egnet. Eksempler er at det er vanskelig å måle realisering av gevinst, konflikt mellom prosjektets mål og virksomhetens mål, silo-tankegang, stor avstand mellom prosjekt- og linjeorganisasjon, en kortsiktig finansieringsmodell, manglende kommunikasjon og utfordringer med overlevering og kunnskapsoverføring.  

Alternativet er å behandle leveransene som kontinuerlige produktutviklingsløp i linja. Det vil da være enklere å måle gevinster kontinuerlig, justere initiativene opp mot virksomhetens mål, tettere samarbeid, nedbryting av siloer, løpende finansiering, bedre kommunikasjon og kunnskapsbygging istedenfor kunnskapsoverlevering.

## "You Build It, You Run It"
Prosjektmedlemmer er avgrenset fra linjeorganisasjonen, og deres involvering med produktene de lager er tidsbegrenset. De slipper å leve med de langsiktige resultatene av deres egne arkitektur- og designbeslutninger. Linjeorganisasjonen er som regel underbemannet og har knappe ressurser og liten evne til å håndtere overleveringer fra prosjekter. De må dessuten administrere, overvåke og supportere eksisterende IT-systemer. Dette medfører som regel dårligere utviklingspraksiser og gradvis forverret kvalitet. Dette forsterkes ytterligere av at man som regel har dårlig tid i prosjekter. Prosjektmedlemmene er som regel skjermet fra analyse og gjenoppretting ved produksjonsproblemer. De tvinges ikke til å legge inn nødvendig overvåkning og nødvendig logging for analyse av rot-årsaker. Teamet gjør ofte et begrenset antall produksjonssettinger og har derfor få insentiver til å investere i automatisering og produksjonslike miljøer.

I Amazon.com, hvor de fokuserer på produkter fremfor prosjekter, er det et viktig prinsipp at de som lager systemene også skal drifte systemene og leve med dem i lang tid. Helt til de dør. "You Build It, You Run It" som Werner Vogels (CTO i Amazon) sier. I Amazon.com har de ikke egne driftsteam. Teamene håndterer selv både drift og utvikling. Det er dette som kalles DevOps.

Da Kent Bekk besøkte DevOps Norway Meetup for et par år siden ble han bedt om å definere hva han legger i begrepet DevOps. Hans svar var: "Developers carry beepers". Når utviklingsteamet får ansvar for å ha beredskap selv, er insentivene på plass for å lage virkelig driftbare systemer. Forvaltning og drift flyttes til starten av utviklingsløpet. Teamet organiseres som en forvaltningsorganisasjon fra dag én.

## Lag funksjoner, ikke systemer
IT-prosjekter har som regel en målsetning om å lage et IT-system som skal løse noen opplevde behov. Disse opplevde behovene formuleres som krav det nye IT-systemet skal støtte. Det nye IT-systemet får gjerne et navn og skal inneholde slik og slik sånn at vi får til slik og slik. Alternativt bestemmer man seg for å implementere den nye funksjonaliteten i et eksisterende system ved å utvide det. Problemet med dette er at det fokuseres mer på systemer (components) og mindre på funksjoner (features).

Dersom man tar utgangspunkt i å lage en ny funksjon, og denne skal lages i et bestemt system, så har man allerede lagt unødvendige begrensninger for hvordan funksjonen kan realiseres. Å fordele oppgaver basert på team som har ansvar for et bestemt system (component) vil som regel medføre at teamet med ansvar for komponenten implementerer funksjonen i sitt eget system som de kjenner godt. At funksjonen bedre kan implementeres i et annet system eller på tvers av flere systemer forsvinner fort med et slikt navlebeskuende fokus. Om man organiserer teamene rundt funksjoner eller forretningsområder, slik det gjøres i for eksempel Spotify, vil systemarkitekturen automatisk speile forretningen bedre. I henhold til Conway's lov fra 1968 så vil strukturen på IT-systemene speile organisasjonens struktur. For å oppnå systemer som speiler forretningsstrukturen må man derfor la team organisere seg rundt funksjoner og ikke systemer.

Når man setter sammen langlevde team rundt funksjoner som understøtter forretningen, så forsterkes forståelsen og ansvarsfølelsen for forretningens visjon. Teamene vet hvor man vil med produktene som lages, og eierskapet, ansvarsfølelsen og stoltheten styrkes. Produktene man lager bør ha sitt opphav i et ønske om å realisere noe verdifullt for virksomheten. Derfor bør det ikke fokuseres på systemer (components), men på funksjoner (features).

## DevOps, Kontinuerlige Leveranser og Sky
Når teamet har ansvaret for hele livssyklusen til systemene de lager, og de forstår og deler forretningens visjon og målsetninger, så finner de måter å jobbe på som ivaretar alle ønskelige aspekter ved produktutvikling. De etablerer en produktutviklingsprosess som støtter rask flyt, slik at veien fra konsept til ferdige funksjoner i produksjon blir så kort som overhodet mulig. Samtidig sikrer de at det ikke går på bekostning av kvalitet, tilgjengelighet, stabilitet, sikkerhet og så videre.

Denne måten å jobbe på er ikke som Smidig i tradisjonell forstand. Smidig impliserer ikke kontinuerlig. I tradisjonell Smidig jobber man som regel med batcher og iterasjoner, med mer planlegging og testing/akseptanse mot slutten av iterasjonene. Kontinuerlige Leveranser innebærer at programvaren kan produksjonssettes til enhver tid. Siste versjon av kildekoden kan slippes i produksjon når som helst uten behov for forberedelser eller tilpasninger.

DevOps og Kontinuerlige Leveranser er som hånd i hanske. De tradisjonelle overleveringene fra utvikling til drift forhindrer kontinuerlige leveranser, så produktteamene må drifte løsningen selv for å være i stand til å jobbe på denne måten. Dette fordrer bredere og en annen type kompetanse enn de fleste utviklingsteam besitter i dag. Det fordrer kompetanse om drift og utvikling, men det er ikke samme type kompetanse om utvikling og drift som man har hatt tidligere. Måten systemene driftes og utvikles på har endret seg mye. 

## Kill all the unnecessary roles
På JavaZone i 2014 holdt jeg et foredrag om alle de unødvendige rollene som eksisterer innen IT, særlig i IT-prosjekter, "[Kill 'Em All – and the ultimate developer will rise again!](https://vimeo.com/105761144)". 

## Fra CapEx til OpEx
CapEx (Capital expenditures) er investeringer man gjør på forhånd for å skape fremtidige gevinster. OpEx (Operational expenditure) er investeringer som gjøres underveis mens forretningen forløper som normalt. Skydrift er et eksmepl på en pay-as-you-go finansieringsmodell hvor elastisiteten og fleksibiliteten gjør at du kan skalere opp eller ned underveis istedenfor å investere masse penger i egen infrastruktur og overkapasitet før du trenger den. Jeg snakker her selvsagt om offentlig sky og ikke privat.

IT-prosjekter er investeringer som betales på forhånd. De har budsjetter. De har risiko. Det er bra å investere i IT, men disse investeringene behøver ikke nødvendigvis å gjøres på forhånd. Når utvikling av funksjoner følger resten av virksomheten tett, vil det være mer fornuftig å smøre kostnadene tynnere utover i organisasjonen. Det betyr ikke at man ikke kan satse stort på et område som koster mye, men som gir stor gevinst tilbake. Forskjellen er at risiko reduseres dramatisk om man tar en gradvis tilnærming til en potensielt dyr, men innbringende satsning. Gjennom å finansiere eksperimenter og gi de mest lovende initiativene mer penger når de trenger det, og de mindre lovende mindre eller ingenting, sikrer man en utvikling som er tettere knyttet opp mot forretningens mål enn gjetning på et alt for tidlig tidspunkt. Hensikten med å eksperimentere mer er å unngå å bli fanget i et blindspor. Om en satsning viser seg å bli innbringende kan man finansiere ytterligere for å maksimere uttak av gevinster.

Denne tilnærmingen er ikke nødvendigvis så enkel – det kan være vanskelig å balansere prioriteringer og budsjettering. Det krever at IT-utvikling blir en integrert del av forretningsutvikling og at resultater og hypoteser verifiseres kontinuerlig. Her gjelder det å innse at alle virksomheter i dag er IT-virksomheter og at det er en dårlig idé å ha et skille mellom IT og forretning om man skal lykkes.

## Det skalerer
Se de største: Netflix, Google, Amazon, Facebook,...


## Oppsummering

Det blir vanskeligere og vanskeligere å se at denne klassiske prosjektmodellen er godt egnet for IT-leveranser som innebærer et stykke skreddersøm. Over tid tror vi denne gjennomføringsmodellen vil forsvinne. MVP-/Lean Startup-tankegang, i kombinasjon med No-/DevOp'sy applikasjonsdrift, flytter forvaltningsfasen til starten av utviklingsløpet. Det er derfor enklere å betrakte leveranseteamet som en forvaltningsorganisasjon fra dag én, og heller håndtere prosjektaktige problemstillinger som spesialtilfeller.

Dersom man skal begynne på nye ting anbefaler vi å ikke gjennomføre disse endringene som et prosjekt, men heller se på de alternative gjennomføringsmodellene nevnt over. Vi anbefaler å fase ut den klassiske prosjektorganisasjonen og erstatte denne med flere, mindre enheter med større autonomi. Fokuset bør være på å starte i det små og levere kontinuerlige forbedringer gradvis, og å etablere en voksende organisasjon gradvis - ut fra erfarte behov. 



