# 📋 Herbruikbare prompt: reisprogramma bouwen met Copilot CLI

Dit document beschrijft de aanpak die is gebruikt om `London-2026/README.md` te bouwen. Gebruik dit als startprompt/instructie om Copilot CLI hetzelfde te laten doen voor een **nieuwe** vakantie.

## Startprompt (kopieer en pas aan)

> Bekijk mijn ruwe programma voor [BESTEMMING, DATUMS, AANTAL PERSONEN] en help mij dit te verbeteren tot een overzichtelijk, mobielvriendelijk markdown-bestand. Voeg sfeerfoto's toe per bezienswaardigheid, voeg routes toe tussen de stops (wandel/OV, met tijd, afstand en een werkende Google Maps-link per vervoerswijze), corrigeer de weekdagen bij de datums, en stel mij onderweg vragen over voorkeuren. Maak een submap `[Bestemming]-[Jaar]/` met een `README.md`, `fotos/` map en volg de regels in `PROMPT.md`.

## Werkwijze / regels

### 1. Sfeerfoto's
* Download foto's lokaal naar `fotos/` binnen de vakantie-submap (rechtenvrije bronnen, bijv. Wikimedia Commons via de Commons Search API — geraden thumbnail-URL's 404'en vaak).
* Eén foto per belangrijke bezienswaardigheid/locatie (niet alleen per dag).
* Embed met `<img src="fotos/bestand.jpg" width="300" alt="...">`; meerdere foto's naast elkaar mag. GitHub schaalt dit automatisch naar 100% breedte op mobiel.

### 2. Routes tussen locaties
* Bepaal per segment (A → B) **afstand** en **reistijd**, en kies de vervoerswijze:
  * 🚶 **Wandelen** tot ~2,2 km (of iets meer als de wandeling zelf sfeervol is, bijv. langs water of door een park).
  * 🚇 **Metro/tram** als lopen >30-40 min zou kosten, of bij tijdsdruk (bagage, aansluiting).
  * 🚌 **Bus** als alternatief noemen waar relevant.
* Vermeld per segment: icoon, van → naar, afstand (km), tijd (min), klikbare Maps-link.
* **Gebruik altijd dit Maps-linkformaat** zodat de juiste modus opent (multi-stop `/maps/dir/A/B/C/`-links openen standaard als auto-route en werken dus niet):
  `https://www.google.com/maps/dir/?api=1&origin=<van>&destination=<naar>&travelmode=walking` (of `transit`/`driving`/`bicycling`).
* Zet segmenten per dag in een compacte tabel (icoon | van → naar | afstand | tijd | link), niet als lopende tekst.
* Voeg bovenaan het bestand een legenda toe (🚶 wandelen · 🚇 metro · 🚌 bus).

### 3. Data/dagen controleren
* Reken bij elke datum de weekdag zelf uit — ga niet uit van aannames.

### 4. Algemeen
* Houd het kort: geen overbodige uitleg, geen dubbele info tussen tabel en tekst.
* Wijzig alleen wat nodig is; laat bestaande, correcte content staan.

### 5. Regenalternatief & reserveringen
* Per dag een korte "☔ Bij regen"-suggestie (overdekt alternatief, liefst uit hetzelfde dagprogramma).
* Bij avondeten een "📅 Reserveren"-regel met link naar de officiële restaurantwebsite + korte tip.
* Vermeld OV-dagcap/transportkosten in de kostentabel wanneer een dag OV gebruikt.

### 6. Openingstijden
* Per dag een "🕒 Openingstijden"-regel voor musea/attracties met vast tijdslot.
* Verifieer bij de officiële website; kan een tijd niet live bevestigd worden, voeg dan "(check voor vertrek)" toe in plaats van te gokken.

### 7. Vaste aankomst-/vertrektijden
* Als een trein/vlucht-tijd bekend is, reken het dagprogramma daar expliciet op terug/vooruit met concrete kloktijden (niet alleen "ochtend/middag").
* Bouw een buffer in vóór vertrek (bijv. Eurostar: ~90 min) en vermeld dit opvallend bovenaan die dag.

### 8. Ontbijt, lunch & fooien
* Per dag een "🍳 Ontbijt"-suggestie op loopafstand van het startpunt, met indicatieprijs p.p.
* Per dag een "🍽️ Lunch"-suggestie (mag een bestaande markt/foodhall zijn), met indicatieprijs p.p.
* Varieer de plekken, gebruik alleen bekende/bestaande zaken.
* Neem een fooien-paragraaf op (lokale conventie, bijv. UK: service charge vaak al inbegrepen).

### 9. Weer & kleding
* Haal een actuele verwachting op (bijv. Open-Meteo — `wttr.in` geeft te weinig dagen vooruit) en zet een compacte tabel bovenaan (temperatuur, neerslagkans).
* Geef kort kledingadvies; vermeld dat een verwachting >6 dagen vooruit indicatief is.

### 10. Achtergrondinfo per locatie
* Voeg per bezienswaardigheid een inklapbaar blok toe: `<details><summary>ℹ️ Achtergrond & tips: X</summary>` met 🔗 bron-link (bijv. Wikipedia), 🏛️ historie, ✅ leuk om te doen, ⚠️ te vermijden.
* Houd dit inklapbaar zodat de pagina op mobiel overzichtelijk blijft.

### 11. Mobielvriendelijkheid
* Voeg bovenaan een `<a id="top"></a>` en een korte inhoudsopgave toe die naar `<a id="dagN"></a>`-ankers per dag springt (betrouwbaarder dan gokken naar GitHub's auto-gegenereerde heading-slugs).
* Voeg na elke dag een `[⬆️ Terug naar boven](#top)`-link toe.
* Gebruik `<details>` voor lange achtergrondinfo zodat de hoofdpagina kort blijft.
* Breed tabellen (routes) mogen op mobiel horizontaal scrollen — dat is acceptabel GitHub-gedrag.

### 12. Repostructuur
* Eén submap per vakantie: `[Bestemming]-[Jaar]/` met daarin `README.md` (het programma, zodat GitHub het automatisch toont bij het openen van de map), `fotos/`, en evt. een lokale `instructies-programma.md` als er bestemming-specifieke afspraken zijn.
* Werk aanpassingen die voor **alle** toekomstige vakanties gelden bij in dit `PROMPT.md` op repo-niveau.
