# Les 2

- [Les 2](#les-2)
  - [React Native](#react-native)
  - [Expo](#expo)
  - [TSX vs JSX](#tsx-vs-jsx)
  - [Opdrachten](#opdrachten)
    - [Opdracht 1](#opdracht-1)
    - [Opdracht 2](#opdracht-2)
    - [Opdracht 3](#opdracht-3)
    - [Opdracht 4](#opdracht-4)
    - [Opdracht 5](#opdracht-5)
    - [Opdracht 6](#opdracht-6)

<br><br>

## React Native
React Native is een framework waarmee je mobiele apps kunt bouwen met JavaScript en React. 
In plaats van HTML en CSS worden native UI-componenten gebruikt, waardoor de app eruitziet en aanvoelt 
als een echte native app.

React Native werkt met een *bridge*, een tussenlaag die zorgt dat JavaScript de native API aan kan spreken.
Hierdoor kan je met JavaScript direct communiceren met de functies van een mobiel besturingssysteem, zoals toegang 
tot de camera of GPS.

Doordat er een bridge is voor Android en voor iOS kan je tijdens de ontwikkeling generieke elementen gebruiken.
In react heb je bijvoorbeeld heyt component `<Button>`, dat op Android vertaald wordt naar `android.widget.Button` en
op iOS naar `UIButton`. 

<br><br>

## Expo
Expo is een ontwikkelomgeving en toolset die het werken met React Native makkelijker maakt.

De Expo Go-app maakt het mogelijk om een app eenvoudig op de telefoon te bekijken, inclusief *live update* 
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

### Opdracht 1
Tijdens deze les zul je meerdere opdrachten uitvoeren. Voor iedere opdracht voer  je opnieuw onderstaande installatie uit,
wat dus betekent dat je voor iedere opdracht een nieuwe app maakt.

Maak je eerste Expo app door de [installatie van les 2](../guides/installatie.md) te volgen.
* Test de app op je telefoon
* Verander de standaard tekst naar 'Hello World', of een eigen creatieve tekst.

<br><br>

### Opdracht 2
[Installeer](../guides/installatie.md) een nieuwe Expo app. Maak een app waarmee je mensen kunt tellen die ergens in en uit lopen (bijvoorbeeld omdat er maar
maximaal 100 mensen tegelijk aanwezig mogen zijn van de brandweer).

* Je hebt de knoppen +1, -1, en reset
* De teller mag nooit kleiner dan 0 worden
* Toon een alert als iemand probeert de teller kleiner dan 0 te maken
* Zorg dat de app er netjes uitzien

Gebruik ```console.log``` om de flow van je app te debuggen.

> Klaar? Lukt het je ook om een progressbar van 0-100 toe te voegen?

Nuttige links: [View](https://reactnative.dev/docs/view), [Text](https://reactnative.dev/docs/text), [Button](https://reactnative.dev/docs/button),
[useState](https://react.dev/reference/react/useState), [style](https://reactnative.dev/docs/style),
[alert](https://reactnative.dev/docs/alert), [Progress](https://www.npmjs.com/package/react-native-progress)

<br><br>

### Opdracht 3
[Installeer](../guides/installatie.md) een nieuwe Expo app. Maak een app met één Button en stel de achtergrondkleur in op wit. 
* De knop verandert de achtergrondkleur
* Dit gaat in een vast patroon, dat herhaalt
* Voeg toe dat de button zelf ook van kleur verandert

<br><br>

### Opdracht 4
[Installeer](../guides/installatie.md) een nieuwe Expo app. Maak een app om een [willekeurige quote](../assets/quotes.json) op te halen en te tonen.
* Er is alleen een load/refresh-knop (gebruik hiervoor het Pressable component)
* Zorg dat de app er netjes uitzien door de knop en de quote te stylen

Nuttige links: [Pressable](https://reactnative.dev/docs/pressable),
[fetch](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API)

<br><br>

### Opdracht 5
nabouwen ontwerp

<br><br>

### Opdracht 6
toevoegen darkmode switch
