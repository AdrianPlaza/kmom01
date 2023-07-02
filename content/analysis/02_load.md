KMOM05 Bild
=======================

Detta är en rapport på tre webbplatser laddningstid.

<div class="line"></div>

Jag har valt tre webbplatser att jämföra laddningstiden på. Den första webbplatsen är "https://www.youtube.com/", vilket jag valde som ett exempel på en krävande hemsida då den behöver ladda in en massvis av saker som t. ex thumbnails, titlar, uppladdningsdatum och mycket mer. Den andra sidan är "https://dbwebb.se/", vilket jag valde för att det är nästan motsatsen mot den första och det jag menar med det är för att det är inte för mycket på sidan jämfört med t. ex "https://www.youtube.com/". Den sista jag valde var "https://www.amazon.se/" för att den är lik youtube i dess uppbyggnad på ett vis, d.v.s att det finns artiklar med bild och titlar men istället för t. ex uppladnings datum finns det istället priser och hur många det finns i lager.

<div class="line"></div>

Jag använde mig av sidan "https://pagespeed.web.dev/" för att samla in mina matvärden. De matvärdena jag samlade in var under kategorin "Upptäck vad de faktiska användarna upplever" vilket är samling av mängder av data från användare som visas under i ett spreadsheet jag skapade där det finns både för dator och mobil.

<iframe class="spreadsheet-kmom05" aria-label="spreadsheet" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vSMbTjuf2Vza9QJtK-0ksqyBbsIhICOLK-XTkg3hngEvXvs7K2-_bXiFG29QvQMB20wu5qewLqhpqwl/pubhtml?widget=true&amp;headers=false"></iframe>

<div class="line"></div>

## 1. https://www.youtube.com/

<picture>
    <source media="(min-width: 668px)" srcset="../image/youtube.jpg?w=1000">
    <source media="(min-width: 376px)" srcset="../image/youtube.jpg?w=333">
    <img src="../image/youtube.jpg?w=375" alt="youtube homepage">
</picture>

Youtube har väldigt dålig laddningstid och det kan bero på att de laddar in resurser med de största fil storlekarna då det ligger på 14,5mb med 67 resurser, jag tror om de drog ner kvalitén på thumbnail bilderna skulle då sidan kunna ladda in en bra bit snabbare.

## 2. https://dbwebb.se/

<picture>
    <source media="(min-width: 668px)" srcset="../image/dbwebb.jpg?w=1000">
    <source media="(min-width: 376px)" srcset="../image/dbwebb.jpg?w=333">
    <img src="../image/dbwebb.jpg?w=375" alt="dbwebb homepage">
</picture>

dbwebb laddas in snabbast av allihopa av sidorna vilket förmodligen bara beror på att den är väldigt tom som en startsida jämfört med de andra två, sidan laddar även bara in två bilder och en av de är själva dbwebb loggan, jag tror inte det finns för mycket man kan göra för att snabba upp sidan.

## 3. https://www.amazon.se/

<picture>
    <source media="(min-width: 668px)" srcset="../image/amazon.jpg?w=1000">
    <source media="(min-width: 376px)" srcset="../image/amazon.jpg?w=333">
    <img src="../image/amazon.jpg?w=375" alt="amazon homepage">
</picture>

Amazon är nog den bästa av sidorna när det kommer till och ladda in, inte för att den gör det snabbast men till skillnad från dbwebb som laddar in 282kb så laddar Amazon in 8,6mb och sidans laddningnstid är ändå mycket närmre till dbwebb än vad den är youtube då dbwebb:s LCP ligger på 
0,4s medans Amazon:s LCP ligger på en stadig 1,5s och youtube på en tragisk 5,6.

<div class="line"></div>

Från min undersökning har jag kommit fram till att ju fler bilder du har på själva sidan som behövs laddas in desto högre kommer laddningstiden bli, vilket man kan se på alla tree webplatserna jag valt då dbwebb var snabbast och youtube var den med högst laddningsttid. Det är inte bara hur många bilder utan vad filstorleken på bilderna är, vilket man ser bra på amazon jämfört med youtube där amazon laddar in 270+ resurser vilket är 8,6mb och youtube laddar in 60+ fast youtube:s storlek på resurser är 14,5mb. Detta visar att om man redigerar sina bilder tillräckligt mycket så kommer man få en betydligt bättre laddningstid.

Nu när jag har gjort min undersökning har jag kommit fram till att amazon är den bästa av sidorna när det kommer till optimering då den har 30 gånger så stor filstorlek som dbwebb fast bara 1,1 sekunder längre LCPf. Sedan är det dbwebb på andra plats då den laddas in fint och bra även fast den inte är så full av innehåll på startsidan. Sist är youtube då det känns som att de inte har optimerat thumbnail bilderna bra överhuvudtaget då det laddar in dubbla filstorleken som amazon men tar 4,1 sekunder längre för LCP, när jag öppnar hinner jag se rutorna för videorna i ungefär 1 sekund innan de ens har laddat in något annat.

Om jag personligen skulle få bestämma är nog är nog den högsta FCP som hemsidor kan ha innan jag börjar ifrågasätta omsidan har för mycket trafik är nog 2-2,5 sekunder. Om det tar längre tid än så att bara se någonting ladda in på hemsidan så tycker jag att de borde investera i att optimera sin laddningstid. Alla sidorna jag har valt ligger under min absolute gräns jag har för sidor att ladda in så jag bryr mig inte riktigt när jag går in på de och en av sidorna vilket i detta fallet är youtube har lägre LCP på själva videor än vad det har på sin rekommenderade sida.

<div class="line"></div>

Övrigt
-----------------------
Jag jobbade inte i en grupp