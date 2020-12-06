---
Title: Kmom05
Description: Report for kursmomenten page.
Template: kmom
---

Kmom05
==================

<div class="embed-container">
    <iframe src="https://www.youtube.com/embed/2aVbW-bnnEA" frameborder="0" allowfullscreen></iframe>
</div>
<br>

### Berätta kort om erfarenheterna med din undersökning av webbplatsers laddningstid och vad du kom fram till.

Användningarna av dev tools network och chroms inbyggda lighthouse funkade bra, lite otydligt på vad dem olika enheterna (Transferred/Resources) betydde, men en google sökning så fixade det sig. Men att ta sig fram till sina resultat var inte så svårt. Roligt att kunna se hur och vad som laddas och vad som kan vara felet på grund av det. Dem sidorna jag genomsökte hade bättre performance på desktop än mobile, men dem lyckades få bättre storlekar och laddningstid (förutom volvo). Volvo var bäst, men alla kunde uppgradera sina mobila enheters sidor.

### Har du några funderingar kring Cimage och dess nytta och features? Vilka bildverktyg använder du själv normalt sett?

Kan vara en nytta att förstå sig på Cimage lite mer, just nu så vet jag bara att den är där, och den ändrar på aspect ration. Om jag skulle göra en egen image skärning, sänka resolution/ändra höjd så hade jag använt mig av photoshop och ändrat på bilden på sånt sätt.

### Vad är din egen allmänna uppfattning kring bilder för webben, nedladdningstider, responsiva bilder och allmänt kring bildbehandling för webben?

Bilder spelar stor roll, men att välja rätt är också en stor del. En fotograf med en collage av sina bilder eller en app som instagram behöver ha en bra scale på sina bilder annars hade det tagit för lång tid att ladda sidan. Val av när det ska laddas och hur många är också en bra ide, vänta tills användaren kommer till sista/näst sista raden av bilder innan man läser in x antal mer bilder. Videos är samma sak, bara att det mesta väntar med att ladda videon tills man har klickat den. Så ja bilder har stor spel på hur en sida laddar bra. I min analys så såg man också att det var mycket koder som låg över som aldrig blir använd också.

### Vilken är din TIL för detta kmom?

Defer offscreen images är ett smart sätt att ladda bilderna, funkar bra med allt som inte har med huvud sidans introduktion att göra med.
