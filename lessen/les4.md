# Les 4

- [Les 4](#les-4)
  - [Persistent data](#persistent-data)
  - [Gebruikersinvoer](#gebruikersinvoer)
  - [Opdracht](#opdracht)
  - [Opdracht](#opdracht-1)


## Persistent data

In mobiele apps is het soms nodig om gegevens lokaal op te slaan, bijvoorbeeld gebruikersvoorkeuren of een inlogsessie.

**AsyncStorage** is een eenvoudige key-value opslagmethode voor het opslaan van gegevens die tussen app-sessies behouden
moeten blijven. Het is vergelijkbaar met localStorage in de browser, maar werkt asynchroon en ondersteunt grotere
hoeveelheden data.
<br>
https://reactnavigation.org/docs/getting-started

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

## Opdracht

kleine oefenopdracht met invoer en storage (bijv. 2 schermen, 1e scherm welkom, 2e scherm laat naam opslaan, 1e scherm
toont 'Hallo ...' ook na afsluiten)

## Opdracht

grote opdracht: CRUD + opmaak + darkmode (in storage)
