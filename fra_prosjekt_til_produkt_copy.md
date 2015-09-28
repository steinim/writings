<!--
# Slutt med IT-prosjekter!

[De store IT-prosjektenes tid er kanskje forbi](http://www.cw.no/artikkel/tiden-store-it-anskaffelser-over), men hva med de "små"? Selv "smidige" prosjekter forventes å bli ferdige på en eller annen dato i fremtiden, og når systemet er levert, skal det overleveres til linja. Er det virkelig bare størrelsen som er problemet, eller er det selve arbeidsformen som ikke fungerer? 

-->

Et prosjekt er en arbeidsform som er avgrenset fra de aktivitetene en organisasjon vanligvis gjennomfører. Det er avgrenset i tid og har et mål for hva man vil ha oppnådd når prosjektperioden er over. Typisk etableres det som en midlertidig organisasjon med personer som enten skal ut, eller tilbake til linja. Formålet er å styrke virksomhetens evne til suksess i tiden som kommer. Det er arbeidsformen dessverre lite egnet til.

Det er flere årsaker til at prosjekt som arbeidsform er lite egnet. Eksempler er at det er vanskelig å måle realisering av gevinst, konflikt mellom prosjektets mål og virksomhetens mål, stor avstand mellom prosjekt- og linjeorganisasjon, en kortsiktig finansieringsmodell, manglende kommunikasjon og utfordringer med overlevering og kunnskapsoverføring.

Mange IT-prosjekter benytter en Smidig gjennomføringsmodell. Dette gjør de for å få bedre forutsigbarhet i prosjektene sine. Det er vel og bra, men ikke tilstrekkelig. Problemet sitter ikke i Smidig som sådan, men utenfor. Om Smidig lykkes i å unnfange og utvikle programvare raskt og taktfast så må alt utenfor være i stand til å ta imot det som produseres i samme takt. Hovedutfordringene med det er at mottaksaparatet sjeldent sitter i prosjektene selv og at Smidige prosjekter sjeldent tar inn over seg at programvareutvikling strekker seg langt utover å levere "programvare som fungerer". Hvordan programvaren oppfører seg i produksjon etter overlevering er dessverre alt for sjeldent Smidig-teamets ansvar.

Alternativet er å behandle leveransene som kontinuerlige produktutviklingsløp i linja. Det vil da være enklere å måle gevinster kontinuerlig, justere initiativene opp mot virksomhetens mål, involvere hele organisasjonen, løpende finansiering, bedre kommunikasjon og kunnskapsbygging istedenfor kunnskapsoverlevering.

## "You Build It, You Run It"
Prosjektmedlemmer er avgrenset fra linjeorganisasjonen, og deres involvering med produktene de lager er tidsbegrenset. De slipper å leve med de langsiktige resultatene av deres egne arkitektur- og designbeslutninger. Linjeorganisasjonen er som regel underbemannet og har knappe ressurser og liten evne til å håndtere overleveringer fra prosjekter. De må dessuten administrere, overvåke og supportere eksisterende IT-systemer. Dette medfører som regel dårligere utviklingspraksiser og gradvis forverret kvalitet. Dette forsterkes ytterligere av at man som regel har dårlig tid i prosjekter. Prosjektmedlemmene er som regel skjermet fra analyse og gjenoppretting ved produksjonsproblemer. De tvinges ikke til å legge inn nødvendig overvåkning og nødvendig logging for analyse av rot-årsaker. Teamet gjør ofte et begrenset antall produksjonssettinger og har derfor få insentiver til å investere i automatisering og produksjonslike miljøer.

I Amazon.com, hvor de fokuserer på produkter fremfor prosjekter, er det et viktig prinsipp at de som lager systemene også skal drifte systemene og leve med dem i lang tid. Helt til de dør. "You Build It, You Run It" som Werner Vogels (CTO i Amazon) sier. I Amazon.com har de ikke egne driftsteam. Teamene håndterer selv både drift og utvikling. Det er dette som kalles DevOps.

Da Kent Bekk besøkte DevOps Norway Meetup for et par år siden ble han bedt om å definere hva han legger i begrepet DevOps. Hans svar var: "Developers carry beepers". Når utviklingsteamet får ansvar for å ha beredskap selv, er insentivene på plass for å lage virkelig driftbare systemer. Forvaltning og drift flyttes til starten av utviklingsløpet. Teamet organiseres som en forvaltningsorganisasjon fra dag én.

## Lag funksjoner, ikke systemer
IT-prosjekter har som regel en målsetning om å lage et IT-system som skal løse noen opplevde behov. Disse opplevde behovene formuleres som krav det nye IT-systemet skal støtte. Det nye IT-systemet får gjerne et navn og skal inneholde slik og slik sånn at vi får til slik og slik. Alternativt bestemmer man seg for å implementere den nye funksjonaliteten i et eksisterende system ved å utvide det. Uansett blir det ofte slik at fokuset er på ett eller en begrenset mengde systemer. Om det er flere systemer involvert deler man som regel opp teamene etter system. Mye av årsaken til at prosjekter fort tenker slik er et iboende ønske om at prosjektet skal få jobbe uforstyrret uten involvering og støy fra resten av virksomheten eller andre team.

Dersom man tar utgangspunkt i å lage en ny funksjon, og denne skal lages i et bestemt system, så har man allerede lagt unødvendige begrensninger for hvordan funksjonen kan realiseres. Å fordele oppgaver basert på team som har ansvar for et bestemt system vil som regel medføre at teamet med ansvar for komponenten implementerer funksjonen i sitt eget system som de kjenner godt. At funksjonen bedre kan implementeres i et annet system eller på tvers av flere systemer forsvinner fort med et slikt navlebeskuende fokus. Om man organiserer teamene rundt funksjoner eller forretningsområder, slik det gjøres i for eksempel Spotify, vil systemarkitekturen automatisk speile forretningen bedre. I henhold til Conway's lov fra 1968 så vil strukturen på IT-systemene speile organisasjonens struktur. For å oppnå systemer som speiler forretningsstrukturen må man derfor la team organisere seg rundt funksjoner og ikke systemer.

Når man setter sammen langlevde team rundt funksjoner som understøtter forretningen, så forsterkes forståelsen og ansvarsfølelsen for forretningens visjon. Teamene vet hvor man vil med produktene som lages, og eierskapet, ansvarsfølelsen og stoltheten styrkes. Produktene man lager bør ha sitt opphav i et ønske om å realisere noe verdifullt for virksomheten. Da bør man ikke fokusere på systemer, men på funksjoner som samsvarer med og støtter opp om forretningens mål.

## Kontinuerlige Leveranser og DevOps
Når team tar ansvaret for hele livssyklusen til systemene de lager, og de samtidig forstår og deler forretningens visjon og målsetninger, så finner de ikke bare måter å jobbe på som støtter rask flyt, slik at veien fra konsept til ferdige funksjoner i produksjon blir så kort som overhodet mulig. De sikrer samtidig at det ikke går på bekostning av kvalitet, tilgjengelighet, stabilitet, sikkerhet og så videre. I [The State of DevOps Report for 2015](https://puppetlabs.com/2015-devops-report) avdekkes det blant annet at virksomheter som jobber på denne måten har 30 ganger  hyppigere produksjonssettinger, 200 ganger kortere ledetid, 60 ganger færre feil og 168 ganger raskere gjenopprettingstid ved problemer, enn sammenlignbare virksomheter.

Denne måten å jobbe på er ikke som Smidig. Smidig impliserer ikke kontinuerlig. I tradisjonell Smidig jobber man som regel med batcher og iterasjoner, med mer planlegging, og med testing og akseptanse med jevne mellomrom. Kontinuerlige Leveranser innebærer at programvaren kan produksjonssettes til enhver tid. Siste versjon av kildekoden kan slippes i produksjon når som helst uten behov for forberedelser eller tilpasninger. I "Tradisjonell Smidig" har man ikke fokusert nok på driftsplattformen og ansvarliggjøring av utviklingsteamet for at programvaren som lages skal fungere i lang tid etter at det er i produksjon.

DevOps er en forutsetning for å kunne drive med Kontinuerlige Leveranser. De tradisjonelle overleveringene fra utvikling til drift forhindrer kontinuerlige leveranser, så teamene må drifte programvaren de lager selv. Det fordrer kompetanse om drift og utvikling. Tradisjonelt sett er drift og utvikling to separate fagfelt som krever ulike typer IT-kompetanse. I dag har imidlertid fagfeltene smeltet sammen og det ser ganske annerledes ut. Det holder ikke at den eksisterende driftsavdelingen samarbeider tett med utviklingsavdelingen (selv om det hjelper). Isteden overtar teknologer som kan både drifte og utvikle. Infrastruktur skrives og dokumenteres som kode (software defined everything), konseptet server har endret seg med immutable infrastruktur og containere, testing og produksjonssettinger er helautomatisert, monitorering er mye mer omfattende. Ikke minst skydrift har revolusjonert måten programvare driftes på.

## Fjern alle unødvendige roller
På JavaZone i 2014 holdt jeg et foredrag hvor jeg forsøkte å synliggjøre alle de etter mitt syn unødvendige rollene som eksisterer innen IT, særlig i IT-prosjekter, "[Kill 'Em All – and the ultimate developer will rise again!](https://vimeo.com/105761144)". Det er viktig å bemerke at det ikke er personer jeg ville til livs, men roller. Det bemannes opp med prosjekteiere, prosjektledere, arkitekter, virksomhetsarkitekter, testere, Scrum-mastere, driftere, dba-er, programmerere – og ofte enda flere. Hver eneste en av disse bidrar til at prosjektene mislykkes, eller at de er unødvendig lite effektive. Hovedpoenget mitt var at det kun er behov for tre roller for å lykkes som IT-virksomhet (som jo alle virksomheter i dag er). De tre rollene er utviklere (i vid forstand), forretning, og brukere. Utviklere lager og drifter programvaren som utvikles, forretning skal kapitalisere på verdien programvaren skaper, og brukerne er de sterkeste bidragsyterne til å definere hva programvaren skal gjøre. Disse jobber tett sammen hver eneste dag.

## Fra CapEx til OpEx
CapEx (Capital expenditures) er investeringer man gjør på forhånd for å skape fremtidige gevinster. OpEx (Operational expenditure) er investeringer som gjøres underveis mens forretningen forløper som normalt, "business as usual". Skydrift er et eksempel på en pay-as-you-go finansieringsmodell hvor elastisiteten og fleksibiliteten gjør at du kan skalere opp eller ned underveis istedenfor å investere masse penger i egen infrastruktur og overkapasitet før du trenger den. Jeg snakker her selvsagt om offentlig sky og ikke privat.

IT-prosjekter er investeringer som betales på forhånd. De har budsjetter. De har risiko. Det er bra å investere i IT, men disse investeringene behøver ikke nødvendigvis å gjøres på forhånd. Når utvikling av funksjoner følger resten av virksomheten tett, vil det være mer fornuftig å smøre kostnadene tynnere utover i organisasjonen. Det betyr ikke at man ikke kan satse stort på et område som koster mye, og som gir stor gevinst tilbake. Forskjellen er at risiko reduseres dramatisk om man tar en gradvis tilnærming til en dyr, men potensielt innbringende satsning. Gjennom å finansiere eksperimenter og gi de mest lovende initiativene mer penger når de trenger det, og de mindre lovende mindre eller ingenting, sikrer man en utvikling som er tettere knyttet opp mot forretningens mål enn gjetning på et alt for tidlig tidspunkt. Hensikten med å eksperimentere mer er å unngå å bli fanget i et blindspor. Om en satsning viser seg å bli innbringende kan man finansiere ytterligere for å maksimere uttak av gevinster.

Denne tilnærmingen er ikke nødvendigvis så enkel – det kan være vanskelig å balansere prioriteringer og budsjettering. Det krever at IT-utvikling blir en integrert del av forretningsutvikling og at resultater og hypoteser verifiseres kontinuerlig. Her gjelder det å innse at alle virksomheter i dag er IT-virksomheter og at det er en dårlig idé å ha et skille mellom IT og forretning om man skal lykkes.

## Bare for de små eller bare for de store?
Til de av dere som umiddelbart responderer med at dette er vel og bra for små start-ups, men vil aldri fungere i større virksomheter: Netflix, Google, Amazon, Facebook, Etsy, Twitter. Så til dere som umiddelbart responderer med at de store web-sjappene er dårlige eksempler og ikke sammenlignbart med det vi gjør her på berget: Gov.uk, CitiBank, (????). Så til dere som mener at bransjen min er så spesiell at det ikke vil fungerer hos oss [HP LaserJet Firmware](http://itrevolution.com/the-amazing-devops-transformation-of-the-hp-laserjet-firmware-team-gary-gruver/). Så til dere som umiddelbart responderer at det ikke vil fungerer for legacy systemer: 


## Oppsummering

Det blir vanskeligere og vanskeligere å se at denne klassiske prosjektmodellen er godt egnet for IT-leveranser som innebærer et stykke skreddersøm. Over tid tror vi denne gjennomføringsmodellen vil forsvinne. MVP-/Lean Startup-tankegang, i kombinasjon med No-/DevOp'sy applikasjonsdrift, flytter forvaltningsfasen til starten av utviklingsløpet. Det er derfor enklere å betrakte leveranseteamet som en forvaltningsorganisasjon fra dag én, og heller håndtere prosjektaktige problemstillinger som spesialtilfeller.

Dersom man skal begynne på nye ting anbefaler vi å ikke gjennomføre disse endringene som et prosjekt, men heller se på de alternative gjennomføringsmodellene nevnt over. Vi anbefaler å fase ut den klassiske prosjektorganisasjonen og erstatte denne med flere, mindre enheter med større autonomi. Fokuset bør være på å starte i det små og levere kontinuerlige forbedringer gradvis, og å etablere en voksende organisasjon gradvis - ut fra erfarte behov. 


