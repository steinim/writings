# Orkestrering av IT-utvikling i store organisasjoner

Avhengigheter mellom leveranseteam, og avhengigheter til eksisterende IT-systemer eller forvaltning kan være utfordrende å håndtere. Særlig ved gjennomføring av større IT-prosjekter. Det mest vanlige er å legge omfattende planer for å synkronisere aktiviteter som har avhengigheter. Omfattende planlegging er imidlertid ikke riktig løsning og er direkte skadelig for organisasjoner som jobber Smidig.

---

Jeg er tilhenger av Smidig, Kontinuerlige Leveranser og DevOps, og jeg har sterke meninger om hvordan organisasjoner bør [rigge seg for mer effektive IT-leveranser](http://open.bekk.no/usrbizdevops). Jeg hevder sågar at man bør [slutte med IT-prosjekter](http://open.bekk.no/slutt-med-it-prosjekter). I flere sammenhenger har jeg blitt utfordret på at dette virker for enkelt og at det ikke passer for alle, særlig ikke større organisasjoner. Skeptikerne hevder at IT-prosjekter krever mye koordinering mellom prosjektets team, linjeorganisasjonen, avdelinger eller andre instanser, og at det derfor uansett må brukes mye tid på omfattende planlegging og orkestrering. Hensikten er å ikke sinke utvikling og sikre at det er kapasitet nok til å håndtere de ulike aktivitetene og systemene. Denne tankegangen er, som de fleste vet ikke feilfri. Forsinkelser og utfordringer vil oppstå uansett hvor mye man planlegger. Jeg har full forståelse for problemstillingen, men mener løsningen på problemet er feil.

# Det handler om kommunikasjon!

En av årsakene til at planlegging oppfattes som eneste mulighet for orkestrering av aktiviteter og instanser er at det innenfor prosjektleder-faget ikke finnes et alternativ. For løsningen er ikke direkte knyttet til prosjektledelse. Den er knyttet til teknologi, arkitektur og organisasjon.

> Organizations which design systems ... are constrained to produce designs which are copies of the communication structures of these organizations
> [M. Conway, How Do Committees Invent, 1968](http://www.melconway.com/research/committees.html)

Smidige team sitter sammen og kommuniserer tett hver dag. De kommuniserer ikke like ofte med andre team. Kjernen i utfordringene med orkestrering av IT-utvikling i store organisasjoner er å sørge for koordinering av aktiviteter som spenner over flere instanser. Det kan være funksjonalitet som ikke er komplett før flere team er ferdige med sine endringer, avhengigheter til kjernesystemer, felles grunndata, kapasitet i linja eller venting på beslutninger. Mer effektiv kommunikasjon er løsningen, men ikke i tradisjonell forstand med møter, bestillinger og endringsanmodninger. Kommunikasjonslinjene må struktureres rundt en fornuftig IT-arkitektur og implementeres som kode.

# Ett team per tjeneste 
Ansvar for tjenester bør ikke deles mellom team. Ende-til-ende funksjonalitet kan spenne over flere tjenester eid av ulike team, men eierskapet for hver tjeneste bør være lokalt. Selv om ende-til-ende funksjonalitet kan spenne over flere tjenester så er det viktig at hver funksjonalitet som inngår implementeres ett og bare ett sted, og eies av ett team. Tjenestene har sin egen komplette implementasjon, så man unngår en organisering basert på teknologi (web-team, backend-team, integrasjons-team osv.). For å lykkes må man også unngå en organisering etter funksjon (utvikling, test, drift osv.). Teamene må være autonome nok til å ikke være avhengige av eksterne for å videreutvikle tjenesten (DevOps). Arkitekturen og teknologien i hver tjeneste trenger ikke å være lik som i de andre tjenestene. Andre team trenger i praksis ikke å vite hva som skjer internt i de andre tjenestene. De trenger kun å vite om API-endringene. Kommunikasjonen mellom teamene struktureres rundt kommunikasjon mellom tjenester via API-er.


# Du trenger fortsatt orkestrering!
OK. Vi har nå tjenester som snakker sommen over API-er og hvert team eier hver sine tjenester. Dette løser vel ikke problemene med funksjonalitet som ikke er komplett før flere team er ferdige med sine endringer, avhengigheter til kjernesystemer, felles grunndata, kapasitet i linja eller venting på beslutninger? Jo det gjør faktisk det. 


# Omfattende planlegging er skadelig


[1] Slutt med IT-prosjekter
[2] Kontinuerlig gevinstrealisering med UsrBizDevOps

http://continuousdelivery.com/2016/04/the-flaw-at-the-heart-of-bimodal-it/


Jeg blir ofte utfordret på at IT-prosjekter krever mye koordinering mellom prosjektets team, linjeorganisasjonen, avdelinger eller andre instanser. Avhengighetene mellom de ulike delene som utgjør IT-prosjekter må orkestreres, synkroniseres og legges inn i en fremdriftsplan slik at prosjektledere kan holde styr på fremdriften. Jeg har stor forståelse for at dette er vanskelig, men problemet kan unngås. Løsningen er ikke alltid så lett å forklare fordi den er teknisk. Ikke organisatorisk.
