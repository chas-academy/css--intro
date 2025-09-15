# Bootcamp FMW2025 - 🎨 Grundläggande CSS

Denna vecka ska vi fokusera på CSS, webbens stylingspråk. Det används till allt från att ändra typsnittstorlekar och bakgrundsfärg till att positionera och animera HTML-element. Utan styling hade webben sett ut som 90-talets uppsatser och textdokument som HTML ursprungligen skapades för.

## 🧱 Tips: Kopiera README

Skriv över readme:n i repon som ni jobbar i med denna för att ha den aktuella informationen lättare tillgänglig.

## 🕵️‍♂️ Analysera designen

Gå tillbaka till designen ni valde förra veckan och analysera dess styling. Går det att se en klar visuell hierarki? Ta hjälp av webbläsarens dev tools.

- Vad har rubrikerna och textstyckena för fontstorlek?
- Har de olika font weight (Tjocklek) och färg?
- Jobbar man med skuggor eller olika färgnyanser för att få designen att se mindre "platt" ut?
- Hur har man använt white space (Mellanrum) som exempelvis padding och margin?
- Hur är de olika parent-elementen och deras children positionerade? Är vissa saker centrerade och andra vänsterställda?

### Alternativ för var stylingen göras

1. Skapa taggarna `<style></style>` direkt i HTML-filen. Lägg taggarna som sibling till `<body></body>`

```html
</head>
  <style>
    .container {
      ...
    }
</style>
<body>
```

2. Skapa ett separat stylesheet - exempelvis `index.css` och `form.css`. Länka till dem i `<head></head>` i vardera HTML-fil.

```html
<head>
  <link rel="stylesheet" href="index.css" />
</head>
```

### Bestäm också om ni ska gå efter "content model" eller "box model"

### Det är givetvis fritt fram att ändra, lägga till och ta bort HTML-element vid behov

Behövs det läggas till klasser på vissa element? Har du bara en av ett visst element? Har du fler av ett element men med olika parent-element?

- Klasser
- Element
- Specificitet
  - Parent
    - Siblings: Child, child

## 🎁 Bonusuppgifter

### Styla klickbara element med psuedo selectors

- `:hover`, `:active` eller `:focused` state
- Implementera transitions

### Skapa en enkel animation med `@keyframes`

Exempelvis på rubriken eller en ikon

## Gör sidan responsiv för tablets

- Kolla upp typiska skärmstorlekar (i pixlar) och hitta en bra utgångspunkt för `@media` queries
