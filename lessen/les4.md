# Les 4

- [Les 4](#les-4)
  - [Persistent data](#persistent-data)
  - [Gebruikersinvoer](#gebruikersinvoer)
  - [Opdracht 4.1](#opdracht-41)
  - [Opdracht 4.2: Settings \& AsyncStorage](#opdracht-42-settings--asyncstorage)
  - [Opdracht 4.3](#opdracht-43)

## Persistent data

In mobiele apps is het soms nodig om gegevens lokaal op te slaan, bijvoorbeeld gebruikersvoorkeuren of een inlogsessie.

**AsyncStorage** is een eenvoudige key-value opslagmethode voor het opslaan van gegevens die tussen app-sessies
behouden moeten blijven. Het is vergelijkbaar met localStorage in de browser, maar werkt asynchroon en ondersteunt
grotere hoeveelheden data. <br> https://reactnavigation.org/docs/getting-started

Voor gevoelige gegevens, zoals wachtwoorden of tokens, kan je beter **Expo Secure Storage** gebruiken. Dit slaat
gegevens versleuteld op en maakt gebruik van de beveiligde opslagmechanismen van het besturingssysteem (bijv. de
Keystore op Android en de Keychain op iOS). Ook deze storage werkt asynchroon. <br>
https://docs.expo.dev/versions/latest/sdk/securestore/

Omdat deze opslagmechanismen alleen strings accepteren, moeten complexe gegevens eerst worden omgezet naar een string
met `JSON.stringify()`. Bij het ophalen kan je dan `JSON.parse()` gebruiken om het oorspronkelijke dataformaat weer
terug te krijgen.

<!--

AsyncStorage
AsyncStorage.setItem('my-key', value) / getItem('my-key);
Alleen stringdata => stringify

Expo Secure Storage
https://docs.expo.dev/versions/latest/sdk/securestore/

Standaard config is genoeg om als storage te gebruiken

SecureStore.setItemAsync(key, value);
SecureStore.getItemAsync(key);
-->

## Gebruikersinvoer

Bij React Native werkt gebruikersinvoer vergelijkbaar met formulieren in gewoon React met state-variabelen om de
ingevoerde waarden op te slaan.

Standaard gaat `TextInput` van tekst uit, maar je kunt ook kiezen voor een numeriek toetsenbord als er getallen
ingevoerd moeten worden (`keyboardType="numeric"`). Ook is het mogelijk om meerdere regels input in te laten voeren met
`multiline={true}`. Op een mobiel scherm kan het toetsenbord soms over invoervelden heen vallen. Om dit te voorkomen,
gebruik je een `KeyboardAvoidingView`.

[TextInput](https://reactnative.dev/docs/textinput)
[KeyboardAvoidingView](https://reactnative.dev/docs/keyboardavoidingview)

[SafeArea](https://docs.expo.dev/versions/latest/sdk/safe-area-context/)

## Opdracht 4.1

Zorg dat de keuze tussen light en dark mode van opdracht 2.6 bewaard blijft, ook als de app afgesloten en opnieuw
opgestart wordt.

## Opdracht 4.2: Settings & AsyncStorage

Bouw een React Native-app met **twee schermen** en gebruik een **Stack Navigator**. Het tweede scherm is een
**settingsscherm** waarin de gebruiker een naam en een leeftijd kan invoeren. Deze gegevens moeten vervolgens worden
weergegeven op het eerste scherm.

**Deel 1**

- **Scherm 1** toont in eerste instantie de melding `Nog geen gegevens bekend` wanneer er nog geen settings zijn
  opgeslagen in de **AsyncStorage**.
- Voeg in de **header** een knop toe met de tekst `Settings`, die **Scherm 2** opent.
- **Scherm 2** bevat twee **invoervelden** om een naam en een leeftijd in te voeren. Zorg ervoor dat het invoerveld
  voor de leeftijd een numeriek veld, zodat er alleen cijfers ingevoerd kunnen worden. Tot slot bevat dit scherm de
  knop **Opslaan**.
- Na drukken op de knop **Opslaan** moet je terug navigeren naar **Scherm 1**, waarbij de naam en leeftijd als
  parameters meegestuurd moeten worden.
  - Let op: standaard wordt er ook een back button getoond links in de header. Wanneer hierop wordt gedrukt hoeven de
    settings niet te worden meegestuurd, dus alleen wanneer op de knop **Opslaan** wordt gedrukt.
- Toon op **Scherm 1** de tekst `Hallo [NAAM], jij bent [LEEFTIJD] jaar oud.`, waarbij de placeholders vervangen moeten
  worden door de ingevoerde settings.

<br>

**Deel 2**

- De settings worden nu op **Scherm 1** getoond, maar wanneer je de app opnieuw opstart dan zijn deze settings weer
  weg. Zorg er daarom voor dat deze worden opgeslagen in de **AsyncStorage**, zodat ze ook na een herstart van de app
  worden getoond op **Scherm 1**.
- Zorg er ook voor dat de invoervelden op **Scherm 2** worden ingevuld met de gegevens uit de **AsyncStorage**

Nuttige links: [Header buttons](https://reactnavigation.org/docs/header-buttons/),
[Passing params to a previous screen](https://reactnavigation.org/docs/params/#passing-params-to-a-previous-screen)

## Opdracht 4.3

Ga verder met je code van opdracht 3.3. Voeg daaraan een Create, Update en Delete toe, en geef de gebruiker de keuze
tussen light en dark mode.
