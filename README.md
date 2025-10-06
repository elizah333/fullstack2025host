Skärmdumpar om hur sidan ska se ut: https://foretagsuniversitetetab-my.sharepoint.com/:f:/g/personal/eliza_haglund_studerande-foretagsuniversitetet_se/Eu_qp5RlbIFBpw2s6n8mBUUBVnboU9iUOVZihfjVNtTkhw?e=I63Ko6

Jag ville skapa en sida med en knapp som var en bild av en karaktär. Landade på jaguaren och bestämmde att göra en informations sida om dom. Jag tog mycket inspiration fron andra tiger sidor och speciellt från WWF med hur de designade sina sidor bade på dator och mobil.

Strukturen:
Start/index, leder till andra sidor.
About Jaguar, fakta om arten
Conservatio, information om miljön.
Take action, kundens sätt att delta och lära sig.
Support us, lär dig mer om vad företaget gör och kontakt.

Min index sida använder denna metoden för jaguar kroppsdel knapparna: https://www.w3schools.com/cssref/css3_pr_clip-path.php . Varje kroppsdel leder till en sida.
Footer inspiration är från wix hemsidor. Det finns en Explore coloumn med alla sidor som finns, en Contact coloumn med fejk mejl och telefon nummer. Connect med fejk knappar till andra sociala medier och tillslut copyright texten. Ville bara ha 3 columner och fylla dom med något så detta blev vad det blev.

About jaguar page har en table med jaguar info som jag tog ifrån denna sidan: https://earth.org/?endangered-species=the-tiger-endangered-species-spotlight 
Ville sedan leka runt med att ha bilder på motsat sida och att texten skulle krama sidorna. En av bilderna testade jag figcaption med liten border.
På botten finns det bild knappar som jag fick inpirationen från botten av sidan här: https://tigers.panda.org/ . Dessa knappar leder till report delen av sidan take action och press release på delen av sidan i support us.

På conservation tog jag mycket inspiration främst från  https://tigers.panda.org/ och https://www.worldwildlife.org/species/tiger . Panda sidan har jag tagit discover knapparna vilket mina knappar leder hellre till Olika delar av conservation sidan. Här började också min färg glada palett för sidorna. Samt pandas vita text över bilden tog jag där ifrån. WWF sidans aside tag och carousel gallery ville jag immitera men jag hittade ingen kod som gjorde det utan javascript så jag fick nöja mig med denna koden: https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_overflow/CSS_carousels 

I take action sidan tog jag hela introt med hero bilde, låg opacity box med vit text över bild och kartan med sid texten från här: https://tigers.panda.org/our_work/where_we_work/ . Jag ville göra knapparna den sidan hade också men det är tydligen javascript. 
Report delen av min sida tog jag inspå från här: https://tigers.panda.org/reports/ . Efter det har jag en merch del med fejk plushies som säljes, det är bara en vanlig flex låda med bild och knapp under. Jag hade sett en sida som hade också hade 4 föremål och en visa mer knapp på någon tiger sida men jag hittade aldrig den igen så jag lekte runt lite med dennas färger och utseende.
I följande adopt del kopierade jag utseendet från denna sidan:  https://www.internationaltigerproject.org/adopt/ . Från toppen till ul tag boxen, sist tog jag contact us delen på slutet av den sidan vilket leer till min andra support us sida. Lagde in en FAQ för ett slut av min sida med inspo igen från: https://www.wwf.se/om-oss/fragor-och-svar/

Support us har en blog av https://www.w3schools.com/howto/howto_css_blog_layout.asp sedan en subscribe input tag. Jag har en press release del vilket är samma kod som min report del, bara byt positionen av bilden. På slutet av sidan har jag en contact us form vilket jag tog utseendet från webben men behövde hjälp att sätta upp koden så lådorna positionerades rätt. 

Som sagt behöll jag färgerna från discover knapparna i conservation till alla design element. Sedan valde jag en specifik guld färg för med viktiga knappar, som i min inner-nav, plushie knapparna och svarta knapparnas hover färg. Kanterna är alltid 8px för modern känsla. Mycket andra design val kom från sagda sidor som WWF.Typografi är arial/Helvetica och titlar brukar vara i bold.
Jag fokuserade främst på desktop vyns utseende men konstant kollade tillbaka i mobil/ipad vy för att se om något blev dåligt och redigerade enligt det samt iaktog hur andra sidor hanterade mobil vy.
Använde mycket flex lådor, coloumns, cards, samma knapp kod repeterades. aside lådor och hero bilder med text över dom.
CSS-monster för interaktivitet: hover, hamburger meny (endast i mobil), scroll snap karusell galleri, detail/summary tag FAQ, responsive bilder med object-fit och aspect-ratio, text clamping för titlar. skip link för tangent avändare, Olika formular med required text fält. 

Kända begränsningar + förbättrningsideer:
Det största problemet jag har är med videon på conservations hero bild. För när den är på ipad eller mobil vy så flyger den åt siden tills man inte kan se den. Som jag förstår nu är de ända lösningar om jag skulle gilla innebär att man behöver javascript. För då kan man ha den flyttande och användaren kan dra runt videon om man vill flytta den själv. Just nu har jag gömt den på bade ipads och mobil så att det inte ser konstigt ut. Alla andra lösningar med att försöka ge videon rum att existera såg dåligt ut för mig. På samma ställe med texten över hero bilden hade jag problem att positionera bilden bra och få texten att få plats. Vita texten var också svårt att läsa så jag försökte ge den text-shadow men av någon anledning så ville den inte ge mig det så jag gav den svarta lådan.
Ett annat stort problem tror jag innebär hur jag satte upp min white-card och inner-nav koden. För jag har viljat ge mina sections gråa eller svarta lådor som WWF sidorna men dom har alltid blockerats och har som en margin som håller fast den att inte gå över 1rem. När jag har lyckats putta ut en grå låda utanför white-card så syns det bara på högra sidan. Men då marker jag problem som med mitt karusell galleri att började existera och följa med gråa lådan utanför vita kortet och då flyttades min titel med den också och align:center blev inte där white-card är utan där gråa lådan följdes ut. Så jag skrottade hela ideen med section lådor. Speciellt eftersom det var så svårt att få inner-nav att klippas ihop med white-card som jag ville att den skulle.
Jag gillar också att använda pinnar mellan coloumns i footern. Vilket jag inte gillar hur de åker till sidan på mobil/ipad vy. Jag ville att de skulle vara horisontellt och i mitten av dom men det var för mycket att lösa. Jag tänkte ha liknane pinnar mellan inner-nav texterna men av någon anledning så var hade dom inte jämna mellanrum mellan orden så jag släppte ideen igen.
Det finns manga load more, read more eller view all osv där jag har lämnat dom ofunktionella. Jag slulle ha velat att dom faktiskt leder någonstans eller utvecklar sig.
Min blogg section tycker jag var väldigt jobbigt att lämna den som den är. Jag vet bara inte hur jag ska fejka en realistik blogg. Då jag skulle behöva mycket mer text, inlägg, sidor och funktioner än vad jag kan. 
På about jaguar sidan är min table lite konstigt på sidan i mobil vy, vet inte hur jag kan fixa det, inget funkar.
Skulle vilja ha bättre palett färger.
Min merch plushies section blev antingen för enkel/tråkig eller för mycket design element och de design element var svår att hålla t.ex. allt grön var för tjock eller tun på vissa delar. Gillar inte slut designen på den. 
Av någon anledning är mina adopt lådor aligned lite till hover i mobil vy också, det förstår jag inte.
Bilder är inte optimerade. Troligen är min text storlek för liten och färg kontraster inte helt bra för alla användare. Clip path kan vara mer precis.
