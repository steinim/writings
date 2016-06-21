![Melvin E. Conway](https://github.com/steinim/writings/raw/master/images/conway.png)

# How do you Invent?

Istedenfor å lese denne bloggposten anbefaler jeg at du leser [Melvin E. Conway](https://en.wikipedia.org/wiki/Melvin_Conway) sin artikkel ["How Do Committees Invent?"](http://www.melconway.com/research/committees.html) fra 1968. Om du likevel fortsetter å lese denne bloggposten vil jeg forsøke å gjenfortelle høydepunkter og knytte noen egne tanker til hva som står i den. Det er nemlig ikke bare Conway's Law som er verdt å få med seg.

---

Du har sikkert hørt om Conway's Law. Den går som følger:

>  Organizations which design systems are constrained to produce designs which are copies of the communication structures of these organizations.
>
> [M. Conway, How Do Committees Invent, 1968](http://www.melconway.com/research/committees.html)

Selv om Conway skrev sin artikkel på sekstitallet, så fikk ikke "loven" så mye oppmerksomhet før på nittitallet. Siden har den vært å finne i [hundretusenvis av bloggposter og presentasjoner](http://lmgtfy.com/?q=conway%27s+law). Å kalle det en lov er å ta hardt i. Det var [Fred Brooks](https://en.wikipedia.org/wiki/Fred_Brooks) som siterte artikkelen i klassikeren ["The Mythical Man-Month"](https://en.wikipedia.org/wiki/The_Mythical_Man-Month), hvor han kalte det for "Conway's Law." Det dreier seg nemlig mer om en _observasjon_ enn et bevis ([senere forskning](https://en.wikipedia.org/wiki/Conway%27s_law#Supporting_evidence) støtter imidlertid observasjonen). Observasjonen beskriver på en utmerket og kortfattet måte sammenhengen mellom organisasjoners struktur og IT-arkitektur. Som for eksempel at hvert Smidig-team lager hvert sitt system når forretningen er organisert etter teaminndelingen. "Loven" har gitt grobunn for et fokus på å bryte ned organisatoriske siloer for å skape mer effektive organisasjoner som tilfredsstiller brukernes behov. Digitalisering, DevOps og mikrotjenester er eksempler på fenomener som har oppstått i kjølvannet.

## Har du ikke lest hele artikkelen?
Jeg har ofte sitert Conway's Law – også før jeg hadde lest hele artikkelen. Kanskje burde jeg ikke ha gjort det, men jeg føler ikke at jeg har bommet på intensjonen. Mange andre (som sikkert har lest artikkelen) har forklart meg hva den betyr. Nå har jeg imidlertid lest artikkelen, og det vil jeg anbefale alle andre å gjøre også. Den inneholder nemlig mye mer gull enn bare "loven". Artikkelen har hatt enorm betydning for moderne IT. Mye mer enn jeg ante.

## Conway's konsekvens
Følgende sitat er ofte omtalt som "Conway's konsekvens" (corollary):

> Flexibility of organization is important to effective design.

Dersom Conway's Law er korrekt vil fleksibiliteten i en organisasjon påvirke hvordan den designer ting, også IT-arkitektur. Han beskriver at det er en homomorfisme (avbildning) mellom organisasjonen og systemet den produserer.

> There is a homomorphism from the linear graph of a system to the linear graph of its organization.

![Homomorfisme mellom system og organisasjon](https://github.com/steinim/writings/raw/master/images/conway_homomorphism.png)

Conway har hatt stor påvirkning på en av de store hypene for tiden – mikrotjenester. Som vi ser av figurene under har [konseptet mikrotjenester](http://martinfowler.com/articles/microservices.html), slik det er formulert av James Lewis og Martin Fowler, hentet inspirasjon fra Conway's konsekvens. Sam Newman, kollega av Lewis og Fowler, skriver i sin bloggpost ["Demystifying Conway's Law"](https://www.thoughtworks.com/insights/blog/demystifying-conways-law):

> Microservices allow organizations to align the architecture of their systems to the structure of their teams.
>
> [Sam Newman, Demystifying Conway’s Law, 2015](https://www.thoughtworks.com/insights/blog/demystifying-conways-law)

![Mikrotjenester](https://github.com/steinim/writings/raw/master/images/microservices.png)

Mikrotjeneste-arkitektur har ingen presis definisjon. For eksempel er det uenighet om hvor store mikrotjenester bør være. Det er imidlertid noen felles karakteristika. Tjenestene skal kunne produksjonssettes uavhengig av hverandre, produksjonssetting skal være automatisert, de er desentraliserte og må orkestreres, de snakker sammen over veldefinerte API-er, og de er organisert rundt forretningsbehov. Det er det siste kjennetegnet som gjør tjenestedesign fleksibelt, men denne fordelen oppnås ikke uten at også organisasjonen er fleksibel. Om mikrotjenester skal gi virkelig verdi må organisasjonen tilpasse seg IT-arkitekturen og vice versa.

## Conway om kontinuerlig forbedring
Har du bidratt til å utvikle et IT-system noen gang så vet du at perfeksjon er umulig. Ikke bare første gang du lager det, men hver gang du gjør en forbedring.

> Given any system design, someone someday will find a better one to do the same job.

Dette er sant for alt vi gjør, og det er derfor vi innen systemutvikling snakker om kontinuerlig alt mulig rart. Kontinuerlig forbedring, -integrasjon, -testing, -deployment, -leveranse og så videre. Vi må gradvis og kontinuerlig forbedre alt vi gjør. Et IT-system er aldri ferdig, på samme måte som at forretningsbehov er under stadig utvikling. Digitaliseringsbølgen som skyller over samfunnet krever kontinuerlig nytenkning og eksperimentering.

> There's never enough time to do something right, but there's always enough time to do it over.

Vi er selvsagt enige i dette, men av (for meg) uforståelige grunner eksisterer det fremdeles IT-prosjekter hvor de som styrer gjennomføringen ikke har tatt dette innover seg. Conway beskriver at idealet om å etablere avgrensninger, lage et konsept, organisere et prosjekt og delegere aktiviteter, koordinere mellom oppgaver og å konsolidere sub-design til ett enkelt system ikke alltid er rett frem å gjøre (underdrivelse!). Endringer i forutsetninger vil kunne inntreffe hvor som helst, og nye åpenbart overlegne design-konsepter vil avdekkes. Dette kan være utfordrende å innrømme, men er nødvendig å forstå om man skal lykkes.

> Such an appearance of uncertainty is unflattering, and the very act of voluntarily abandoning a creation is painful and expensive.

## Conway om store systemer og store organisasjoner

Jo større en organisasjon er jo vanskeligere er det å være fleksibel. Effektiv kommunikasjon med lite overhead er krevende å få til. Samarbeid mellom de riktige enhetene og personene som kreves for å oppnå mål er uoversiktelig og vanskelig å legge til rette for.

> To the extent that an organization is not completely flexible in its communication structure, that organization will stamp out an image of itself in every design it produces. The larger an organization is, the less flexibility it has and the more pronounced is the phenomenon.

Om man ikke evner å skape fleksibilitet i organisasjonen og sette sammen mindre grupperinger som kan jobbe med avgrensede forretningsområder vil resultatet bli monolittiske store IT-systemer som er tilsvarende lite fleksible. Store og komplekse IT-systemer er svært krevende å forvalte og videreutvikle og vil ofte falle over av sin egen tyngde. Endringer blir vanskeligere og vanskeligere å legge til, og nye forretningsmuligheter vanskelige å forfølge. Mindre systemer er derfor å foretrekke, men det krever en fleksibel organisasjon som kan håndtere det.

> The structures of large systems tend to disintegrate during development, qualitatively more so than with small systems.

Conway gir tre årsaker til hvorfor dette er tilfelle.

### Årsak #1
> The realization that the system will be large, together with certain pressures in their organization, make irresistible the temptation to assign too many people to a design effort.

Om oppgaven blir for stor er det fristende å skalere opp med mye folk. Store IT-prosjekter er et godt eksempel på at man gaper over for mye. Ofte tar man ikke i betraktning at flere folk sjeldent gjør at oppgaven løses raskere.

> Two men working for a year or one hundred men working for a week (at the same hourly cost per man) are (not) resources of equal value.

Å bemanne opp med fler folk i et pågående prosjekt for å kompensere for at oppgaven ikke løses raskt nok er enda værre, noe [Fred Brooks](https://en.wikipedia.org/wiki/Fred_Brooks) også forklarer i ["The Mythical Man-Month"](https://en.wikipedia.org/wiki/The_Mythical_Man-Month).

> Adding manpower to a late software project makes it later.
>
> [Fred Brooks, The Mythical Man-Month, 1975](https://en.wikipedia.org/wiki/Brooks%E2%80%99_law)

### Årsak #2
> Application of the conventional wisdom of management to a large organization causes its communication structure to disintegrate.

> Even in a moderately small organization it becomes necessary to restrict communication in order that people can get some "work" done.

> Communication is a sign of dysfunction... We should be trying to figure out a way for teams to communicate less with each other, not more.
> 
> [Jeff Bezos, CEO i Amazon](http://www.amazon.com/The-Everything-Store-Bezos-Amazon/dp/0316219266)

### Årsak #3
> Homomorphism insures that the structure of the system will reflect the disintegration which has occurred in the organization.

## Hva kan vi så lære av Conway?
1. Increase communications

2. Support continuous process

3. Organize teams by products

4. Make teams small as necessary


---
> If you have four groups working on a compiler, you'll get a 4-pass compiler.
>
> [Eric S. Raymond, 1991](http://catb.org/~esr/jargon/html/C/Conways-Law.html)
