# Les 1

- [Les 1](#les-1)
- [JavaScript](#javascript)
  - [Opdracht 1: Mini-puzzels](#opdracht-1-mini-puzzels)
    - [Werkwijze](#werkwijze)
  - [Opdracht 2: Overzicht van Emoji's 🤯](#opdracht-2-overzicht-van-emojis-)
    - [Opdrachten](#opdrachten)
  - [Front-end Frameworks](#front-end-frameworks)
    - [Opdracht](#opdracht)


# JavaScript

**AANTEKENING: onderwerpen om te herhalen:**

- Ternary & nullish coalescing operators
- Optional chaining
- Spread & rest
- Destructuring Arrays & Objects
- Arrow functions & this scope
- Events
- Array & Object Iteration
- Promises
- Try/catch
- Fetch
- Await/async

<br><br>

## Opdracht 1: Mini-puzzels
Deze opdracht bestaat uit een reeks **JavaScript mini-puzzels**, waarbij elke puzzel zich richt op een specifieke
techniek binnen JavaScript. Dit is een oefening om belangrijke concepten te herhalen en toe te passen in kleine,
gerichte codevoorbeelden.

### Werkwijze

1. Kopieer de [startcode van de puzzels](../startcode/les1/puzzels.js) naar een eigen document.
2. Elke puzzel begint met een titel en een korte uitleg in **commentaar**.
3. Onder de uitleg staat `// Schrijf hier de code...`. **Vervang dit door jouw oplossing.**
4. Onder de code staan **console.logs** die de code testen. **Haal deze uit commentaar** om je oplossing te controleren.
5. Test je code door het bestand met node te starten (`node puzzels.js`), of druk op de Run-knop in PhpStorm.

<br><br>

## Opdracht 2: Overzicht van Emoji's 🤯

Je gaat een kleine Javascript applicatie bouwen die je via nodeJS aan
gaat roepen. In deze applicatie ga je een lijst tonen van beschikbare emojis met
hun bijbehorende categorie, htmlCode en unicode. Je geeft 2 argumenten mee
aan dit script die invloed hebben op de output.

1. Argument die resultaten filtert op categorie. Bij 'all' krijg je alles
2. Argument die bepaalt of je een API gebruikt of je eigen data

Dit doe je via je command line via het volgende commando:

```shell
node script.js all api #toont alle data vanuit de API
node script.js symbols own #filtert op categorie en toont eigen data
```

In je Javascript kun je bij het aanroepen van een script via Node,
de argumenten op de volgende manier ophalen:

```javascript
const arguments = process.argv.slice(2);
```

De slice zorgt ervoor dat de eerste 2 argumenten die standaard
meegegeven worden (pad van Node, en pad van het aangeroepen bestand),
eraf gehaald worden en je alleen de argumenten overhoudt die voor jou
relevant zijn.

### Opdrachten

1. Maak een array met objecten aan waarin je een lijst met emojis te zien krijgt.
    * Zorg dat je minimaal 10 items hebt met verschillende waardes. Hou hierbij de structuur aan zoals in de [API](https://emojihub.yurace.pro/api/all)
2. Loop door de informatie heen met een `for...of` loop en console.log de waardes. Log de eigenschappen
   per entry door middel van template strings.
3. Gebruik `destructuring` om de arguments op regel 1 van je script op te halen en gelijk om te zetten naar variabelen
   met logische namen
4. Plaats voor de `for...of` loop een `.filter` om de data te filteren op category. Gebruik de arrow notatie voor je callback functie.
    * Gebruik als dit werkt een if statement om te voorkomen dat de data gefilterd wordt wanneer de category 'all' is.
    * Vervang daarna het if statement door de `ternary operator`.
5. Gebruik `fetch` om de data van de daadwerkelijke API in te laden.
    * Het tweede argument bepaalt of je jouw eigen data of de data van de API gaat gebruiken.
    * Gebruik in deze versie nog de `.then()`/`.catch()` notatie.
6. Schrijf de `fetch` om door gebruik te maken van `async`/`await` i.p.v. `.then()`/`.catch()`.
7. Bedenk een slimme manier om beide scenario's (eigen data & API-data) dezelfde filter logica
   te laten gebruiken en dubbele code te voorkomen.
8. Toon als category 'list' gebruikt wordt een lijst met alle beschikbare categorieën. Je output zijn nu dus geen emojis meer,
   maar alle categorieën die bestaan.

<br><br>

## Front-end Frameworks
Werking van een framework/useState 

<br><br>

### Opdracht
Om meer inzicht te krijgen in de werking van een framework, gaan we zelf...
case: mini-react


