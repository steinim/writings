# How do you Invent?

Istedenfor å lese denne bloggposten anbefaler jeg at du leser [Melvin E. Conway](https://en.wikipedia.org/wiki/Melvin_Conway) sitt paper ["How Do Committees Invent?"](http://www.melconway.com/research/committees.html) fra 1968. Om du likevel fortsetter å lese denne bloggposten vil jeg forsøke å gjenfortelle mine åpenbaringer da jeg leste det.

---

Du har sikkert hørt om Conway's Law. Den går som følger:

>  Organizations which design systems are constrained to produce designs which are copies of the communication structures of these organizations.
>
> [M. Conway, How Do Committees Invent, 1968](http://www.melconway.com/research/committees.html)

Selv om Conway skrev sin artikkel på sekstitallet, så fikk ikke "loven" så mye oppmerksomhet før på nittitallet.  Siden har den vært å finne i [hundretusenvis av bloggposter og presentasjoner](http://lmgtfy.com/?q=conway%27s+law). Å kalle det en lov er å ta hardt i. Det var [Fred Brooks](https://en.wikipedia.org/wiki/Fred_Brooks) som siterte artikkelen i klassikeren ["The Mythical Man-Month"](https://en.wikipedia.org/wiki/The_Mythical_Man-Month), hvor han kalte det for "Conway's Law." Det dreier seg nemlig mer om en _observasjon_ enn et bevis ([senere forskning](https://en.wikipedia.org/wiki/Conway%27s_law#Supporting_evidence) bekrefter imidlertid at det stemmer). Observasjonen beskriver på en utmerket og kortfattet måte det også mange andre, inkludert meg, har observert om sammenhengen mellom organisasjoners oppbygning og IT-arkitektur. Som for eksempel at hvert Smidig-team lager hvert sitt system når forretning er organisert etter teaminndelingen. "Loven" har gitt grobunn for fokuset på å bryte ned organisatoriske siloer for å skape mer effektive organisasjoner som tilfredsstiller brukernes behov. Digitalisering, DevOps og mikrotjenester er eksempler på fenomener som har oppstått i kjølvannet.

## Har du ikke lest hele artikkelen?
Jeg har ofte sitert Conway's lov – også før jeg hadde lest hele artikkelen. Kanskje burde jeg ikke ha gjort det, men jeg føler ikke at jeg har bommet på intensjonen. Mange andre (som sikkert har lest artikkelen) har forklart meg hva den betyr. Nå har jeg imidlertid lest artikkelen, og det vil jeg anbefale alle andre å gjøre også. Den inneholder nemlig mye mer gull enn bare "loven".

## Conway's konsekvens
Følgende sitat er ofte omtalt som "Conway's konsekvens" (corollary), og sier at fleksibilitet i organisasjonen er viktig for å oppnå effektiv design.

> Flexibility of organization is important to effective design.


> There is a homomorphism from the linear graph of a system to the linear graph of its design organization.

> If you have four groups working on a compiler, you'll get a 4-pass compiler.
>
> [Eric S. Raymond, 1991](http://catb.org/~esr/jargon/html/C/Conways-Law.html)


## Conway om kontinuerlig forbedring
> There's never enough time to do something right, but there's always enough time to do it over.

> Given any system design, someone someday will find a better one to do the same job.

## Store systemer går i oppløsning
> The structures of large systems tend to disintegrate during development, qualitatively more so than with small systems.

> If a team can’t be fed with two pizzas, it’s too big.
>
> Jeff Bezos, CEO Amazon

### Årsak #1
> The realization that the system will be large, together with certain pressures in their organization, make irresistible the temptation to assign too many people to a design effort.

> Two men working for a year or one hundred men working for a week (at the same hourly cost per man) are (not) resources of equal value.

> Adding manpower to a late software project makes it later.
>
> [Fred Brooks, The Mythical Man-Month, 1975](https://en.wikipedia.org/wiki/Brooks%E2%80%99_law)

### Årsak #2
> Application of the conventional wisdom of management to a large organization causes its communication structure to disintegrate.

> Even in a moderately small organization it becomes necessary to restrict communication in order that people can get some "work" done.

### Årsak #3
> Homomorphism insures that the structure of the system will reflect the disintegration which has occurred in the organization.

## Hva kan vi lære av Conway?
1. Increase communications

2. Support continuous process

3. Organize teams by products

4. Make teams small as necessary
