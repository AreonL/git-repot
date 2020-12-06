---
Title: Load
Description: Analysis for color page.
Template: analysis
---

Laddningstid
=======================

Uppgiften "Utvärdera webbplatsers laddningstid och användbarhet" ut går på att jag ska dokumentera olika webbsidors ladningstid och användbarhet och sedan komma fram till om det finns förbättringar innom webbsidan.

Urval
-----------------------

Jag har valt att utvärdera Volvo, Tesla och Ferrari. Detta tre valen är baserade på olika pris nivåer för användning av en liknande produkt. Tanken är att se vilket företag som har mest optimalitet men under samma produkt.

Metod
-----------------------

Jag valde att spara alla mina mätningar i ett Excel-ark via Google Kalkylark. Jag använder mig av devtools, nätverk tabben och lighthouse tabben innom devtools för att få fram mina mätningar. Jag använder mig av devtools funktion 'disable cache' för att få osparade filer vid varje laddning. Mobil inställning på devtools använder jag mig av iPhone X.

Resultat
-----------------------

Här kan vi hitta Exel-arket med resultaten: <a href="https://docs.google.com/spreadsheets/d/1zDGP5_jE3JwBMe1tN5WqlqdFFTJMAVOfvUMyeEAhBDo/edit?usp=sharing">Exel-ark</a>
<br/>

### Volvo
<br>

![Screenshot of Volvo](../content/analysis/img/volvo.jpg)

Volvo's sida tar 1.48s att laddas in och klar på 2.55s, sidan är 4.7mb stor och skickar 2.3mb compressade filer. Sidans mobil och desktop mäts med respektiva resultat.
Lighthouse gav Volvo en performance av 82 på desktop men 26 på mobile. Det som är det två stora problem på Volvos mobil sida är resize på bilderna, de kan spara laddnings tid och cellular data. Det andra som kan fixas är att ta bort JavaScript som inte används, detta sänker storleken på sidan. Desktop så har Volvo samma problem, men inte lika illa som mobile.


### Tesla
<br>

![Screenshot of Tesla](../content/analysis/img/tesla.jpg)

Tesla's sida tar 2.41s att laddas in och klar på 6.57s, sidan är 8.6mb stor och skickar 5.4mb compressade filer. Sidans mobil är snabbare och mindre, den skickar 2.7mb av sin storlek på 6.0mb och tar 883ms att ladda och är klar på 6.74s.
Lighthouse gav Tesla en performance av 60 på desktop men 30 på mobile. Det största ändringarna på mobile för Tesla är att ta bort oanvänd Css och JavaScript samt 'Defer offscreen images', ladda bilderna efter det viktiga komponenterna har laddats. På desktop så gäller att ta bort oanvänd Css och resize på bilder, samt 'Defer offscreen images'.

### Ferrari
<br>

![Screenshot of Ferrari](../content/analysis/img/ferrari.jpg)

Ferrari's sida tar 2.31s att laddas in och klar på 5.28s, sidan är 30.4mb stor och skickar 20.3mb compressade filer. Sidans mobil är snabbare och mindre, den skickar 10.8mb av sin storlek på 21.0mb och tar 1.71s att ladda och är klar på 4.21s.
Lighthouse gav Ferrari en performance av 48 på desktop men 6 på mobile. Det största ändringarna på mobile för Ferrari är att ta bort oanvänd JavaScript, JavaScripten tar upp 3ggr så mycket laddnings tid än nästa problem som är 'Defer offscreen images'. Ferrari behöver ändra på deras render/resize och format på vissa filer, samt ta bort oanvänd Css. På desktop så gäller att ta bort oanvänd JavaScript.

Analys
-----------------------

Alla tre hemsidor har en bättre performance score på desktop än mobila enheter. Vi kan se att ladnings tiden ökar med fil storlekarna. Både Ferrari och Tesla sänker deras laddnings tid och transfarred/resources som skickas och laddas på sidan blir mindre på mobila enheter, men sida blir klar ungefärligt samma som desktop. Det som sänker alla tre sidor är för det mesta oanvända Css och JavaScript kod. Det andra stora är deras resize och 'Defer offscreen images', där dem behöver vänta tills all kritiska resurser har laddats efter det så kan sidorna ladda in bilderna.

1: Volvo<br>
2: Tesla<br>
3: Ferrari<br>

Volvo vinner nog stort när det kommer till laddnings tid/total, fil storlek och optimisering på desktop. Även om Volvo har dåligar score än tesla på mobil så har den bättre performance med allt annat. Teslas mobil verision är mycket bättre än det andras mobila men det tar ändå lång tid att ladda klart. Ferrari har både dålig score för desktop och mobile.

Min gräns för laddnings tid är runt 2 sekunder. Man ska inte behöva stirra på ingenting men också inte se hur sidorna laddas upp och ha visuella uppstöringar. Volvo passar in i detta, man kan se bilden laddas in men inga konstiga hop i font eller någon font/text som laddas in sent. Tesla och Ferrari har längre laddnings tid och det syns, Tesla har text/knappar/pil som hoppar in efter en stund. Ferrari har en hel täckande svart färg med sin logo som laddnings skärm, efter den så kommer sidan upp, det funkar men känns för mycket, men det är bättre än att vissa fonter eller text hoppar konstigt.


Övrigt
-----------------------

Skriven av: Areon lundkvist
