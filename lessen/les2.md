# Les 2

<!--
// TODO: native wind
-->

- [Les 2](#les-2)
  - [React Native](#react-native)
  - [Expo](#expo)
  - [TSX vs JSX](#tsx-vs-jsx)
  - [Opdrachten](#opdrachten)
    - [Opdracht 1 - Hello World](#opdracht-1---hello-world)
    - [Opdracht 2 - Bezoekersteller](#opdracht-2---bezoekersteller)
    - [Opdracht 3 - Wisselende Achtergrondkleur](#opdracht-3---wisselende-achtergrondkleur)
    - [Opdracht 4 - Random Quote Generator](#opdracht-4---random-quote-generator)
    - [Opdracht 5](#opdracht-5)
    - [Opdracht 6](#opdracht-6)

<br><br>

## React Native

React Native is een framework waarmee je mobiele apps kunt bouwen met JavaScript en React.
In plaats van HTML en CSS worden native UI-componenten gebruikt, waardoor de app eruitziet en aanvoelt
als een echte native app.

React Native werkt met een _bridge_, een tussenlaag die zorgt dat JavaScript de native API aan kan spreken.
Hierdoor kan je met JavaScript direct communiceren met de functies van een mobiel besturingssysteem, zoals toegang
tot de camera of GPS.

Doordat er een bridge is voor Android en voor iOS kan je tijdens de ontwikkeling generieke elementen gebruiken.
In react heb je bijvoorbeeld heyt component `<Button>`, dat op Android vertaald wordt naar `android.widget.Button` en
op iOS naar `UIButton`.

<br><br>

## Expo

Expo is een ontwikkelomgeving en toolset die het werken met React Native makkelijker maakt.

De Expo Go-app maakt het mogelijk om een app eenvoudig op de telefoon te bekijken, inclusief _live update_
terwijl `console.log`s op je PC te lezen zijn. Gebruik dit voor debugging.

<br><br>

## TSX vs JSX

De officiële documentatie van Expo gebruikt tegenwoordig TypeScript (`.tsx` bestanden), terwijl wij in deze
cursus met JavaScript (`.jsx` bestanden) werken.

TypeScript lijkt erg op JavaScript, maar voegt daaraan typedeclaraties (en controle) toe.
Als je documentatie tegenkomt met TypeScript-code (Bijv. `:string`), kun je deze meestal eenvoudig omzetten naar
JavaScript door de type-aanduidingen weg te laten.

<br><br>

## Opdrachten

### Opdracht 1 - Hello World

Tijdens deze les zul je meerdere opdrachten uitvoeren. Voor iedere opdracht voer je opnieuw onderstaande installatie
uit,
wat dus betekent dat je voor iedere opdracht een nieuwe app maakt.

Maak je eerste Expo app door de [installatie van les 2](../guides/installatie.md) te volgen.

- Test de app op je telefoon
- Verander de standaard tekst naar 'Hello World', of een eigen creatieve tekst.

<br><br>

### Opdracht 2 - Bezoekersteller

[Installeer](../guides/installatie.md) een nieuwe Expo app.
<br>
Bouw vervolgens een React Native-app waarmee je het aantal mensen kunt bijhouden dat een ruimte in- en uitloopt (bijvoorbeeld omdat er maar
maximaal 200 mensen tegelijk aanwezig mogen zijn van de brandweer).

- De app bevat drie knoppen:
  - **+1** om een persoon toe te voegen.
  - **-1** om een persoon te verwijderen.
  - **Reset** om de teller op 0 te zetten.
- De teller mag nooit kleiner dan **0** worden.
- Als een gebruiker probeert de teller onder **0** te verlagen, toon dan een **alert** met een waarschuwingsbericht.
- Zorg dat de app er **visueel aantrekkelijk** uitziet.

Gebruik `console.log` om de flow van je app te debuggen.

> Klaar? Voeg ook een **progressbar** toe die de capaciteit van 0% tot 100% weergeeft? De progressbar moet dynamisch de huidige waarde tonen.

Nuttige
links: [View](https://reactnative.dev/docs/view), [Text](https://reactnative.dev/docs/text), [Button](https://reactnative.dev/docs/button),
[useState](https://react.dev/reference/react/useState), [style](https://reactnative.dev/docs/style),
[alert](https://reactnative.dev/docs/alert), [Progress](https://www.npmjs.com/package/react-native-progress)

<br><br>

### Opdracht 3 - Wisselende Achtergrondkleur

[Installeer](../guides/installatie.md) een nieuwe Expo app.
<br>
Bouw vervolgens een React Native-app met een enkele **Button** die de achtergrondkleur van het scherm verandert in een **vast patroon**. Zodra de reeks kleuren is doorlopen, begint deze opnieuw.

- Het scherm heeft een **witte achtergrond** bij de start.
- Er is één **Button** die de achtergrondkleur verandert.
- De kleuren veranderen in een **vaste volgorde** en herhalen zich zodra de reeks is doorlopen.
- De **Button zelf verandert ook van kleur** bij elke klik, los van de achtergrondkleur.

<br><br>

### Opdracht 4 - Random Quote Generator

[Installeer](../guides/installatie.md) een nieuwe Expo app.
<br>
Bouw vervolgens een React Native-app die bij elke druk op een knop een willekeurige quote ophaalt en toont.
Klik [hier](../assets/quotes.json) voor de quotes, klik vervolgens op "Raw" en kopieer dan de URL

- De app bevat een **Pressable** knop waarmee je een nieuwe quote kunt laden.
- De quote wordt dynamisch bijgewerkt zodra de knop wordt ingedrukt.
- Zorg voor een **stijlvolle vormgeving**, waarbij zowel de knop als de tekst duidelijk en aantrekkelijk worden weergegeven.

Nuttige links: [Pressable](https://reactnative.dev/docs/pressable),
[fetch](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API)

<br><br>

### Opdracht 5

nabouwen ontwerp

<br><br>

### Opdracht 6

toevoegen darkmode switch
