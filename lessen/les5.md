# Les 5

## Maps

React Native biedt ondersteuning voor het gebruik van kaarten in apps. Afhankelijk van het platform wordt automatisch de
juiste kaartendienst gekozen:

* Google Maps voor Android
* Apple Maps voor iOS

Met Expo Go is het mogelijk om kaarten te gebruiken zonder een API-key te configureren. Voor een productie-app is
dit wel nodig.

https://docs.expo.dev/versions/latest/sdk/map-view/ (MapView)<br>
https://github.com/react-native-maps/react-native-maps (Marker)

## Location

Mobiele apparaten kunnen hun locatie op verschillende manieren bepalen.

### Coarse Location (`LocationAccuracy.Low`)

Maakt gebruik van wifi-netwerken, mobiele zendmasten en IP-adressen. Dit is minder nauwkeurig (vaak binnen enkele
honderden meters), maar wel sneller en verbruikt minder energie (batterij).
Gebruik dit als nauwkeurigheid niet zo belangrijk is, bijvoorbeeld voor een weer-app.

### Fine Location (`LocationAccuracy.High`)

Hierbij wordt de GPS gebruikt, vaak in combinatie met andere sensoren op de telefoon (zoals gyroscoop en kompas). Dit
zorgt voor een zeer nauwkeurige plaatsbepaling (tot op enkele meters), maar heeft daardoor ook een hoger
batterijverbruik. Gebruik dit dus alleen als je echt precies moet weten waar iemand is, bijvoorbeeld voor een
navigatie-app.

Nodig voor navigatie-apps en precieze locatiebepalingen
Testen van locatie
Tijdens ontwikkeling kun je locatiefunctionaliteit testen op een emulator of een fysiek apparaat.

### Locatie-app testen

Om een locatie-app te testen zonder steeds naar buiten te hoeven, kan je gebruik maken van de opties in de Android
Emulator (Extended controls - Location) of iOS simulator (Features - Location). Ook is het mogelijk om op een Android
device een app te installeren om een fake locatie in te stellen.

https://docs.expo.dev/versions/latest/sdk/location/<br>
https://docs.expo.dev/versions/latest/sdk/location/#locationoptions (Accuracy)

#### Opdracht

toon eigen locatie op de kaart, voeg spoor (van markers) toe op de kaart als je beweegt

## Eindopdracht

Uitleg en start eindopdracht