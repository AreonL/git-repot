---
Title: Design och webbplatser
Description: Analysis for Design och webbplatser page.
Template: analysis
---
Design och webbplatser
=======================
 
Uppgiften "Uppdrag 6: Analys valfri" utgår på att jag ska välja ett av det analysteman från kursmomenten 4-6. Jag valde kmom05, Bilder och laddningstider. Där dokumentera jag kmom10 webbsidans laddningstid och användbarhet och sedan komma fram till om det finns förbättringar inom webbsidan.
 
Urval
-----------------------
 
Urvalet är min egna sida som jag har skapat som ska analyseras. Jag väljer att göra alla huvud sidorna Home, About och Highlight. 
 
Metod
-----------------------
 
Jag valde att spara alla mina mätningar i ett Excel-ark via Google Kalkylark. Jag använder mig av devtools, nätverk tabben och lighthouse tabben inom devtools för att få fram mina mätningar. Jag använder mig av devtools funktion 'disable cache' för att få osparade filer vid varje laddning. Mobil inställning på devtools använder jag mig av iPhone X.
 
Resultat
-----------------------
 
Här kan vi hitta Exel-arket med resultaten: <a href="https://docs.google.com/spreadsheets/d/1_8lW5V-ue-cDH-R-VQQUk2FeGE70s9GfNWaRSybsRAI/edit?usp=sharing">Exel-ark</a>
<br/>
 
### Home
<br>
 
![Screenshot of Home](../content/analysis/img/home.png)
 
Lighthouse devtoolen gav Home 75 performance poäng på desktop och 64 på mobile. Det som är det två stora problem på Homes sida är resize på Flash bilden och ändra bilderna så det är next-gen format, som JPEG och WebP format. De kan spara laddningstid och cellular data.
 
Det tog Home 1.35s att laddas in och är klar på 1.35s, sidan är 5.8mb stor och skickar 5.8mb compressade filer. Homes mobil är snabbare och mindre, det tar 794ms att laddas in och är klar på 788ms, sidan är 3.8mb stor och skickar 3.7mb compressade filer.
 
### About
<br>
 
![Screenshot of About](../content/analysis/img/about.png)
 
Lighthouse devtoolen gav About 75 performance poäng på desktop och 67 på mobile. Det som är det tre stora problem på About sida är resize på Flash bilden och ändra bilderna så det är next-gen format. Mobile har ett eget problem som är att ta bort resources som blockar renderingar. 
 
Det tog About 1.46s att laddas in och är klar på 1.45s, sidan är 6.3mb stor och skickar 6.2mb compressade filer. Abouts mobil är snabbare och mindre, det tar 866ms att laddas in och är klar på 859ms, sidan är 3.8mb stor och skickar 3.8mb compressade filer.
 
### Highlight
<br>
 
![Screenshot of Highlight](../content/analysis/img/highlight.png)
 
Lighthouse devtoolen gav About 75 performance poäng på desktop och 64 på mobile. Det som är det tre stora problem på About sida är resize på Flash bilden och ändra bilderna så det är next-gen format. Mobile har ett eget problem som är att ta bort resources som blockar renderingar. 
 
Det tog Highlight 1.88s att laddas in och är klar på 1.87s, sidan är 8.4mb stor och skickar 8.3mb compressade filer. Highlights mobil är lite mer än dubelt så snabbare och mindre, det tar 909ms att laddas in och är klar på 902ms, sidan är 4mb stor och skickar 3.9mb compressade filer.
 
 
Analys
-----------------------
 
Alla tre sidor har en bättre performance score på desktop än mobila enheter. About sidan har en smula bättre performance på mobilen än va det andra två sidorna har. Laddningstiderna ökar när storleken av filer som skickas på sidan ökar. Laddningstiderna är mindre på mobile än desktop. Den snabbaste sida på mobile är Home, detta kan bero på antalet av filer som skickas samt total storleken som skickas. Det största laddnings beroendet är Flash bilden och att bilderna inte är next-gen formaterat. Både About och Highlights mobile laddning behöver ta bort resources som blockar renderingar av sidan, där behöver man ladda det kritiska resurser (js/css) först sen ladda det icke-kritiska.
 
1: Home<br>
2: About<br>
3: Highlight<br>
 
Home vinner, men skillnaden är inte stor. Det som får Home att vinna är den är det snabbaste sidan på sin laddningstid/total. Den effektivaste sida från desktop till mobile är Highlight, eftersom den halverar sin laddningstid och storleken på laddningen. Även om den är långsammaste så har den ändå en effektivitet på 50% mellan desktop och mobile.
 
Den gräns för laddnings tid som jag har valt är runt 2 sekunder. Man märker av det vid 2 sekunder, men är inte irriterad av det. Efter 2 sekunder så upplever jag sidan för långsam och kan få mig själv att undra om det är mitt internet eller dator/mobil som laggar. Så runt/under 2 sekunder är en bra tid. Man ser när man laddar alla sidorna att det tar sin tid för flash bilden att ladda in. About har en bild mer än Home, så naturligt så tar det lite längre, samma med Highlight som har två mer bilder än Home. Så fixa laddningen för flash bild och ändra bildens format till next-gen format som WebP och JPEG.
 
 
Övrigt
-----------------------
 
Skriven av: Areon lundkvist
 


