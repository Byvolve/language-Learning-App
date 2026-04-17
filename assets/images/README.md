# Afbeeldingen — naamconventie

Sla afbeeldingen op in de map van het bijbehorende thema.

## Structuur

```
assets/images/
  supermarket/
    boodschappen.jpg
    kassa.jpg
    korting.jpg
    tas.jpg
    wachten.jpg
  family/
    picknick.jpg
    kleedje.jpg
    boterhammen.jpg
    verstoppertje.jpg
  daily-life/
    buurt.jpg
    bak.jpg
    riem.jpg
    snurkt.jpg
```

## Naamconventie

- Gebruik de **NL naam van het woord** als bestandsnaam (lowercase)
- Spaties → koppelstreepjes (bijv. `hide-and-seek.jpg`)
- Formaat: JPG of WebP
- Formaat: bij voorkeur **vierkant**, minimaal **400 × 400 px**

## Koppelen aan een woord

Open `index.html` en zoek het keyword-object dat je wilt bijwerken.  
Verander `image: null` naar het pad:

```js
// Oud:
{ word: "boodschappen", emoji: "🛒", audio: null, image: null, ... }

// Nieuw:
{ word: "boodschappen", emoji: "🛒", audio: null, image: "assets/images/supermarket/boodschappen.jpg", ... }
```

Doe hetzelfde voor de `flashcardSets` array (ook in `index.html`).  
Zodra `image` is ingevuld, toont de app de foto in plaats van de emoji.
