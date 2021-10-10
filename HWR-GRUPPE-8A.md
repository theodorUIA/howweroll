# How-We-Roll Gruppe 8A

I denne markdown filen skal vi beskrive vår fremgangsmåte for å lage nettsiden **How We Roll**. Vi har benyttet utviklingsmetodikken Kanban for å organisere programmeringen, men vi har organisert gruppen mer tradisjonelt med en gruppeleder og en gruppeleder-vara. Gruppelederens oppgave har vært å inkludere så mange som mulig i gruppen i arbeidet, i tillegg har gruppelederen ansvar for praktisk organisering av oppmøter m.m.
Gruppeleder-vara har i oppgave å ta over oppgavene til gruppeleder i gruppeleders fravær, samt skrive referat fra hvert møte vi gjennomfører.

## Fremgangsmåte/metodikk
Utviklingssyklussen. Skisser. Prototyper. 

## Organisering
Gruppesammensettning. Gruppeorganisering. Ledelsesstruktur. Mål og ønsker i starten. Utvikling underveis. Hva fungerte godt. Hva fungerte dårlig.

## Verktøy
Programmeringsmiljø. Nettressurser vi fokuserte på. Kilder til læring. Læringsmetoder. Undervisning internt i gruppen.

## Regler for Git
Hva vi ble enige om i starten. Begrunnelse for hvorfor vi gjorde det slik. Hvorfor vi eventuell ikke burde gjøre det videre.

## Utviklingsprosess
Hvert enkelt gruppemedlem har bidratt til prosjektet i større og mindre grad. I et slikt prosjekt er det vanskelig å få lik deltakelse, men vi har etterstrebet at alle gruppemedlemmer skal inkluderes i alle steg av utviklingsprosessen. 

### Skisser/prototype
[Vise bilder av design og brukerreiser her.]

### Avgjørelser i.h.t design og programmeringskode
Vår innlevering består av 3 språk. HTML, CSS og Javascript. Dette er de tre mest grunneleggende kodespråkene en kan lære og likevel anvende på en effektiv og god måte. Vi ble anbefalt til å lære oss disse språkene, mest kritisk var HTML og CSS. Siden disse er grunnsteinen i en nett side var det viktigst at vi satt oss inn i det først. Deretter mot slutten av prosjektet ble vi oppfordret til å se litt på Javascript, siden det ville være relevant med uthenting av data fra oppgaven. Det var ikke forventet å "kunne" Javascript, men ha en viss forståelse. HTML brukte vi for å legge inn teksten og innholdet i nettsiden, samt legge til funksjoner som knapper og linker. Deretter CSS for å "style" dette slik at det skulle se bra ut. Så til slutt for å hente ut og framvise data, brukte vi Javascript. Javascript er ikke kun for å hente ut data, men for å lage funskjoner som gjør at nettsiden fungerer bedre. Ved hjelp av mer tid og annet kodespråk kunne nettsiden blitt det som er forventet av systematikere den dag idag, men siden vi fortsatt er i startfasen ble det en forsåvidt "enkel" nettside. 

Det at nivået i gruppa når det kom til koding varierte, førte også til at mye av gruppetimer ble brukt til bortlæring og fremvisning. Mens noen kodet inn for eksempel Javascript så resten av gruppen på en delt skjerm, og fikk gjennomgang i hvordan koden fungerte. Det hjalp i gi en felles forståelse av kode som ble brukt i prosjektet innad i gruppa, samtidig som at de som hadde erfaring fikk gjennomgå det å undervise.
Målet til gruppen var å gi nybegynnerne en god start, samtidig som de med erfaring fikk frisket opp. Samtidig som de lærte om det å undervise og noen ganger noe nytt om koding.


### Læringsprosesses
Gruppen har fokuset på enkelte nettressuser for å komme frem til nettsiden slik den er idag. Listen reflekterer ikke den komplette listen over ressurser vi har brukt, men er ment for å trekke frem noen ressurser og forklare fordeler og ulemper ved disse.
- [HTML tutorial](https://developer.mozilla.org/en-US/docs/Web/Tutorials#html-tutorials)
- [CSS tutorial](https://developer.mozilla.org/en-US/docs/Web/Tutorials#css-tutorials)
- [Javascript tutorials](https://developer.mozilla.org/en-US/docs/Web/Tutorials#javascript-tutorials)
- [W3 schools](https://www.w3schools.com/)

### Individuell refleksjon/læringsprosess
Hvert enkelt gruppemedlem har hatt et ulikt utgangspunkt ved starten av denne oppgaven. Derfor har læringsprosessen hos den enkelte også vært ulik. Noen likehetstrekk har vi, men vi har valgt å fremheve de individuelle fremgangsmåtene under.

#### Theodor
I forkant av How We Roll har jeg programmert tidligere og har hatt god kjennskap til HTML, CSS og JavaScript fra før. Jeg har derfor fokusert på detaljene i undervisningen som er gitt i programmering, samt nøyaktighet på syntax som benyttes i HTML og CSS. Kanban-board og bruk av GitHub-projects var nytt for meg, og jeg benyttet noen [videoer om Kanban](https://youtu.be/CKWvmiY7f_g) fra YoutTube for å lære mer detaljert om hva metodikken innebærer. Kanban minner mye om SCRUM som jeg har jobbet med tidligere, så jeg har jobbet med å fremheve forskjellene underveis i prosjektet. Også i dette har jeg benyttet YouTube til å finne [videoer som beskriver forskjellene](https://youtu.be/HNd1_irOL5k). GitHub-projects var også nytt for min del, og jeg brukte litt tid i starten for å sette meg inn i hvordan vi skulle organisere prosjektet der når så få hadde bakgrunn fra programmering, og ikke minst GitHub. For å få litt oversikt over GitHub-projects benyttet jeg denne [videoen om automatisert Kanban project management](https://youtu.be/YVFa5VljCDY), samt undervisningen som ble gitt i emnet.

Underveis i prosjektet ble Javascript mer aktuelt, og spesielt generering av canvas-element basert på `fetch()`av json-filer som jeg aldri har gjort før. Jeg satte meg grundig inn i hvilke muligheter og begrensninger som fantes ved å lese på [w3schools.com](https://www.w3schools.com/html/html5_canvas.asp), [MDN Web docs](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API), samt se på hva [som var mulig å få til](https://code.tutsplus.com/articles/21-ridiculously-impressive-html5-canvas-experiments--net-14210). Etter å har laget en nesten ferdig kode for visning av data ved bruk av Canvas, ønsket jeg å se litt nærmere på et alternativ; SVG.

*Utdrag fra Canvas-koden:*
```

	//Funksjon for å tegne sirkler på linjen i canvas-elementet "work-canvas".
	Trenger en tallverdi og en farge-verdi for å fungere.
function drawWork (value, color) {
		let val = value * 10; //henter inn tallverdi og ganger med 10 for å vises korrekt på linjen i canvas-elementet
		if(val == 0) { val = val + 10; }
		if(val == 1000) { val = val - 10; }
		var sirkel = workCanvas.getContext("2d"); //Oppretter sirkel-tegning
		sirkel.beginPath(); //start på sirkel
		sirkel.arc(val,25,10,0,2*Math.PI); //"Kurven" på sirkelen
		sirkel.fillStyle = color; //Legger inn fargen på fyllet i sirkelen fra variabel "color"
		sirkel.fill(); //Fyller sirkelen med farge
		sirkel.stroke(); //Setter en ramme rundt sirkelen
	}
```

SVG hadde jeg heller ikke programmert særlig med, selv om jeg har laget noen ikoner og små-ting tidligere så var denne typen visualisering nytt. Jeg benyttet de samme kildene som når jeg undersøkte Canvas, men jeg fant spesielt en ressurs som jeg tok mye inspiriasjon fra. [Motionstricks](https://www.motiontricks.com/creating-dynamic-svg-elements-with-javascript/) går gjennom steg-for-steg hvordan man genererer SVG med JS. [Creative blog](https://www.creativebloq.com/features/the-complete-guide-to-svg) har også en god guide på innføring i SVG som var nyttig i avgjørelsen om gå fra Canvas til SVG. Hovedgrunnen til å bytte fra Canvas-element til SVG-element var på grunn av måten de genereres på i Javascript og hvordan SVG-elementene kan manipuleres etter at siden (DOM) er lastet. Det at [Canvas er mindre ressurskrevende enn SVG](https://www.sitepoint.com/canvas-vs-svg/) var heller ikke aktuelt i denne oppgaven siden det ikke var mange elementer som skulle lages. Men skulle visualiseringen inneholdt mange flere elementer hadde nok Canvas vært et bedre valg for å unngå for mye belasting på klienten.

Jeg har brukt mye av tiden i gruppetimene til å vise/forklare ulike deler av HTML, CSS og Javascript for resterende gruppemeldemmer, men det var ikke før vi bestemte oss for å teste par-programmering at utviklingen hos den enkelte satte fart. Hvert par diskuterte seg imellom før de evt spurte meg om det satt fast på, noe som gjorde tiden vi brukte på felles gjennomgang av kode mye mer nyttig.

Vi har utviklet en løsningen hvor Javascript-koden kanskje er unødvendig avansert mtp erfaringsnivået i gruppen, men vi har gjennomgått koden i detalj sammen og mitt inntrykk er at alle har en forståelse for hvordan de ulike funksjonene fungerer uten å ha inngående kunnskap om det.

Neste gang det kommer et slikt prosjekt vil jeg prøve å fokusere enda mer på organisering og prosessen rundt fordeling av programmeringsoppgaver. Jeg opplevde det som uoversiktlig å ikke starte med gode rammer for hvordan Git skulle fungere i gruppen, og ikke minst hvordan fordele relativt **små** programmeringsoppgaver på 8 gruppemedlemmer. Effekten av at vi var så mange kom til syne når alle hadde en grunnleggende forståelse for programmering i HTML og CSS. Da ble det produsert kode hurtig, og nettsiden slik den ser ut i dag kom ganske kjapt sammen.




Hva jeg har lært, hvordan (med kilder), hvilken betydning det hadde for prosjektet. Hva jeg ville gjort annerledes. Hvilke kilder/ressurser som virket bedre enn andre. Foretrukket læringsmetode; forelesning, gruppe-undervisning, par-programmering, undersøke på egenhånd, undervise/forklare til andre.

#### Thomas
Hva jeg har lært, hvordan (med kilder), hvilken betydning det hadde for prosjektet. Hva jeg ville gjort annerledes. Hvilke kilder/ressurser som virket bedre enn andre. Foretrukket læringsmetode; forelesning, gruppe-undervisning, par-programmering, undersøke på egenhånd, undervise/forklare til andre.

#### Jacob
I løpet av How we roll oppgaven har jeg forsøkt i sette meg inn i koding på et veldig enkelt nivå.
Jeg har tilegnet meg en veldig grunnleggende kompetanse, som gir meg mulighet til å bruke Html og Css i en viss grad.
I startperioden av prosjektet kom jeg ikke så veldig godt i gang, noe som gjorde at jeg mistet noe motivasjon for å sette meg inn i koding
men motivasjonen kom tilbake senere i prosjektet da jeg innså hvor viktig dette er å lære. W3schools.com har vært et hjelpemiddel jeg har prøvd å lære av, men
jeg har uten tvil lært mest av mine gruppemedlemmer samt ulike læringsvideoer på youtube.com.
Javascript har jeg enda ikke lært meg, men målsetter meg å få en grei forståelse for dette før jul.

#### Zeyd
Hva jeg har lært, hvordan (med kilder), hvilken betydning det hadde for prosjektet. Hva jeg ville gjort annerledes. Hvilke kilder/ressurser som virket bedre enn andre. Foretrukket læringsmetode; forelesning, gruppe-undervisning, par-programmering, undersøke på egenhånd, undervise/forklare til andre.

#### Truls
Hva jeg har lært, hvordan (med kilder), hvilken betydning det hadde for prosjektet. Hva jeg ville gjort annerledes. Hvilke kilder/ressurser som virket bedre enn andre. Foretrukket læringsmetode; forelesning, gruppe-undervisning, par-programmering, undersøke på egenhånd, undervise/forklare til andre.

#### Magnus
Hva jeg har lært, hvordan (med kilder), hvilken betydning det hadde for prosjektet. Hva jeg ville gjort annerledes. Hvilke kilder/ressurser som virket bedre enn andre. Foretrukket læringsmetode; forelesning, gruppe-undervisning, par-programmering, undersøke på egenhånd, undervise/forklare til andre.

#### Marius
Hva jeg har lært, hvordan (med kilder), hvilken betydning det hadde for prosjektet. Hva jeg ville gjort annerledes. Hvilke kilder/ressurser som virket bedre enn andre. Foretrukket læringsmetode; forelesning, gruppe-undervisning, par-programmering, undersøke på egenhånd, undervise/forklare til andre.

#### Eirik
I løpet av arbeidsperioden på How We Roll-oppgaven så har jeg lært grunnleggende koding. I HTML, CSS og javaScript. I starten fokuserte jeg mest på HTML og CSS siden disse var de mest elementære, og letteste og lære. Det var først etter halvveis gjennom prosjektet jeg begynte å se på javascript. Javascript virket veldig mye vanskeligere enn de to første språkene, men etter øving og anvending kommer det litt lettere. Jeg driver fortsatt å lærer alle tre språkene, men javascript har fått mer vekt nå nylig og fremover.

Jeg brukte aller først developer.mozilla.org, men syntes de var litt vanskelig å komme inn i, for en komplett nybegynner som meg selv. Dermed brukte jeg w3schools først, siden de gikk mer gjennom det grunnleggende rolig og strukturert. Etterhvert som jeg lærte mer gikk jeg derimot tilbake til mdn web docs. Der var det mer demonstrasjon og implementering av kode, enn bare å lære syntax og begreper. Følte jeg lærte mer med dette, og hvis jeg skulle gjort noe annerledes, hadde det vært å prøvd litt hardere på mdn web docs i starten.

Jeg syntes alle undervisningsformene førte til et helhetlig godt læringsmiljø for min del. I starten var forelesningene litt forvirrende og vanskelig å følge med på. Spesielt med tanke på at jeg ikke hadde noe erfaring med kode, og at de som hadde det stilte veldig kompliserte spørsmål om ting vi ikke hadde lært enda. Gruppearbeidet hjalp ved å gi et miljø hvor noen hadde erfaring og andre ikke. Dette senket skuldrene litt og det å få hjelp fungerte veldig godt. Var litt forvirring i starten om vi skulle kode eller ikke. Dette gjorde at jeg ikke tok det å lære med kode like seriøst, men jeg prøvde å kode litt hver dag uansett.

Det å undersøke på egenhånd var vanskelig i starten, jeg ante ikke hvilke sider som var nyttige og hva jeg burde fokusere på. Det at det var forvirring om hvorvidt vi skulle kode eller ikke hjalp ikke særlig. Etterhvert gikk det mye bedre og det å kode selv ga en stor mestringsfølelse, når det ikke gjorde det følte jeg alltid det var lav terskel for å spørre dagen etter i gruppe eller til lærer.


#### Oppgavebeskrivelse
Liste over innhold/besvarelser i HowWeRoll-oppgaven:<br>
- Opprette en hovedside/hjemmeside som ligger på github-pages<br>
- LHWR01: index.html med visittkort og hyperlenker til how-we-roll.html og hwr-report.html<br>
- LHWR02: how-we-roll.html med form-elementer for kartlegging av gruppemedlemmer. Send/lagre knapp <br>
- LHWR03: hwr-report.html med visualisering av data fra how-we-roll.html<br>
- LHWR04: HWR-GRUPPE-8A.md (leveres i PDF format).<br>
- LHWR04a: Dokumentere analyse- og designprosessen fra brukerhistorier gjennom papir-prototyper/”mocups”, “wireframes” til kode i HTML og CSS. Dokumentasjon skal være i Markdown format og også tilgjengelig i deres hovedrepository i Github.<br>
-LHWR04b: HWR-GRUPPE<gruppe-id>.md skal inneholde et sammendrag av deres arbeid med “How We Roll”-oppgaven. Dere skal så konsist som mulig beskrive hva dere gjorde for å besvare oppgaven. For eksempel, hvordan organiserte dere dere, hvordan dere tok i bruk verktøy og hva som fungerte bra, minde bra og dårlig? Hvilke regler dere satt for bruke av hovedrepository og hvordan fungerte disse? Hvordan sørget dere at alle lærer grunnleggende programmering i HTML og CSS (arbeid i par, arbeid med alle, individuelt arbeid osv.)? Detaljerte beskrivelser relatert til design av deres programmer (koding), kan dere vurdere å legge inn i koden.<br>
	- LHWR04c: Innhold i Markup-fil:<br>
	(1) at alle har bidratt tilstrekkelig til arbeidet med oppgaven,<br>
	(2) at alle kilder dere har brukt er det blitt referert til,<br>
	(3) om dere tillater oss å bruke deres arbeid i undervisning i fremtiden og<br>
	(4) hyperlenkene til deres Github hovedrepository og deres hjemmeside.<br>
- LHWR05: Bruke GitHub-Project med Kanban oppsett + alle har rimelig antall commits i prosjektet<br>
- Endelig leveranse bør sjekket opp mot https://validator.w3.org/<br>


