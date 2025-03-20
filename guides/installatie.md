# Installatie

## Les 1

Check of node en npm de juiste versie hebben:

`node -v` versie 20 of 22

`npm -v` versie 10

- Installeer node/npm indien nodig: https://nodejs.org/en/download (Scroll naar beneden voor installer van een prebuilt
  versie)

## Les 2

Als het goed is heb je alle vereisten al om met Expo te werken.

Maak je eerste project aan door het volgende commando uit te voeren (vervang `newproject` voor de naam van jouw
project):

`npx create-expo-app newproject --template blank`

Update bij problemen eerst je npm: `npm install -g npm@latest`

Open het zojuist aangemaakte project in PhpStorm. Daarna kun je de app bekijken met de Expo Go app op je telefoon, door
in de terminal van je project het volgende uit te voeren:

`npm run start`

**Let op!** Je telefoon moet verbonden zijn met hetzelfde netwerk als je computer.

[Expo Go App en simulator opties](https://docs.expo.dev/get-started/set-up-your-environment/)
