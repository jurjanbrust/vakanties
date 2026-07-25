# Instructies voor het onderhouden van programma.md

Deze regels gelden voor alle toekomstige aanpassingen aan `programma.md` (en vergelijkbare reisprogramma's in deze map).

## 1. Sfeerfoto's
* Download foto's lokaal naar de map `fotos/` (rechtenvrije bronnen, bijv. Wikimedia Commons).
* Gebruik één foto per belangrijke bezienswaardigheid/locatie (niet per dag, niet alleen bovenaan).
* Embed met `<img src="fotos/bestand.jpg" width="300" alt="...">` zodat de layout compact blijft; meerdere foto's naast elkaar mag.

## 2. Routes tussen locaties
* Bepaal per segment (van stop A naar stop B) de **afstand** en **reistijd**, en kies de vervoerswijze:
  * 🚶 **Wandelen** als de afstand ≤ ~2,2 km is (of iets langer als de wandeling zelf een sfeervol onderdeel van het programma is, bijv. langs de Theems of door een park).
  * 🚇 **Metro/tube** als lopen > ~30-40 minuten zou kosten, of als er tijdsdruk is (bijv. bagage, aansluiting op trein).
  * 🚌 **Bus** als alternatief noemen waar relevant (bijv. korte stukken zonder metrostation dichtbij).
* Vermeld bij elk segment: icoon, van → naar, afstand (km), tijd (min), en een klikbare Google Maps-link.
* Gebruik voor de Maps-link altijd het officiële formaat met expliciete `travelmode`, zodat de link ook echt in de juiste modus opent:
  `https://www.google.com/maps/dir/?api=1&origin=<van>&destination=<naar>&travelmode=walking` (of `transit`, `driving`, `bicycling`).
  Gebruik geen losse multi-stop `/maps/dir/A/B/C/` links — die openen standaard als auto-route.
* Zet de segmenten per dag in een compacte tabel (icoon | van → naar | afstand | tijd | link), niet als lopende tekst, om het overzichtelijk te houden.
* Voeg bovenaan het bestand een kleine legenda toe (🚶 wandelen · 🚇 metro · 🚌 bus).
* Waar een lange loop-route ook een leuk alternatief vervoer heeft (bijv. bus), noem dat kort als "alt." in een cursieve toelichting binnen de tabelrij — niet als aparte rij, om de tabel kort te houden.

## 3. Data/dagen controleren
* Controleer bij elke wijziging of de weekdag bij een datum klopt (bereken dit, ga niet uit van eerdere aannames in het document).

## 4. Algemeen
* Houd het overzicht kort: geen overbodige uitleg, geen dubbele info tussen tabel en lopende tekst.
* Wijzig alleen wat nodig is; laat bestaande, correcte content staan.

## 5. Regenalternatief & reserveringen
* Voeg per dag een korte "☔ Bij regen"-suggestie toe (overdekt alternatief uit het bestaande programma van die dag, geen nieuwe locaties verzinnen tenzij nodig).
* Voeg bij het avondeten een "📅 Reserveren"-regel toe met een link naar de officiële restaurantwebsite (geen OpenTable-gok-links) en een korte tip (wel/niet reserveerbaar, hoe druk).
* Vermeld transportkosten (OV-dagcap) in de kostentabel wanneer een dag metro/bus gebruikt.

## 6. Openingstijden
* Voeg per dag een "🕒 Openingstijden"-regel toe voor musea/attracties met vast tijdslot (Tower of London, British Museum, London Eye, Tate Modern, Wallace Collection, markten).
* Verifieer tijden bij de officiële website; als een tijd niet live te bevestigen is, voeg "(check voor vertrek)" toe in plaats van te gokken.

## 7. Vaste aankomst-/vertrektijden
* Als een trein/vlucht-tijd bekend is (aankomst of vertrek), reken het dagprogramma daar expliciet op terug/vooruit met concrete kloktijden per stap (niet alleen dagdelen als "ochtend/middag").
* Bouw een buffer in vóór vertrek (Eurostar: ~90 min voor check-in/paspoortcontrole) en vermeld dit in een opvallende regel bovenaan de dag.

## 8. Ontbijt, lunch & fooien
* Voeg per dag een "🍳 Ontbijt"-suggestie toe op loopafstand van het startpunt van die dag (meestal het hotel), met korte omschrijving en indicatieprijs p.p.
* Voeg bij het middaggedeelte een "🍽️ Lunch"-suggestie toe (kan een bestaande markt/foodhall uit het programma zijn), met indicatieprijs p.p.
* Varieer de ontbijt-/lunchplekken per dag, gebruik alleen bekende/bestaande zaken.
* Neem een fooien-paragraaf op in de Extra Tips-sectie (UK-conventie: service charge vaak al inbegrepen).

## 9. Weer & kleding
* Haal een actuele weersverwachting op (bijv. via Open-Meteo) voor de reisdagen en zet een compacte tabel (temperatuur, neerslagkans) bovenaan het bestand.
* Geef kort kledingadvies gebaseerd op de verwachting; vermeld expliciet dat een verwachting >6 dagen vooruit indicatief is en dichter bij vertrek herzien moet worden.

## 10. Wijzigingen in reistijden (vertraging/vervroeging)
* Als een aankomst-/vertrektijd wijzigt (bijv. vertraging), werk de betreffende dag(en) bij met de nieuwe kloktijd en vermeld kort de oorspronkelijke tijd erbij (bijv. "was 14:17"), zodat de wijziging traceerbaar blijft.
* Controleer of aansluitende tijdsblokken (check-in, buffers) nog kloppen na de aanpassing.

## 11. Alternatieven per dag
* Voeg onderaan het bestand een tabel toe met per dag één of meerdere alternatieven voor onderdelen die kunnen tegenvallen (druk, gesloten, uitverkocht), bij voorkeur in dezelfde buurt zodat er geen extra reistijd nodig is.

## 12. Losse wandelroutes (Komoot)
* Voeg onderaan het bestand een tabel toe met Komoot-zoeklinks (`https://www.komoot.com/discover?query=<zoekterm>`) per dag/gebied, verdeeld in kort (~2-3 km), middel (~5-6 km) en lang (~8-10 km), als optionele extra wandeling naast het hoofdprogramma.

