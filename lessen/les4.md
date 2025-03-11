# Les 4

- [Les 4](#les-4)
  - [Persistent data](#persistent-data)
  - [Gebruikersinvoer](#gebruikersinvoer)
  - [Opdracht 4.1](#opdracht-41)
  - [Opdracht 4.2: Persoonlijke welkomstboodschap](#opdracht-42-persoonlijke-welkomstboodschap)
  - [Opdracht 4.3](#opdracht-43)

## Persistent data

In mobiele apps is het soms nodig om gegevens lokaal op te slaan, bijvoorbeeld gebruikersvoorkeuren of een inlogsessie.

**AsyncStorage** is een eenvoudige key-value opslagmethode voor het opslaan van gegevens die tussen app-sessies behouden
moeten blijven. Het is vergelijkbaar met localStorage in de browser, maar werkt asynchroon en ondersteunt grotere
hoeveelheden data. <br> https://reactnavigation.org/docs/getting-started

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

Safe Area 'formulieren' Numeriek / Alfa

## Opdracht 4.1

Zorg dat de keuze tussen light en dark mode van opdracht 2.6 bewaard blijft, ook als de app afgesloten en opnieuw
opgestart wordt.

## Opdracht 4.2: Persoonlijke welkomstboodschap

Bouw een React Native-app met **twee schermen** en gebruik een **Stack Navigator**. Het tweede scherm is een
settingsscherm waarop je een naam moet kunnen invoeren. Zorg ervoor dat de app de naam onthoudt met **AsyncStorage**,
zodat een persoonlijke welkomstboodschap op het eerste scherm kan worden weergegeven.

**Functionaliteiten**

- **Scherm 1** toont een **algemene welkomstboodschap**.
- Plaats in de header een knop aan de rechterkant met de tekst `Settings` die **Scherm 2** opent wanneer je erop drukt.
- **Scherm 2** bevat een **invoerveld** waarin de gebruiker een naam kan typen.
- Nadat de gebruiker een naam invoert en terugkeert naar **Scherm 1**, wordt de algemene boodschap aangepast en wordt de
  naam weergegeven.
- De ingevoerde naam moet behouden blijven, ook na het afsluiten en opnieuw opstarten van de app.

## Opdracht 4.3

Ga verder met je code van opdracht 3.3. Voeg daaraan een Create, Update en Delete toe, en geef de gebruiker de keuze
tussen light en dark mode.
