---
hide:
  - navigation
---  
# Lage instruksjonsvideoer

Denne siden forklarer steg for steg hvordan du lager en instruksjonsvideo, populært kalt "tutorial video". Stegene beskrevet nedenfor er en måte å tilnærme seg en slik oppgave, du kan selv velge om du ønsker å gjøre det annerledes.

!!! warning Informasjon om denne ressursen

    Denne siden er laget i forbindelse med `LTEK10222-1 24V Profesjonsfaglig digital kompetanse` som et eksempel på en digital ressurs. 

## Oversikt

Å lage en instruksjonsvideo kan føles som en stor og litt skremmende oppgave, men hvis du bryter den ned i mindre steg så blir den mye mer overkommelig. På denne siden viser jeg prosessen med å lage en kort video hvor vi lager et python program. 

*Kort oppsummert er prosessen:*

1. Vit hva du skal lage
2. Lag en kjøreplan for videoen din
3. Ha kontroll på det tekniske
4. Spill inn videoen
5. Rediger videoen din
6. Eksporter videoen og gjør den tilgjengelig

## Vit hva du skal lage

Når du skal lære bort noe er det viktig at du kan det godt. Derfor er første steg alltid å sjekke at du vet hvordan du gjør det. Her er det enkelt å tenke *"Ja dette kan jeg"* for så å hoppe rett til innspilling og oppdage at det var noen hull i det du kan.

!!! tips Tips når du tester at du kan det

    Mens du tester ut at du kan det er det ofte lurt å notere stegene på et papir, mens du tester. Gjør du det så har du allerede et utkast til en kjøreplan når du kommer til neste punkt.

### Python video

Før jeg skulle lage python videoen testet jeg ut at jeg husket hvordan jeg skulle skrive koden og sjekket at det virket som det skal på datamaskinen jeg gjør opptak på.

Når jeg gjorde det innså jeg at det er lurt å ha noe tekst i `input()` funksjonen, for å gjøre programmet mitt mer brukervennlig. 

#### Koden
Etter at jeg hadde testet det ut hadde jeg allerede notert stegene på et papir og jeg hadde koden min, dette er den jeg senere brukte i starten av videoen for å demonstrere hva vi skal lage.

**Koden ser slik ut:**

```python linenums="1"
navn = input("Skriv navnet ditt: ")
print("Hei " + navn)
```

Når jeg nå har testet at jeg vet hvordan jeg gjør det jeg skal lage video om er jeg klar til å lage kjøreplanen min. 

## Lag en kjøreplan for videoen din

Kort fortalt er en kjøreplan bare en steg-for-steg plan over hva du skal gjøre i videoen. Målet er at den skal være en liten guide som hjelper deg å unngå at du glemmer noen viktige steg når du spiller inn videoen.

Du kan lage kjøreplanen din i et hvilket som helst format, men det er en fordel å få den ut på papir, da kan du ha en penn og krysse av mens du spiller inn videoen.

### Eksempel

I boksen nedenfor ser du kjøreplanen jeg brukte til videoen min.

!!! abstract "Eksempel på kjøreplan"

    Åpne terminal (PowerShell)
    Lag ny mappe til prosjektet
    Lag ny fil og åpne den i VS Code : code navn.py
    Skriv koden

    ```
    navn = input()
    print("Hello " + navn)
    ```

    Kjør koden for å vise at den virker
    Forklar hva koden gjør

        - navn : lager en variabel hvor vi kan lagre navnet til brukeren
        - = : lagrer det som er på høyre side i variabelen på venstre side
        - input() : En funksjon som ber brukeren skrive inn noe, det som står i parentes vises til brukeren
        - "Skriv navnet ditt: " Teksten som vises til brukeren når vi ber dem skrive inn noe

        - print() : Dette er en funksjon som skriver ut det som er i parentes til terminalen
        - "Hello" : Når det står i hermetegn betyr det at det er en tekst
        - + : betyr at vi skal koble sammen flere ting og som skrives til terminalen
        - navn : er variablen hvor navnet til brukeren er skrevet


    Lukk VS Code
    Kjør koden i terminalen : python navn.py

## Ha kontroll på det tekniske

Det er mange måter å spille inn en video på datamaskinen din, felles for dem alle er at du må være sikker på at alt virker, før du gjør selve innspillingen, ellers vil du bruke svært mye tid på feilsøking.

Det tekniske du må ha kontroll på er:

- Hvordan skal du gjøre opptaket?
- Er lyden god

### Innspilling

Det finnes mange programmer for innspilling av skjermvideo, jeg brukte MS Stream, som er tilgjengelig via Office pakken, men du står fritt til å velge et annet verktøy.

#### MS Stream

I videoen nedenfor viser Mike Tholfsen fra Microsoft kort hvordan du kan spille inn video i Stream

<iframe width="560" height="315" src="https://www.youtube.com/embed/RYEDqBzwNFY?si=EESBU1vXWU4qzNPH&amp;start=112" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

Hvis du foretrekker en skriftlig forklaring kan du lese en [Steg for steg forklaring hos Microsoft](https://support.microsoft.com/en-gb/office/microsoft-stream-screen-recorder-e98d8791-2b82-4dc7-889a-959724e3cbad)

MS Stream er en del av office pakken og du trenger ikke installere noe for å bruke det, [klikk på linken for å åpne stream](https://www.microsoft365.com/launch/stream)

??? info "Konvertering av video"
    Bruker du MS Stream og vil laste ned og redigere videoen etterpå må du kanskje konvertere den til et annet format for at Premier Pro skal kunne åpne den.

    Dette kan du bruke ffmpeg til, les mer på fireship: [Editing videos with ffmpeg](https://fireship.io/lessons/ffmpeg-useful-techniques/)

#### OBS Studio

Et annet godt alternativ er å bruke OBS Studio. Dette er et program du installerer på datamaskinen din. Her får du mer kontroll over hva som spilles inn og kvaliteten på det, men det er også betydelig mer avansert å bruke. 

Videoen nedefor gir en fin introduksjon til hvordan du kan bruke OBS.

<iframe width="560" height="315" src="https://www.youtube.com/embed/ySENWFIkL7c?si=GcJlGVlNZc7ntErG" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

OBS er gratis, og tilgjengelig både på Windows, Mac og Linx. Du kan laste det ned fra [hjemmesiden til OBS prosjektet](https://obsproject.com/)

### Lyd

Når du lager videoer så er det viktig at lyden er best mulig, dårlig lyd gjør det vanskeligere å følge med på videoen. 

Min anbefaling er at du finner et rolig rom og bruker en ekstern mikrofon når du spiller inn.

!!! tips "Trenger du låne mikrofon?"

    Hvis du ikke har egen mikrofon kan du låne en av skolen. 

### Skriftstørrelse

Husk at ofte skal de som ser videoen bruke en liten skjerm (for eksempel en mobiltelefon). Derfor er det lurt å lage teksten større, slik at det er enklere å se hva som skjer.

Ofte så er den enkleste måten å gjøre dette på å **endre oppløsningen til 1280x720** på skjermen du bruker til opptak.

## Spill inn videoen

Du er nå klar til å spille inn videoen, her kan det være fristende å stoppe opptaket og strte på ny, når du gjør feil. Som oftest skaper det mer jobb enn nødvendig. Det beste er normalt å bare trekke pusten og ta det en gang til, så klipper du bare vekk feilene når du redigerer det.

#### Eksempel

Selv om den endelige videoen min er ca 4 minutter lang så er råfila 12 minutter lang, det er rett og slett enklere og mer effektivt å klippe vekk ekstradelene når jeg redigerer. 

##### Uredigert video (12:08)

Videoen nedenfor er den uredigerte versjonen av videoen min, her har jeg ikke gjort noe med hverken lyd eller klippet noe.

<iframe width="560" height="315" src="https://www.youtube.com/embed/utHTnHq6t5g?si=KTOtDlM67k7mGtXa" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

##### Redigert versjon (4:02)

I denne videoen har jeg fikset litt på lyden og så klippet videoen for å få en bedre flyt i den. Det endelige resultatet er omtrent 1/3 del av den uredigerte. 

<iframe width="560" height="315" src="https://www.youtube.com/embed/wka97BSRnBU?si=5hFjVw3uNMwXU2ut" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

*Hvis jeg skulle stoppet og startet hver gang jeg gjorde feil ville jeg brukt mye mer enn 8 minutter ekstra.*

## Rediger videoen din

Når du nå har spilt inn videoen din er du klar til å redigere, åpne Premier Pro og importer videoen din.

??? tips "Klikk her for å se hvordan du laster ned og konverterer video fra Stream"

    Når videoen min er spilt inn kan jeg laste den ned fra Stream, men må da konvertere den først, før jeg kan bruke den i Permier Pro

    <iframe width="560" height="315" src="https://www.youtube.com/embed/yjYp3RSeRTY?si=CmrnZxzp2wuMeoSj" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

Videoen nedenfor viser hvordan du kommer i gang med videoen din og gir et godt tips til hvordan du kan få lyden bedre.

<iframe width="560" height="315" src="https://www.youtube.com/embed/19atrKDlxiY?si=F3DzWs-YjrG7qsru" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### Introduksjon til Premier Pro

Hvis du trenger en introduksjon til Premier Pro gir denne videoen en grei introduksjon til programmet.

<iframe width="560" height="315" src="https://www.youtube.com/embed/2Gy_WYrlnYc?si=_oucEUXlXpf-IPyF" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Eksporter videoen og gjør den tilgjengelig

Når videoen er redigert må du eksportere den til en video, det er viktig at du leverer videoen og ikke Premier Pro prosjektet. 

Den enkleste måten å eksportere er å ha tidslinjen åpen og klikke på eksporter på toppen av skjermen i Premier Pro.

<iframe width="560" height="315" src="https://www.youtube.com/embed/CU58o_iB6Ls?si=1sKmeUwPXLf0Y0IO" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>