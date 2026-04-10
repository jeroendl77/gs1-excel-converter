# GS1 Import Converter

Teamtool voor het omzetten van klantenbestanden naar het GS1 Datasource importformat.

## Gebruik

1. Open de applicatie via de Vercel-link
2. Log in met het teamwachtwoord: `gs1team2024`
3. Upload een Excel-bestand van een klant
4. Klik op "AI-detectie starten"
5. Controleer en pas de veldkoppelingen aan waar nodig
6. Detecteer hiërarchieën en download het GS1-importbestand

## API Key instellen

De AI-detectie heeft een Anthropic API key nodig. Voeg deze toe in Vercel:

1. Ga naar je project op vercel.com
2. Klik op "Settings" → "Environment Variables"
3. Voeg toe: naam = `ANTHROPIC_API_KEY`, waarde = jouw API key
4. Klik op "Save" en herdeplooy

Of voeg tijdelijk toe aan index.html (niet aanbevolen voor productie):
```js
window.ANTHROPIC_API_KEY = 'jouw-api-key-hier';
```

## Wachtwoord wijzigen

Zoek in index.html naar:
```js
const PASS = 'gs1team2024';
```
Vervang door een eigen wachtwoord.

## Verbeteringen doorvoeren

1. Vraag een nieuwe versie van index.html op
2. Upload het bestand naar GitHub (vervang het bestaande)
3. Vercel herdeployt automatisch binnen 30 seconden
