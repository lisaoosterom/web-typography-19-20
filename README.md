# Responsive Typography, 2019/2020

Als je doof bent, of als je om een andere reden geen geluid kunt horen, dan mis je veel informatie als je een film kijkt. Knisperende voetstappen, langzaam aanzwellende muziek, nerveus getik op een deur, je hoort het natuurlijk allemaal niet. Nu bestaat er zoiets als *closed caption*, wat een type ondertiteling is waarbij ook dingen als omgevingsgeluiden en de muziek beschreven worden. Hierdoor krijgt een kijker die informatie wel binnen.

Alleen wordt die auditieve informatie nogal neutraal beschreven. Het geluid van huilend persoon zou bijvoorbeeld beschreven kunnen worden als *snikgeluid op de achtergrond*. En iemand die lacht zou geschreven kunnen worden als *iemand lacht.* Heel neutraal, bijna zakelijk, en bovendien allebei in precies hetzelfde neutrale lettertype. Terwijl het toch echt over twee heel verschillende emoties gaat. 

Dat kan visueel sterker. 

En dat gaan jullie doen.

## Leerdoelen

- Je kan de kennis over vormgeving die je hebt opgedaan tijdens de minor technisch toepassen met behulp van CSS
- Je kan verborgen nuance uit een audiotrack overtuigend vertalen naar visuele (typografische) beelden
- Je kan je typografische keuzes onderbouwen.
- Je hebt de exclusive design principles gebruikt.

## Oplevering




### Font keuze

Voor mijn flosed captions ben ik gegaan voor het systeem font. Ik als ontwerper voel mij altijd prettiger met beperkingen, omdat css nou niet helemaal mijn straatje was, leek het mij wel een goed idee om voor het systeemfont te gaan ipv de brenner. Ook voelde ik niet zo veel bij het brenner font, ik was zelf gegaan voor een soort digital font zoals je ze ziet op je wekker. Bij dit fragemnt heb ik dus gewerkt met normal, cursif en bold. 

De scene bestaat vooral uit twee stemmen de stem van constant K en die van de computer. Die twee stemmen heb ik apart gestyled. De computer stem heb ik met een blauwe glow gestyled, de glow zodat het die digitale sfeer heeft. De stem van constant K heb ik wit gestyled, zonder gekke poespas. Dit omdat ik goed het onderscheid tussen de twee stemmen wilde laten zien, omdat het niet altijd even duidelijk is wie er spreekt. 

Op een gegeven moment herhaalt constant K de computer met 'cells' en 'interlinked', die onderdelen heb ik een class 'repeat' meegegeven en groter weergeven. Dit omdat die herhalingen best bij mij binnen komen, zonder geluid lijkt me dit een best droge scene omdat je de dialoog niet helemaal meekrijgt. Door het vergroten van die herhalingen van constant K denk ik dat die op een zelfde manier binnen komen en blijven hangen als dat ik het ervaar.


### Testen met Marie

Bij de eerste onmoeting met Marie wist ik zelf niet zo goed wat ik precies kon vragen omdat ik nog totaal geen idee had waar dit project naar heen ging. Er zijn me wel een aantal dingen opgevallen uit de eerste ontmoeting.
 * Ze houd van lezen en leest ook wel snel
 * Leest zowel engels als nederlands
 * Scarcasme is moeilijk te begrijpen vanuit de closed captions
 * Als ze bij een concert zou zijn zou ze wel viberatie ervaren die uit de bass komt, dus wel een soort tempo ervaren.
 * Als de gene die spreekt in de film in beeld is is het duidelijk wie er spreekt, als dit niet zo is word het lastiger.
 * Maakt in het dagelijks leven niet zo veel gebruik van emojis.
 * Sfeer meekrijgen van een film met veel geluid is lastig
 
 Met deze informatie ben ik aan de slag gegaan en vooral gaan expierimenteren voor test 1, omdat ik geen flauw benul had waar Marie precies behoefde aan had.

## Expierimenteren.

Voor de eerste test met Marie had ik veel geexpirimenteerd in het eerste deel van het fragment. Dit heb ik vooral gedaan door rondom het video frame dingen te laten gebeuren. Zo had ik bijvoorbeeld een laser effect over de video heen laten gaan, op het moment dat er een laser geluid voorbij kwam. En had ik de video laten 'skewen'. 
### Tijdens het afspelen

Tijdens het afspeelen wordt er een class `on` op de caption gezet als hij moet verschijnen, en een class `off` als hij klaar is. *Zowel class `on` als class `off` blijft op de caption staan!*

De timimg van de captions kan je aanpassen in [closed-captions/captions.js](closed-captions/captions.js).

Er verschijnen ook classes op de body op momenten dat er geluiden worden afgespeeld, zoals `sound1` en `sound2`. Je kan geluiden toevoegen in [closed-captions/sounds.js](closed-captions/sounds.js).

*let op,* de geluiden zijn niet compleet, dit zal je zelf moeten aanvullen.

## Een eigen fragment (afgeraden, uitgebreide onderbouwing is nodig)

Je kan er ook voor kiezen om een eigen, *beter* fragment te gebruiken. Dit wordt afgeraden. De tijd die je besteedt aan het zoeken naar dat fragment kan je beter besteden aan het werken aan de opdracht. Bovendien blijkt dat er vaak fragmenten worden gekozen die niet goed voldoen aan de opdracht. Als je een ander fragment kiest dan *moet* je dit goed onderbouwd voorleggen aan je docent. De deadline hiervoor is vrijdagochtend in de eerste week.

### Waar moet je op letten bij het kiezen van een eigen fragment.
Lees de opdracht nog eens goed door. Waar gaat het ook al weer precies om? 

Voor een goede onderbouwing van je keuze voor een ander fragment moet je deze vragen in elk geval beantwoorden:

- Welke informatie zit er in de audio die echt niet zichtbaar is?
- Welke rol speelt de audio in het fragment?
- Werkt de scene nog zonder geluid?
- Waarom is dit fragment beter dan het aangeboden fragment?

Je kan dan de nodige HTML en JavaScript genereren door gebruik te maken van [caption generator](https://cmda-minor-vid.github.io/web-typography-18-19/generator/) (in Google Chrome). 

Als je de closed captions wil bewerken dan kan je een tool zoals [Amber Script](https://www.amberscript.com/en) gebruiken. Daar kan je exporteren als `.srt`, en die kan je weer door de generator halen.
