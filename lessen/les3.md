# Les 3

- [Les 3](#les-3)
  - [Navigatie in React Native](#navigatie-in-react-native)
    - [Stack Navigator](#stack-navigator)
    - [Bottom Tabs Navigator](#bottom-tabs-navigator)
  - [Lijsten in React Native](#lijsten-in-react-native)
    - [List Views](#list-views)
  - [Opdracht](#opdracht)
  - [Opdracht](#opdracht-1)
  - [Opdracht](#opdracht-2)


## Navigatie in React Native

In React Native werkt navigatie anders dan in een browser. Er zijn geen URL’s zoals op het web, maar in plaats daarvan
gebruik je schermen. Elk scherm heeft een naam, en je kunt daartussen navigeren.

Bij navigeren kun je ook **data meegeven**. Bijvoorbeeld: als je een lijst met producten hebt, kun je bij een klik op
een product de details doorsturen naar het volgende scherm.

### Stack Navigator

Een `Stack Navigator` werkt als een stapel schermen, waarbij alleen het bovenste scherm zichtbaar is voor de gebruiker.
Wanneer je naar een nieuw scherm gaat, wordt dit **bovenop de stapel** geplaatst. Het vorige scherm blijft eronder staan
en verdwijnt niet uit het geheugen. Wanneer je op de terug-knop drukt, dan wordt het bovenste scherm **weggehaald**, en
zie je dus weer het vorige scherm.

Dit is vergelijkbaar met hoe een browsergeschiedenis werkt: als je een nieuwe pagina opent, kun je met de terug-knop
weer naar de vorige pagina.

https://reactnavigation.org/docs/stack-navigator

### Bottom Tabs Navigator

Een `Bottom Tabs Navigator` maakt een navigatiebalk onderin het scherm met tabbladen. Dit zie je vaak in apps zoals
Instagram of WhatsApp. Binnen elke tab zou je weer een Stack Navigator gebruiken als er binnen die tab tussen
verschillende schermen genavigeerd moet kunnen worden. 🔗 https://reactnavigation.org/docs/bottom-tab-navigator

<br><br>

## Lijsten in React Native

Een mobiele app heeft **geen oneindig groot scherm** en ook geen standaard scrollbar zoals in een webbrowser. Als je meer content wilt tonen dan op het scherm past, moet je zelf zorgen voor scroll-functionaliteit, bijvoorbeeld met een `ScrollView`.

Een `ScrollView` maakt scrollen mogelijk en werkt prima voor bijvoorbeeld tekstpagina’s. Maar als je een lijst met een onbekend aantal items wilt tonen, is een `ScrollView` minder geschikt. Dit komt omdat een `ScrollView` **alle** items in één keer laadt, zelfs als ze niet zichtbaar zijn. Bij lange lijsten kan dit veel geheugen verbruiken en je app trager maken. De oplossing hiervoor is om gebruikt maken van een `List View`.

### List Views

Een `List View` is een geoptimaliseerde manier om lijsten weer te geven. In tegenstelling tot een `ScrollView` laadt een List View alleen de items in die op dat moment op het scherm zichtbaar zijn. Dit maakt het efficiënter en voorkomt onnodig geheugenverbruik.

React Native biedt twee soorten List Views:

- **`FlatList`** → Het standaardcomponent voor het weergeven van een lijst met items.  
- **`SectionList`** → Voor een lijst met gegroepeerde items, zoals een alfabetische lijst met secties per letter.



https://reactnative.dev/docs/scrollview<br> https://reactnative.dev/docs/safeareaview<br>
https://reactnative.dev/docs/using-a-listview

<br><br>

## Opdracht

Maak een app met 2 schermen, met behulp van een stack navigator.

- Een button op scherm 1 opent scherm 2
- Voeg een tweede button en een counter toe
- Toon op scherm 2 de waarde van de counter, door deze mee te sturen als param met de navigatie

<br><br>

## Opdracht

2 schermen, statische lijst + gegevens doorsturen uit die lijst als je klikt

<br><br>

## Opdracht

2 schermen, lijst ophalen van notes/chess + detailpagina
