# Hoofdstuk 9 – Dijkstra's twintig minuten

## DEEL IV: WEDEROPBOUW EN DE GEBOORTE VAN DE COMPUTER (1945–1975)

---

Het is een zomerse ochtend in 1956. Amsterdam drinkt zijn eerste koffie. Op een terrasje in het centrum — Dijkstra zou later zeggen dat het een café was, al herinnert hij de naam niet meer — zit een vijfentwintigjarige wiskundige met zijn verloofde.

Ze zijn op weg naar een meubelzaak, of misschien naar een park — de details wisselen in de verschillende versies van het verhaal, want herinneringen zijn geen computerprogramma's. Maar één ding is zeker: Dijkstra heeft een probleem in zijn hoofd. Hij heeft er al een tijdje over nagedacht. Nu ziet hij de oplossing.

Het probleem is dit: gegeven een netwerk van steden verbonden door wegen, wat is de kortste route van stad A naar stad B?

In twintig minuten, zonder papier, zonder potlood, denkt hij de oplossing uit.

---

### Het probleem van het kortste pad

Het kortste-pad-probleem klinkt simpel. En voor een klein netwerk — vier steden, vijf wegen — is het ook simpel. Je kijkt gewoon naar alle mogelijke routes en kiest de kortste.

Maar hoe groter het netwerk, hoe sneller het aantal mogelijke routes explodeert. Een netwerk van twintig steden heeft al miljarden mogelijke paden. Een netwerk van honderd steden heeft meer mogelijke paden dan er atomen in het heelal zijn. Brute force — alle paden uitproberen — is computationeel onmogelijk.

Dijkstra's inzicht was dit: je hoeft niet alle paden te proberen. Je hoeft alleen slim te zoeken.

Zijn algoritme begint bij de startstad en breidt zich geleidelijk uit naar buiten, steeds de dichtstbijzijnde onbezochte stad bezekend. Op elk moment weet het algoritme wat de kortste bekende afstand is tot elke stad die al is bezocht. Als een nieuwe stad wordt bezocht, wordt die afstand bijgewerkt als er een kortere route beschikbaar is.

Het sleutelwoord is *greedy*: het algoritme maakt steeds de lokaal optimale keuze — ga naar de dichtstbijzijnde stad — en dit levert, zoals Dijkstra bewees, het globaal optimale resultaat op. Je hoeft niet alles te proberen. Je hoeft alleen het juiste te doen op elk moment.

Het algoritme werkt in polynomiale tijd: voor een netwerk met *n* knopen heeft het orde *n²* stappen nodig. Vergelijk dat met de exponentieel groeiende brute-force aanpak. Het verschil is de verschil tussen een rekening die je kunt betalen en een rekening die het universum failliet zou maken.

---

### De man achter het algoritme

Edsger Wybe Dijkstra werd geboren op 11 mei 1930 in Rotterdam. Zijn vader was chemicus, zijn moeder wiskundige — een achtergrond die hij zou omschrijven als ideaal voor iemand die van precisie houdt.

Hij was briljant op school zonder dat het hem veel moeite leek te kosten. Hij overwoog een carrière in de rechten — zijn vader drong erop aan — maar koos uiteindelijk voor theoretische fysica. In Leiden studerend ontdekte hij de informatica — of liever, de informatica ontdekte hem.

In 1952 begon hij als programmeur bij het Mathematisch Centrum in Amsterdam. Hij werkte direct voor Van Wijngaarden. Het was een onwaarschijnlijke combinatie: de rigoureuze theoreticus Van Wijngaarden en de jonge, charismatische Dijkstra die liever nadacht over waarom iets werkte dan over hoe je het moest doen.

In 1956 — het jaar van de café-inval — was Dijkstra 25 jaar oud en al een erkende figuur in de Nederlandse computergemeenschap. Hij had al bijgedragen aan de programmering van de ARMAC, de opvolger van de ARRA. Hij dacht in algoritmen op een manier die zijn collega's verbaasde: altijd op zoek naar het principe achter de methode, de reden achter de stap.

---

### Een algoritme als kunstwerk

Dijkstra publiceerde het algoritme in 1959 in *Numerische Mathematik*, een Duits wiskundetijdschrift. Het artikel was drie pagina's lang. De beschrijving van het algoritme zelf besloeg minder dan een pagina.

Het was bijna provocatief eenvoudig.

Dijkstra geloofde — hij zou dit zijn hele leven blijven herhalen, in lezingen en essays en de legendarische handgeschreven documenten die hij zijn EWD-nummers noemde — dat elegantie een kwaliteitskenmerk is. Niet een luxe, maar een noodzaak.

"Als debugging het proces is van het verwijderen van bugs," schreef hij ergens in de jaren zeventig, "dan moet programmeren het proces zijn van het introduceren ervan." De grap had een serieuze kern: code die simpel is, heeft minder bugs. Code die elegant is, is makkelijker te begrijpen. Code die begrijpelijk is, is makkelijker te onderhouden. En onderhoud is 90% van de levensduur van software.

Dijkstra's algoritme is elegant. Het heeft geen onnodige stappen. Elk element doet precies wat het moet doen. Het is zo compact dat het in een paar regels pseudocode kan worden opgeschreven, en zo krachtig dat het de basis is van vrijwel elk routealgoritme dat vandaag de dag bestaat.

---

### Van café naar GPS

Welke route het u ook maakt — op uw telefoon, in uw navigatiesysteem in de auto, in de routeplanner op de website van de NS — ergens in de berekening zit Dijkstra's algoritme, of een variant erop.

Google Maps gebruikt een combinatie van Dijkstra's algoritme en A*, een verfijnde versie die gebruik maakt van heuristieken om nog sneller te zoeken. OpenStreetMap, de open kaart die door vrijwilligers wordt gebouwd en door duizenden toepassingen wordt gebruikt, doet hetzelfde.

De pakketbezorger die uw bestelling optimaal routeert. Het vliegtuig dat zijn vluchtpad bepaalt. Het IP-pakket dat via duizenden routers zijn weg zoekt naar uw computer. Al deze systemen lossen varianten op van het kortste-pad-probleem. Al deze systemen staan op de schouders van een vijfentwintigjarige wiskundige die op een zomerochtend in Amsterdam iets inzag dat zijn verloofde kon wachten.

---

### GOTO is schadelijk

Dijkstra's tweede grote bijdrage was misschien nog invloedrijker, maar is minder bekend buiten de computerwetenschappelijke wereld.

In 1968 stuurde hij een brief aan de Communications of the ACM — het toonaangevende tijdschrift voor computerwetenschappers. De brief was getiteld: "Go To Statement Considered Harmful."

De GOTO-instructie was in die jaren een van de meest gebruikte in programmeercode. Het stelde programmeurs in staat om op elk willekeurig punt in een programma te springen — een soort teleporter voor code. Het was krachtig. Het was flexibel. Het was ook een ramp.

Programma's met veel GOTO-instructies werden al snel onleesbaar. De uitvoering sprong heen en weer door de code op een manier die niemand meer kon volgen, zelf de programmeur niet. Dit was "spaghetti code" — een term die in die jaren werd gemunt — en het veroorzaakte bugs die bijna onmogelijk te vinden waren.

Dijkstra betoogde in zijn brief dat GOTO nooit nodig is. Dat alle programma's konden worden geschreven met drie eenvoudige controlestructuren: sequentie (doe A, dan B), keuze (als X, doe A, anders doe B) en herhaling (blijf A doen zolang X waar is). Dit is gestructureerd programmeren.

De reacties waren heftig. Sommige programmeurs voelden zich aangevallen. GOTO was hun gereedschap, en nu zei een Nederlandse theoreticus dat ze het verkeerd gebruikten?

Maar Dijkstra had gelijk. In de decennia die volgden, verdween GOTO uit vrijwel alle moderne programmeertalen. Python heeft geen GOTO. Java heeft geen GOTO. JavaScript heeft geen GOTO. De brief van drie pagina's veranderde hoe de wereld programma's schrijft.

---

### De filosoof van het algoritme

In 1972 won Dijkstra de Turing Award — het equivalent van de Nobelprijs in de informatica. In zijn acceptance speech zei hij iets wat veel van zijn toehoorders verbaasde: "Computerwetenschappers moeten meer filosofen worden, niet minder."

Hij meende het. Dijkstra geloofde dat de grondslagen van de informatica niet technisch maar wiskundig en filosofisch waren. Dat de vraag hoe een programma correct is — niet waarschijnlijk correct, maar bewezen correct — net zo fundamenteel was als de vraag of een wiskundig bewijs klopt.

In de late jaren zeventig en tachtig werkte hij aan formele methoden voor programmacorrectie: wiskundige technieken om te *bewijzen* dat een programma doet wat het moet doen. Het was abstract werk, ver van de dagelijkse praktijk van softwareontwikkeling.

Maar de principes die hij formuleerde — denk na over de eigenschappen van je programma voordat je het schrijft, bewijz dat je algoritme klopt voordat je het implementeert — zijn nog steeds de basis van de beste softwareontwikkelpraktijken.

Elke keer dat een moderne programmeur een "unit test" schrijft — een klein programmaatje dat controleert of een functie doet wat ze moet doen — handelt ze in de geest van Dijkstra.

---

### Eindhoven en de American Graffiti

In 1984 verhuisde Dijkstra van de TU Eindhoven — waar hij hoogleraar was geworden — naar de Universiteit van Texas in Austin. Hij emigreerde, deels vanwege de grotere middelen in de Verenigde Staten, deels vanwege een teleurstelling over de Nederlandse academische cultuur die hij nooit helemaal articuleerde.

Maar hij bleef schrijven. De EWD-documenten — handgeschreven op papier, gefotokopeerd en verspreid, later gescand en online gezet — gingen door tot kort voor zijn dood in 2002. In totaal zijn er meer dan 1.300, over onderwerpen die variëren van algoritmische puzzels tot bittere observaties over de staat van de informatica-opleiding.

Hij stierf op 6 augustus 2002 in Nuenen, Noord-Brabant, het dorp waar hij zijn pensioen doorbracht. Zijn laatste EWD-document schreef hij een paar weken voor zijn dood.

Op zijn grafsteen staat: "Simplicity is a great virtue but it requires hard work to achieve it and education to appreciate it. And to make matters worse: complexity sells better."

---

### Het algoritme dat altijd loopt

Terwijl u dit leest, voert ergens een computer een kortste-pad-berekening uit. Misschien in een datacenter in Iowa, misschien in een telefoon in uw zak, misschien in een server in Japan. Elke seconde worden er miljoenen van deze berekeningen uitgevoerd, voor navigatiesystemen, voor netwerken, voor logistieke platforms.

Ze lopen allemaal op een idee dat een vijfentwintigjarige Nederlander bedacht in twintig minuten, op een zomerochtend in Amsterdam, zonder papier, zonder potlood.

Dat is de kracht van het juiste idee op het juiste moment.

---

*→ Verder naar [Hoofdstuk 10: Philips en het tijdperk van de cassette](deel4_h10.md)*
