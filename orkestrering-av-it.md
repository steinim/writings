![orchestration](https://github.com/steinim/writings/raw/master/images/dirigent.png)

# Orkestrering av IT-utvikling i store organisasjoner

Avhengigheter mellom leveranseteam, og avhengigheter til eksisterende IT-systemer eller forvaltning kan være utfordrende å håndtere. Særlig ved gjennomføring av større IT-prosjekter. Det mest vanlige er å legge omfattende planer for å synkronisere aktiviteter som har avhengigheter. Omfattende planlegging er imidlertid ikke riktig løsning og er direkte skadelig for organisasjoner som jobber Smidig.

---

Jeg er tilhenger av Smidig, Kontinuerlige Leveranser og DevOps, og jeg har sterke meninger om hvordan organisasjoner bør [rigge seg for mer effektive IT-leveranser](http://open.bekk.no/usrbizdevops). Jeg hevder sågar at man bør [slutte med IT-prosjekter](http://open.bekk.no/slutt-med-it-prosjekter). I flere sammenhenger har jeg blitt utfordret på at dette virker for enkelt og at det ikke passer for alle, særlig ikke for større organisasjoner. Skeptikerne hevder at IT-prosjekter *krever* mye koordinering mellom prosjektets team, linjeorganisasjonen, avdelinger eller andre instanser, og at det derfor uansett må brukes mye tid på omfattende planlegging og orkestrering. Hensikten er å sikre effektiv utvikling, og å samtidig sikre at det er kapasitet nok til å håndtere de ulike aktivitetene og systemene. Denne tankegangen er, som de fleste vet, ikke problemfri. Forsinkelser og utfordringer vil oppstå uansett hvor mye man planlegger. Jeg har full forståelse for problemstillingen, men mener løsningen på problemet som regel er feil.

En av årsakene til at planlegging oppfattes som eneste mulighet for orkestrering av aktiviteter og instanser er at det innenfor prosjektleder-faget ikke finnes et godt alternativ til omfattende planlegging, mange roller, mange aktiviteter, sjekkpunkter og milepæler. [Scaled Agile Framework&reg;](http://www.scaledagileframework.com/) (SAFe&trade;) er ett eksempel på feil tilnærming til skalering av Smidig. Det er vanskelig å se for seg at eksperimentering og kontinuerlig forbedring har gode levevilkår innenfor dette rammeverket.

## Kommuniser mindre!

> Communication is a sign of dysfunction. It means people aren’t working together in a close, organic way. We should be trying to figure out a way for teams to communicate less with each other, not more.
>
> [Jeff Bezos, CEO i Amazon](http://www.amazon.com/The-Everything-Store-Bezos-Amazon/dp/0316219266)

Smidige team sitter sammen og kommuniserer tett hver dag. De kommuniserer ikke like tett med andre team. Løsningen på denne utfordringen er ikke å bruke tid og krefter på å øke kommunikasjonen mellom teamene. Kommunikasjon på tvers av team ender fort opp med misforståelser, uenigheter, tidkrevende møter og omfattende dokumentasjon. Man bør derfor se etter løsninger hvor teamene er mindre avhengige av å måtte kommunisere med andre team. Teamene bør være mest mulig autonome. Autonome team er team som kan løse alle oppgaver som skal til for å videreutvikle tjenester uten ekstern innblanding eller behov for å henvende seg til utenforstående personer. Dette gjør at tjenesteutvikling kan foregå raskest mulig.

## Systemer = forretningsbehov
> Organizations which design systems ... are constrained to produce designs which are copies of the communication structures of these organizations
>
> [M. Conway, How Do Committees Invent, 1968](http://www.melconway.com/research/committees.html)

Man må for all del unngå team organisert etter teknologi (web-team, backend-team, integrasjons-team). Like viktig er det å unngå team organisert etter funksjon (utvikling, test, drift, sikkerhet, ux). Slike inndelinger kalles silo-organisasjon og kompliserer kommunikasjonen enormt. Det er dessuten veldig lite effektivt fordi oppgaver må løses på tvers av flere enheter, noe som medfører overleveringer, venting og misforståelser. Teamene bør isteden organiseres rundt forretningsbehov.

> Microservices allow organizations to align the architecture of their systems to the structure of their teams.
>
> [Sam Newman, Demystifying Conway’s Law, 2015](https://www.thoughtworks.com/insights/blog/demystifying-conways-law)

En viktig forutsetning for å lykkes med en API-basert organisasjon er at IT-arkitekturen brytes ned på en måte som gjør at det å legge til ny funksjonalitet påvirker én tjeneste. Data og funksjonalitet implementeres der hvor det i et forretningsperspektiv hører best hjemme eller som en ny tjeneste dersom det ikke har et naturlig tilholdssted.

Forretningsbehovene implementeres som frittstående applikasjoner av team som besitter all kompetanse som skal til for å videreutvikle tjenestene de eier. Teamet eier hele stacken fra database til GUI og har ansvar for design, utvikling, test, og release til produksjon. Arkitekturen og teknologien i hver tjeneste trenger ikke å være lik som i de andre tjenestene. Andre team trenger i praksis ikke å vite hva som skjer internt i de andre tjenestene. De trenger kun å vite om API-endringene. Kommunikasjonen mellom teamene struktureres rundt kommunikasjon mellom tjenester via API-er.

![Team kommuniserer over api-er](https://github.com/steinim/writings/raw/master/images/teams_api.png)

##  Anyone who doesn’t do this will be fired.  Thank you; have a nice day!
Sitatet er hentet fra et [pålegg](http://nfbnet.org/pipermail/nfbcs_nfbnet.org/2011-October/003472.html) utstedt av Jeff Bezos, CEO i Amazon, i 2002 i følge en tidligere ansatt. Pålegget sa at alle team fra nå av var nødt til å eksponere funksjonalitet og data gjennom API-er og at teamene kun hadde lov til å kommunisere med hverandre via API-ene. Ingen unntak. Denne beslutningen la mye av grunnlaget for at Amazon kunne gå fra å kun være en bokhandel til å også bli den ledende tilbyderen av skyplattform i verden ([AWS](https://aws.amazon.com/)).

Det er viktig med streng disiplin og en forretningsside som deltar tett sammen med teamene og som understøtter deres forretningsområde. Det er forretning som skal drive utviklingsarbeidet av sine produkter og tjenester, ikke IT. Utviklingsteamet skal legge til rette for at forretningssiden kan produsere verdi kontinuerlig gjennom en effektiv, smidig og fullautomatisert prosess for utvikling og utrulling av endringer. Med systemer som er adskilt fra hverandre og som kommuniserer over API-er er det ikke særlig vanskelig å legge til rette for en slik prosess. Men det krever disiplin!

> There will be no other form of inter-process communication allowed: no direct linking, no direct reads of another team’s data store, no shared-memory model, no back-doors whatsoever. The only communication allowed is via service interface calls over the network.
>
> [Jeff Bezos, CEO Amazon, i følge en tidligere ansatt i Amazon](http://nfbnet.org/pipermail/nfbcs_nfbnet.org/2011-October/003472.html)

## DevOps for stormaskin
Vi kan grovt dele inn en virksomhets systemer i to. Grunndata-systemer og kundevendte systemer. Grunndata er fellessystemer som ofte tjener som backend for kundevendte systemer. De inneholder ofte sensitive og verdifulle data for virksomheten og er preget av å være utviklet i en annen tid. De kan også inneholde virksomhetskritisk funksjonalitet, som for eksempel bokføring av banktransaksjoner. Kundevendte systemer bygges ofte på toppen av disse og benytter kritiske data og funksjoner fra grunndata-systemene for å tilby tjenester til sluttbrukere. Om flere kundevendte systemer leser fra og skriver til disse systemene, eller har behov for endringer, så oppstår integrasjoner som ikke foregår over API-er. Dette forhindrer hva vi ønsker å oppnå. Det er fort gjort å falle tilbake til orkestrering gjennom omfattende planlegging og orkestrering.

Å skrive om alle disse grunndata-systemene til mikrotjenester uten avhengigheter og med perfekte veldefinerte API-er som kan releases kontinuerlig er neppe en farbar vei for å komme ut av dette uføret på kort sikt. Det vil jeg heller ikke foreslå å gjøre. For det første er det veldig vanskelig å forstå hvorfor og hvordan alle delene henger sammen i et stort og komplekst system, for det andre er det enormt ressurskrevende, og for det tredje tar det fokus bort fra å lage kundevendte systemer som brukerne og forretning ønsker seg.

Løsningen er å gradvis skape en arkitektur med løsere koblinger til baksystemene og sakte flytte funksjonalitet og data dit hvor de hører naturlig hjemme. Formålet er å muliggjøre utvikling, testing og produksjonssetting uten å være avhengig av et integrert miljø med alle avhengigheter.

> So if you think you can’t implement DevOps practices because your app runs on a mainframe, think again. Don’t focus on the type of system you have: Instead, focus on re-architecting for testability and deployability.
>
> [2015 State of DevOpsReport](https://puppet.com/resources/white-paper/2015-state-of-devops-report), side 17.

## Kvel meg sakte
Det man bør forsøke å oppnå, er færrest mulig endringer i baksystemene og løsere koblinger mellom kundevendte systemer og baksystemene. Ved utvikling av nye tjenester bør man derfor forsøke å gjøre seg så uavhengig som mulig av funksjoner som er implementert i baksystemene. Den nye tjenesten som skal utvikles har egne krav til funksjonalitet som kanskje ligner, men som ikke er helt det samme som er implementert i baksystemet. Gjenbruk er fristende, men bør unngås for enhver pris. På kort sikt medfører dette at man ikke ødelegger for andre tjenester fordi man slipper å gjøre endringer i baksystemet som benyttes av flere. Om man i tillegg kan få andre tjenester til å bruke den nye tjenesten over et API har man virkelig tatt et stort steg i riktig retning. På lengre sikt vil kanskje ingen ha bruk for funksjonaliteten i baksystemet lenger og man kan skru denne av. Ved streng disiplin vil man således sakte kvele det gamle systemet.

Delte data er også utfordrende og bør håndteres på en lignende måte. Ved utvikling av nye tjenester fokusert rundt forretningsbehov bør man være kritisk til hvilke data tjenestene har behov for å lese, og hvilke den har behov for å manipulere. Data bør eies av *en og bare en* tjeneste og tilgjengeliggjøres via et API. For å få til dette må man sikre seg at den resulterende datamodellen er fornuftig med tanke på forretningsmessige behov. Det anbefales ikke å gjøre dette i en stor operasjon. Endringene bør være forretningsdrevet. Den mest fornuftige datamodellen oppnås gjennom å la den gjenspeile forretningen.

Hovedpoenget er at dette ikke er noe man gjør i én stor omskrivingsoperasjon. Omfattende endringer i datamodellen går sjelden bra. Om man skal lykkes er det viktig å ha is i magen. Det bør likevel ikke være en hindring for hovedpoenget i denne artikkelen om orkestrering av IT-utvikling i store organisasjoner. Tvert imot. Gjennom å fokusere på forretningsbehov for enhver endring man gjør, og ved å finne de naturlige tjenestene som understøtter konkrete forretningsbehov, så vil den rolige transformasjonen mot en virksomhet som ruller ut verdiskapende programvare på løpende bånd komme som en konsekvens. Ikke på lengre sikt, men ganske umiddelbart.

## En teknisk løsning på en organisatorisk utfordring
Orkestrering av IT-utvikling i store organisasjoner og/eller prosjekter er utfordrende. Derfor brukes det ofte mye tid og krefter på omfattende planlegging, dokumentasjon, løpende koordinering, overleveringer, møter og endringsanmodninger. Disse aktivitetene koster mye i form av tid og krefter, og de bidrar i liten grad til å løse de reelle utfordringene. Effektene av dårlig organisering løses best ved omorganisering, ikke ved mer koordinering og kontroll.

Om man skal lykkes med Smidig er det viktig at teamene får jobbet uforstyrret og effektivt uten venting. De skal slippe å bruke mye tid på kommunikasjon og koordinering med aktører utenfor teamet. Det forutsetter at hvert team er organisert rundt systemer som kan videreutvikles uten avhengigheter til endringer i andre systemer. Dette oppnås ved at teamene lager applikasjoner som skal løse enkeltstående forretningsbehov og at all kommunikasjon med andre systemer foregår over API-er. Arkitekturen som oppstår som en følge av denne inndelingen påvirker organisasjonen. Forretning organiseres i henhold til hvordan systemene og utviklingsteamene er organisert og kan videreutvikle sine forretningsbehov uavhengig av resten av organisasjonen. Orkestrering handler dermed om å styre og koordinere i henhold til de forretningsmessige behovene og ikke IT-systemene.
