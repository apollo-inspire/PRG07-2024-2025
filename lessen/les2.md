# Les 2

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

## Expo
Expo is een ontwikkelomgeving en toolset die het werken met React Native makkelijker maakt.

De Expo Go-app maakt het mogelijk om een app eenvoudig op de telefoon te bekijken, inclusief *live update* 
terwijl `console.log`s op je PC te lezen zijn. Gebruik dit voor debugging.

## TSX vs JSX
De officiële documentatie van Expo gebruikt tegenwoordig TypeScript (`.tsx` bestanden), terwijl wij in deze 
cursus met JavaScript (`.jsx` bestanden) werken.

TypeScript lijkt erg op JavaScript, maar voegt daaraan typedeclaraties (en controle) toe. 
Als je documentatie tegenkomt met TypeScript-code (Bijv. `:string`), kun je deze meestal eenvoudig omzetten naar 
JavaScript door de type-aanduidingen weg te laten.


#### Opdracht
Installatie // TODO: installatiestappen toevoegen of link naar Expo


### UI - output
View https://reactnative.dev/docs/view 
Tekst https://reactnative.dev/docs/text 

### Styles
https://reactnative.dev/docs/style 

stylesheets

### UI - input
Button https://reactnative.dev/docs/button
Pressable https://reactnative.dev/docs/pressable 


#### Opdracht
Maak een app waarmee je mensen kunt tellen die ergens in en uit lopen (bijvoorbeeld omdat er maar
maximaal 100 mensen tegelijk aanwezig mogen zijn van de brandweer).

* Je hebt de knoppen +1, -1, en reset
* De teller mag nooit kleiner dan 0 worden
* Toon een alert als iemand probeert de teller kleiner dan 0 te maken
* Zorg dat de app er netjes uitzien

Gebruik ```console.log``` om de flow van je app te debuggen.

> Klaar? Lukt het je ook om een progressbar van 0-100 toe te voegen?

Nuttige links: [Text](https://reactnative.dev/docs/text), [Button](https://reactnative.dev/docs/button),
[useState](https://react.dev/reference/react/useState), [style](https://reactnative.dev/docs/style),
[alert](https://reactnative.dev/docs/alert), [Progress](https://www.npmjs.com/package/react-native-progress)

#### Opdracht
Maak een App met één Button, en achtergrondkleur wit. 
* De knop verandert de achtergrondkleur
* Dit gaat in een vast patroon, dat herhaalt
* Voeg toe dat de button zelf ook van kleur verandert

#### Opdracht
Maak een app om een [willekeurige quote](../assets/quotes.json) op te halen en te tonen.
* Er is alleen een load/refresh-knop (gebruik hiervoor geen Button component)
* Zorg dat de app er netjes uitzien

Nuttige links: [Pressable](https://reactnative.dev/docs/pressable),
[fetch](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API)

#### Opdracht
nabouwen ontwerp

#### Opdracht
toevoegen darkmode switch
