# Vinyl Vault 2.0

Mobile-first HTML/CSS/JavaScript. Geen buildstap.

## Starten
- Lokaal: `python -m http.server 8000` in deze map, open http://localhost:8000.
- Telefoon: publiceer alle bestanden via HTTPS (bijvoorbeeld GitHub Pages). Open de URL in Chrome en kies Installeren / Toevoegen aan startscherm.
- Discogs: maak een persoonlijk token op https://www.discogs.com/settings/developers en vul dit in bij Instellingen. Zoek op titel, artiest, catalogusnummer of barcode. Controleer de geïmporteerde gegevens voor opslaan.
- Scanner: gebruikt de browser-eigen BarcodeDetector en camera. HTTPS of localhost en toestemming vereist. Niet elke browser ondersteunt dit; handmatige invoer is altijd mogelijk.
- Offline: na een succesvolle eerste online installatie werkt de lokale bibliotheek offline. Discogs en externe covers vereisen internet.
- Dezelfde localStorage-sleutel als v1. Bij dezelfde origin blijft de collectie beschikbaar; bij andere origin eerst JSON exporteren en importeren. Token wordt niet geëxporteerd. Geen synchronisatie.
- Token wordt lokaal onversleuteld opgeslagen en rechtstreeks aan Discogs verzonden. Gebruik alleen een vertrouwde privé-installatie; geen gedeeld token in broncode. Browser-CORS of API-wijzigingen kunnen een serverproxy noodzakelijk maken.
- Discogs-gegevens en afbeeldingen vallen onder de voorwaarden van Discogs; controleer die voor publieke distributie. Geen marktwaardebepaling.

## Controle
JavaScript syntax gecontroleerd; live API, camera en installatie niet op een echt toestel getest.
