> SakNet är del av ett grupparbete under Hack for Heritage 2018
> läs mer om de andra idéerna på http://edvind.github.com/h4h2018

# SakNet

Att få en översikt över en museisamling är sällan en lätt uppgift. Ofta är en museisamling oöverskådlig och svårnavigerad om du inte har specialkunskaper eller erfarenhet av den. Idag presenteras samlingar på webben med hjälp av olika gränssnitt där användaren oftast söker sig fram till objekten. Hur kan vi upptäcka eller visa en museisamling på ett alternativt vis?

Idén är kort sagt att presentera samlingen med en interaktiv visuell representation istället för en sökruta.

## För vem?
 - Museianställda som övergripande vill visualisera sina samlingar.
 - Nyfikna som vill upptäcka samlingar på ett nytt sätt.

## Användningsområden
 - Kan upptäcka föremål som har med andra föremål att göra på ett intuitivt vis.
 - Kan skapa en övergripande bild av museisamlingen. Hur stor är gaffelsamlingen i relation till konstsamlingen?

## Användbar data?
Många museisamlingar lider av bristfällig digitisering eller att det inte finns en konsekvent katalogisering. En anledning till detta är att de skrivits in av flera olika människor under lång tid. En klassificering som, åtminstone vid Hälsinglands Museum, använts konsekvent och som täcker i stort sett hela samlingen är den metadata som utgår från ämnesklassifikationssystemet Outline (https://libris.kb.se/bib/7603750). Genom att utgå från denna data kan en bild av en museisamling visualiseras.

## Maskininlärning
För att få en uppfattning om hur alla objekt hör ihop med varandra används maskinlärning. All tillgänglig metadata matas in i systemet och grupperas med tekniken Clustering. 

## Clustering
Typen av maskinlärning som används kallas Clustering. Clustering innebär att man ger en relevanspoäng mellan varje objekt och alla kategorier. Denna poäng används sedan för att avgöra det visuella avståndet mellan punkterna, och därmed punkternas position på kartan. 

## Visualisering
För att ge en bild av hur samlingen skulle kunna presenteras gjorde vi en hastigt hopskriven skiss baserad på en cirkel.
![SakNet](https://github.com/ostwilkens/SakNet/raw/master/SakNet.png)
Den kategoribaserade bilden ger en idé om hur samlingen ser ut och var olika föremål hamnar beroende på hur de relaterar till varandra. Kyrkliga träskulpturer hamnar nära kyrkliga textilier men textilierna hamnar närmre kategorin "textil, skinn och fibrer" än träskulpturerna. På detta sätt kan en person navigera samlingarna. 
