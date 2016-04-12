# Orkestrering av IT-utvikling i store organisasjoner

Avhengigheter mellom leveranseteam, og avhengigheter til eksisterende IT-systemer eller forvaltning kan være utfordrende å håndtere. Særlig ved gjennomføring av større IT-prosjekter. Det mest vanlige er å legge omfattende planer for å synkronisere aktiviteter som har avhengigheter. Omfattende planlegging er imidlertid ikke riktig løsning og er direkte skadelig for organisasjoner som jobber Smidig.

---

Jeg er tilhenger av Smidig, Kontinuerlige Leveranser og DevOps, og jeg har sterke meninger om hvordan organisasjoner bør [rigge seg for mer effektive IT-leveranser](http://open.bekk.no/usrbizdevops). Jeg hevder sågar at man bør [slutte med IT-prosjekter](http://open.bekk.no/slutt-med-it-prosjekter). I flere sammenhenger har jeg blitt utfordret på at dette virker for enkelt og at det ikke passer for alle, særlig ikke for større organisasjoner. Skeptikerne hevder at IT-prosjekter krever mye koordinering mellom prosjektets team, linjeorganisasjonen, avdelinger eller andre instanser, og at det derfor uansett må brukes mye tid på omfattende planlegging og orkestrering. Hensikten er å ikke sinke utvikling og sikre at det er kapasitet nok til å håndtere de ulike aktivitetene og systemene. Denne tankegangen er, som de fleste vet, ikke feilfri. Forsinkelser og utfordringer vil oppstå uansett hvor mye man planlegger. Jeg har full forståelse for problemstillingen, men mener løsningen på problemet er feil.

En av årsakene til at planlegging oppfattes som eneste mulighet for orkestrering av aktiviteter og instanser er at det innenfor prosjektleder-faget ikke finnes et godt alternativ til omfattende planlegging, mange roller, mange aktiviteter, sjekkpunkter og milepæler. [Scaled Agile Framework&reg;](http://www.scaledagileframework.com/) ([SAFe&trade;]) eksemplifiserer feil tilnærming til skalering av Smidig. Det er vanskelig å se for seg at eksperimentering og kontinuerlig forbedring har gode levevilkår innenfor dette rammeverket.

# Kommuniser mindre!

> Communication is a sign of dysfunction. It means people aren’t working together in a close, organic way. We should be trying to figure out a way for teams to communicate less with each other, not more.
> Jeff Bezos, CEO i Amazon [1]

Smidige team sitter sammen og kommuniserer tett hver dag. De kommuniserer ikke like tett med andre team. Løsningen på denne utfordringen er ikke å bruke tid og krefter på å øke kommunikasjonen mellom teamene. Kommunikasjon på tvers av team ender fort opp med misforståelser, uenigheter, tidkrevende møter og omfattende dokumentasjon. Man bør derfor se etter løsninger hvor teamene er mindre avhengige av å måtte kommunisere med andre team. Teamene bør være mest mulig autonome. Autonome team er team som kan løse alle oppgaver som skal til for å videreutvikle tjenester uten ekstern innblanding eller behov for å henvende seg til utenforstående personer.

> Organizations which design systems ... are constrained to produce designs which are copies of the communication structures of these organizations
> [M. Conway, How Do Committees Invent, 1968](http://www.melconway.com/research/committees.html)

Man må for all del unngå team organisert etter teknologi (web-team, backend-team, integrasjons-team). Like viktig er det å unngå team organisert etter funksjon (utviklere, testere, drift, sikkerhet, ux). Slike inndelinger kalles silo-organisasjon og kompliserer kommunikasjon enormt. Det er dessuten veldig lite effektivt fordi oppgaver må løses på tvers av flere enheter, noe som medfører overleveringer, venting og misforståelser. Teamene bør isteden organiseres rundt forretningsbehov. Forretningsbehovene implementeres som frittstående applikasjoner av team som besitter all kompetanse som skal til for å utvikle tjenestene de eier. Arkitekturen og teknologien i hver tjeneste trenger ikke å være lik som i de andre tjenestene. Andre team trenger i praksis ikke å vite hva som skjer internt i de andre tjenestene. De trenger kun å vite om API-endringene. Kommunikasjonen mellom teamene struktureres rundt kommunikasjon mellom tjenester via API-er.

![Team kommuniserer over api-er](https://github.com/steinim/writings/raw/master/images/teams-api.png)

# Du trenger fortsatt orkestrering!
OK. Vi har nå tjenester som snakker sommen over API-er og hvert team eier hver sine tjenester. Dette løser vel ikke problemene med funksjonalitet som ikke er komplett før flere team er ferdige med sine endringer, avhengigheter til kjernesystemer, felles grunndata, kapasitet i linja eller venting på beslutninger? Jo det gjør faktisk det. 


# Omfattende planlegging er skadelig

[1] [The Everything Store, Jeff Bezos and the Age of Amazon](http://www.amazon.com/The-Everything-Store-Bezos-Amazon/dp/0316219266), Brad Stone, Little, Brown and Company; 1st edition (October 15, 2013).
[2] Slutt med IT-prosjekter
[3] Kontinuerlig gevinstrealisering med UsrBizDevOps

http://continuousdelivery.com/2016/04/the-flaw-at-the-heart-of-bimodal-it/


Jeg blir ofte utfordret på at IT-prosjekter krever mye koordinering mellom prosjektets team, linjeorganisasjonen, avdelinger eller andre instanser. Avhengighetene mellom de ulike delene som utgjør IT-prosjekter må orkestreres, synkroniseres og legges inn i en fremdriftsplan slik at prosjektledere kan holde styr på fremdriften. Jeg har stor forståelse for at dette er vanskelig, men problemet kan unngås. Løsningen er ikke alltid så lett å forklare fordi den er teknisk. Ikke organisatorisk.

Kjernen i utfordringene med orkestrering av IT-utvikling i store organisasjoner er å sørge for koordinering av aktiviteter som spenner over flere instanser. Det kan være funksjonalitet som ikke er komplett før flere team er ferdige med sine endringer, avhengigheter til kjernesystemer, felles grunndata, kapasitet i linja eller venting på beslutninger. Mer effektiv kommunikasjon er løsningen, men ikke i tradisjonell forstand med møter, bestillinger og endringsanmodninger. Kommunikasjonslinjene må struktureres rundt en fornuftig IT-arkitektur og implementeres som kode.
