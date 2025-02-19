# Les 3

## Navigatie

Navigatie in React Native is vergelijkbaar met browserrouting in React, maar dan zonder URL's. In plaats van URL's
geef je zelf namen aan de verschillende schermen, die je gebruikt om te navigeren.

Bij navigeren kun je data meegeven en ontvangen, bijvoorbeeld om details van een item door te sturen naar een volgend
scherm.

Een `Stack Navigator` 'stapelt' schermen op elkaar, zodat je eenvoudig terug kunt navigeren. Dit lijkt op een terug-knop
in de browser. Je kunt de Stack Navigator gebruiken om te zorgen dat een gebruiker in een vast volgorde door de app
gaat.<br>
https://reactnavigation.org/docs/stack-navigator

Een `Bottom Tabs Navigator` creëert een navigatiebalk onderaan het scherm met tabbladen, wat in veel mobiele apps
gebruikt wordt. Hierbij kan je geen vaste volgorde afdwingen, wel is het mogelijk om binnen een Tab een Stack Navigator
te gebruiken.<br>
https://reactnavigation.org/docs/bottom-tab-navigator

## Lijsten

Op mobiel is de schermruimte beperkt en er is standaard geen scrollmechanisme zoals bij webpagina’s. Als je meer content
wilt tonen dan op één scherm past, gebruik je daarom een `ScrollView`.

Je zou gegevens uit een lijst kunnen tonen door een array te mappen naar `Text`-componenten binnen een `ScrollView`,
maar dat is niet efficiënt bij grote lijsten.

Voor betere performance van je app gebruik je een List View, omdat deze items alleen rendert als ze op het scherm
zichtbaar zijn. Onzichtbare items worden automatisch verwijderd om geheugen te besparen.

De `FlatList` gebruik je als alle items hetzelfde zijn, de `SectionList` als de items gegroepeerd zijn (per secties).

https://reactnative.dev/docs/scrollview<br>
https://reactnative.dev/docs/safeareaview<br>
https://reactnative.dev/docs/using-a-listview

#### Opdracht

Maak een app met 2 schermen, met behulp van een stack navigator.

* Een button op scherm 1 opent scherm 2
* Voeg een tweede button en een counter toe
* Toon op scherm 2 de waarde van de counter, door deze mee te sturen als param met de navigatie

#### Opdracht

2 schermen, statische lijst + gegevens doorsturen uit die lijst als je klikt

#### Opdracht

2 schermen, lijst ophalen van notes/chess + detailpagina