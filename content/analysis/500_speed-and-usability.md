##Speed and usability

I kursmoment 4 när vi analyserade färgval valde vi ut 4 hemsidor att analysera. Vi valde helt enkelt att expandera analysen av dessa sidor genom att fortsätta med dom denna vecka. I testet har vi Karlskrona Hockey, Volvo, Vapiano och McDonalds. Mätningarna har gjorts enligt uppgiften, att mäta laddningshastighet i devtools genom att ladda sidan och notera resultatet, för att sedan notera sidans poäng i Google Pagespeed, både mobile och desktop.


### KHK.SE

Laddningstid:   43s
GPS-Mobile:     62/100
GPS-Desktop:    47/100

KHKs sida är onödigt stor. Bilder är inte optimerade för den storleken dom visas, vilken och är GPS första åtgärdspunkt för desktop. GPS vill också att KHK ska ta bort javascript i början av sidan. Sidan tog jättelång tid att ladda pga sin storlek och att den har ca 230 requests under laddningen.


### VOLVOCARS.SE

Laddningstid:   25s
GPS-Mobile:     45/100
GPS-Desktop:    65/100

Volvos sida är även den mycket stor. Åtgärder som kan göras inkluderar att minifiera css, html och javascript. Även här tycker GPS att man skall ta bort javascript i början av sidan. GPS tycker också att Volvo skall utnyttja cache-lagring i webbläsaren och aktivera komprimering. Trots att sidan är större är KHKs sida så är laddningstiden nästan halverad vilket kan bero på att antalet requests är mindre än hälften av KHKs, nämligen ca 100 till antalet.


### VAPIANO.SE

Laddningstid:   5s
GPS-Mobile:     42/100
GPS-Desktop:    53/100

Vapiano var den den sida som hade snabbast laddningstid i testet och bara 14 requests. Trots detta fick den totalt sett sämst av alla i GPS-testet. Åtgärder inkluderar som i dom tidigare sidorna att ta bort javascript i början av sidan samt att aktivera komprimering. Även minifiering av all kod rekommenderas samt optimering av bilder. GPS klagar även på sidan redirects.


### MCDONALDS.se

Laddningstid:   12s
GPS-Mobile:     46/100
GPS-Desktop:    60/100

McDonalds sida hade en helt ok laddningstid jämfört med dom andra deltagarna och har 46 requests. GPS-poängen var även den helt ok i jämförelse. McDonalds sida representerar mycket bra alla problem dom andra sidorna har enligt GPS. Detta inkluderar minifiering av all kod, optimering av bilder, ta bort javascript i början av sidan samt att undvika redirects.


### SAMMANFATTNING

Enligt GPS var det nästan samma åtgärdsförslag på alla sidor. Dessa var minifiering av all kod, optimering av bilder, ta bort javascript i början av sidan, samt att undvika omdirigeringar. Man kan tycka att vissa av dessa saker kan vara jätteenkla att fixa till och det får mig att undra varför företag av den kalibern inte redan har gjort det. Kanske det finns anledningar varför man väljer att ha script i början av en sida, t.ex facebook-integreringar, eller att man har redirect för att man har flera lokala domäner som alla länkar till en sida som egentligen är samma. Optimering av bilder och minifiering har jag dock svårare att hitta en motivering varför man inte har gjort just det men har man tur är det kanske ett framtida jobb för en framtida webdesigner. Något jag tycker var väldigt tydligt i detta test är sambandet mellan laddningstid och requests. Jag som har gjort testet med en Gbit-uppkoppling upplever att det är snarare hur många nedladdningar som skall göras snarare än mängden. Detta visar sig tydlugast mellan KHK och Vovlo där KHKs sida var 20% mindre än Volvos men laddningstiden och requests över det dubbla. Personligen tycker jag alla dessa sidor laddade för långsamt men det kan även bero på externa omständigheter så dom sin egen datorprestanda och om man har många krävande program/sidor igång samtidigt, t.ex Google Hangouts. För att en sida skall upplevas som snabb tycker jag en laddningtid bör ligga under en sekund och för den där riktigt sköna ssd-känslan skall man gärna ner på 0.2 sekunder.

Meddeltagare i testet var:

Ann
Christofer
Jacob
Marcus
Nicklas
