# Hoofdstuk 11 – Python wordt geboren

## DEEL V: DIGITALE PIONIERS (1975–2000)
*Het internet vindt zijn weg naar de Lage Landen*

---

Amsterdam, december 1989. Het is de kerstvakantie. Guido van Rossum, 33 jaar oud, programmeur bij het Centrum Wiskunde & Informatica, heeft vrij.

Hij is een beetje verveeld.

Hij heeft een idee voor een nieuwe programmeertaal — al een tijdje. Iets dat eenvoudiger is dan C, eleganter dan BASIC, krachtiger dan de shell-scripts die Unix-gebruikers in elkaar plakken. Iets dat leesbaar is voor mensen, niet alleen voor machines. Iets dat je direct kunt gebruiken: typ een opdracht, zie het resultaat.

Hij noemt het, min of meer willekeurig, Python — naar Monty Python, de Britse comedygroep, niet naar de slang.

De kerstvakantie verstrijkt. Python is geboren.

---

### De filosofie van de eenvoud

Van Rossum was geen typische hacker. Hij was niet de man die door de nacht schreef en op drankjes en opwinding draaide. Hij was methodisch, bedachtzaam, en gefocust op een eigenschap die de meeste programmeurs als luxe beschouwden: leesbaarheid.

Code, betoogde Van Rossum, wordt veel vaker gelezen dan geschreven. Een programmeur schrijft een functie eenmalig maar leest hem tientallen keren terug — zelf, en anderen. Als die functie moeilijk te lezen is, kost elke herlezing tijd en verhoogt de kans op misverstanden.

Python was ontworpen om dit te verhelpen. De taal dwong structuur af via witruimte: de inspringing van code was niet decoratief maar syntactisch. Een blok code dat bij een if-statement hoorde, moest ingesprongen zijn. Als het niet ingesprongen was, was het niet onderdeel van het blok.

Dit was controversieel. Programmeurs waren gewend aan accolades en begin/end-keywords. Betekenisvolle witruimte voelde willekeurig en fragiel.

Maar het werkte. Python-code zag er uit als pseudocode — als de informele beschrijvingen die programmeurs opschreven als ze een idee uitlegden aan een collega. Het was al bijna begrijpelijk voor mensen die de taal niet kenden.

---

### Het Zen van Python

In 1999 schreef Tim Peters, een van de kernbijdragers aan Python, een tekst die later als een soort grondwet voor de taal zou worden beschouwd: "The Zen of Python". Nineteen aforismen over hoe goede Python-code eruitziet.

Een paar van de meest geciteerde:

*"Beautiful is better than ugly."*
*"Explicit is better than implicit."*
*"Simple is better than complex."*
*"Readability counts."*
*"There should be one — and preferably only one — obvious way to do it."*

Dit laatste aforisme is de meest Dijkstra-achtige: niet veertien manieren om hetzelfde te doen, maar één. Niet maximale flexibiliteit, maar maximale duidelijkheid.

De echo van Dijkstra's filosofie is niet toevallig. Van Rossum had gestudeerd aan de Universiteit van Amsterdam, werkte bij het CWI waar Dijkstra's invloed nog tastbaar was, en was mede gevormd door de Nederlandse informaticacultuur die geloofde in elegantie als een technische deugd.

---

### Van hobby naar wereldtaal

In 1991 publiceerde Van Rossum de eerste versie van Python online. Er was geen grote lancering, geen persconferentie, geen budget. Hij plaatste de broncode op een FTP-server — de manier waarop bestanden in die pre-web-dagen werden gedeeld — en schreef een bescheiden aankondiging op een nieuwsgroep.

De reacties waren positief maar beperkt. Python was interessant, zeiden de programmeurs die het probeerden. Maar C was sneller. En Perl was al populair voor scripting.

Wat volgde was een langzame maar onstuitbare groei. Python vond zijn eerste grote niche in systeembeheer — het automatiseren van taken op Unix-servers. Vervolgens in wetenschappelijk computing: de taal was makkelijk te leren voor wetenschappers die geen professionele programmeurs waren maar wel data moesten verwerken.

In de jaren 2000 vond Python zijn weg naar het web via frameworks als Django en Flask. In de jaren 2010 werd het de standaardtaal voor machine learning en data-analyse, mede dankzij bibliotheken als NumPy, Pandas en TensorFlow.

Vandaag is Python de meest gebruikte programmeertaal ter wereld, volgens vrijwel elke meting die daarvoor bestaat.

---

### Haarlem naar Google naar Microsoft

In 2003 verliet Van Rossum Nederland voor de Verenigde Staten. Hij werkte achtereenvolgens bij Zope Corporation, Google (waar hij zes jaar doorbracht en Python intern enorm populariseerde) en Dropbox. In 2020 kondigde hij zijn pensioen aan — en een half jaar later trad hij in dienst bij Microsoft, aangetrokken door de kans om Python nog verder te integreren in de tools die de wereld gebruikt.

Het is een Hollandse success story met een Amerikaans kapitel. Maar de taal zelf is onmiskenbaar gevormd door Nederlandse waarden: de nadruk op duidelijkheid boven slimheid, op consensus boven eigengereidheid, op het doen wat logisch is.

Python heeft een "benevolent dictator for life" — zo noemde de gemeenschap Van Rossum: de uiteindelijke beslisser over de richting van de taal. Maar de gemeenschap besliste via Python Enhancement Proposals: openbare documenten waarin veranderingen werden voorgesteld, bediscussieerd en uiteindelijk geaccepteerd of afgewezen. Het was, bijna letterlijk, het poldermodel toegepast op softwareontwikkeling.

---

### ABC: de voorloper die niemand kent

Python had een voorvader die nog Nederlandser was: ABC.

ABC was een programmeertaal die was ontwikkeld bij het CWI in de jaren 1980, door Lambert Meertens (een medewerker van Van Wijngaarden) en Steven Pemberton. Ze was ontworpen met hetzelfde doel als Python: een taal die leesbaar was, die fouten makkelijk maakte te vinden, die mensen zonder informaticaopleiding konden leren.

ABC was technisch indrukwekkend. Ze had automatisch geheugenbeheer, een interactieve modus, en een syntaxis die dichter bij het Engels lag dan welke andere taal dan ook.

Ze flopte commercieel. Ze draaide alleen op specifieke computers. Ze was moeilijk te extensen. En ze werd nooit open source.

Van Rossum had als promovendus bij het CWI aan ABC gewerkt. Toen hij Python begon, nam hij de beste ideeën van ABC mee en voegde toe wat ABC miste: uitbreidbaarheid, openheid, draagbaarheid naar elke computer ter wereld.

Python is ABC plus de lessen van ABCs mislukking. Zonder ABC geen Python. En ABC is een CWI-product — een directe lijn van Van Wijngaarden naar Van Rossum.

---

### De taal die AI begrijpelijk maakte

Er is één bijdrage van Python die het meest consequenties heeft voor de wereld van vandaag: het maakte kunstmatige intelligentie toegankelijk.

Machine learning — het trainen van modellen op grote hoeveelheden data — vereiste jarenlang gespecialiseerde kennis van C++ en FORTRAN-gebaseerde wiskundebibliotheken. Alleen ervaren programmeurs met een achtergrond in computerwetenschappen konden erbij.

Python veranderde dat. De NumPy-bibliotheek maakte matrixberekeningen eenvoudig. Scikit-learn maakte klassieke machine-learningalgoritmen één-lijners. TensorFlow en PyTorch — de bibliotheken achter moderne deep learning — kozen Python als hun primaire interface.

Het resultaat: een bioloog kan vandaag in een middag een model trainen om celbeelden te classificeren. Een econoom kan een dataset analyseren zonder een computerwetenschapper in te huren. Een journalist kan overheidsdata doorzoeken zonder te programmeren.

Python democratiseerde AI. Een taal die in Amsterdam was bedacht in de kerstvakantie van 1989, door iemand die zich verveelde, is nu het gereedschap waarmee de mensheid haar meest complexe modellen van de werkelijkheid bouwt.

---

### De andere digitale Nederlanders

Van Rossum was niet de enige Nederlander die in de jaren tachtig en negentig het internet mee vormgaf.

Piet Beertema, een netwerkspecialist bij het CWI, was in 1988 de eerste Europeaan die een stuk van het vroege internet aan een instituut verbond buiten de VS. De verbinding liep van het CWI naar een computernetwerk aan de NSF in de VS — de eerste Europese verbinding met wat het internet zou worden. Nederland was er vroeg bij.

Mark Overmars, hoogleraar informatica in Utrecht, ontwikkelde in de jaren negentig Game Maker — een programmeromgeving waarmee mensen zonder programmeerkennis eenvoudige spellen konden maken. Het was, lang voor de App Store en Steam, een poging om spelontwikkeling te democratiseren. Honderdduizenden mensen leerden programmeren via Game Maker; enkele daarvan groeiden uit tot serieuze spelontwikkelaars.

Arjen Kamphuis en Rop Gonggrijp — de laatste bekend van de Chaos Computer Club — waren sleutelfiguren in de vroege Nederlandse internetgemeenschap, die een cultuur van openheid, technische excellentie en maatschappelijk bewustzijn had die sterk aan de Leidse traditie van vrij denken herinnerde.

---

*→ Verder naar [Hoofdstuk 12: Van PTT naar KPN](deel5_h12.md)*
