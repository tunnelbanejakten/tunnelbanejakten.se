# tunnelbanejakten.se – statisk kopia

Det här är en statisk [Astro](https://astro.build)-sajt som är en kopia av den publika innehållet från den tidigare WordPress-sajten [tunnelbanejakten.se](https://tunnelbanejakten.se).

Alla sidor som är synliga för icke-inloggade besökare finns med. Inloggningsskyddade sidor, formulär och pluginfunktionalitet (t.ex. anmälningsformuläret) är inte inkluderade.

## Komma igång

**Krav:** Node.js 18 eller senare.

```bash
# Installera beroenden
npm install

# Starta utvecklingsserver (http://localhost:4321)
npm run dev

# Bygg sajten till statiska filer i dist/
npm run build

# Förhandsgranska den byggda sajten lokalt
npm run preview

# Formatera koden med Prettier
npm run format
```

## Projektstruktur

```
src/
  layouts/
    Layout.astro        # Delad layout med header, nav och footer
  pages/
    index.astro         # Startsidan
    anmal.astro         # Anmälan
    kontakt.astro       # Kontakt
    distans-klassen.astro
    webappen.astro
    overnattning.astro
    om-tsl/             # Info-sektionen
    dagen/              # Under dagen-sektionen
    resultat*.astro     # Resultat 2013–2023
```

## Teknik

- **Ramverk:** [Astro](https://astro.build) v4
- **Output:** Helt statisk (ingen server krävs)
- **Formatering:** [Prettier](https://prettier.io) med `prettier-plugin-astro`
