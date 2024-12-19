# Übungsaufgabe zur Wiederholung (JS Woche 1)

**Themenbereiche:**

- Variablen
- Datentypen
- Condition (if/else)

## Aufgaben

Erstelle für jede Aufgabe eine eigene Datei und führe diese anschließend im Terminal aus.
Überlege genau welche Variablen sich ändern können und welche nicht (const/let).

---

### Task 1

- Lege verschiedene Variablen mit deinen Daten an
  - firstname
  - age
  - isMarried

Erzeuge in einem `console.log()` einen Template String in dem der Satz ausgeben wird:

```js
"Ich heiße ... , bin ... Jahre alt und verheiratet.";
"Ich heiße ... , bin ... Jahre alt und nicht verheiratet.";
```

Achte darauf, dass die Leerzeichen stimmen!

---

### Task 2

Vorgaben

```js
const greeting = "Hallo";
let num = 13;
let bool = false;
let output;
```

- Kombiniere `greeting` und `num`
- Inkrementieren `num` um 1 (+1)
- ändere `bool` zu true
- speichere den letzten Satz in der Variable `output`
- erstelle verschiedene Ausgaben mit `console.log()` um folgende Ergebnisse zu erhalten

```js
"Hallo13";
"Ursprungszahl" 13
"neue Zahl" 14
true

`Hallo 13, ich bin 14, das ist true`
```

---

### Task 3

- Lege folgende Variablen an
  - price 6.20€
  - amount 4
  - discount 0.2
  - isDiscounted false
  - sum ?
- Überprüfe ob die Summe der 3 Artikel durch 2 Teilbar ist
  - Wenn die Summe durch zwei Teilbar ist, erhält der Käufer 20% Rabatt (discount)
  - Wenn die Summe nicht teilbar ist, erhält deri Käufer keinen Rabatt (discount)

---

### Task 4

Du möchtest deine Einnahmen und Ausgaben kontrollieren um zu wissen ob du etwas Geld beiseite legen kannst. Als Ziel setzt du dir, dass nach Abzug deiner Kosten 500€ überbleiben sollen um sparen zu können.

- Lege ein paar Variablen an
  - salary 1451
  - electric 93
  - internet 49.99
  - water 18
  - rent 683.24
  - purchase 250
- Berechne wie viel Geld nach Abzug aller Kosten noch bleibt und gibt das ganze als Währung aus

  - Output: "Gehalt: 12/24 356.77 €"
  - Output: "Sparen ist nicht möglich!"

- Dein Chef sagt dir, dass du ab Januar 2025 eine Gehaltserhöhung von 10% erhälst
  - überschreibe den urspränglichen Betrag mit der neuen Summe (+200)
  - gib erneut aus, wie viel Geld du nach Abzug der Kosten noch hast
  - überprüfe ob du mehr als 500€ über hast um zu wissen ob du nun auf den Sommerurlaub sparen kannst.
    - Output: "Gehalt: 01/25 501.87 €"
    - Output: "Sparen ist möglich!"

---

### Task 5

- Kopiere folgenden Code und versuche ihn zu kürzen
  - Beschreibe in einem Kommentar, was hier im Code geprüft wird

```js
const a = 4;

// ...dein Kommentar

if (a ** 2 > 10) {
  if (a ** 2 % 2 === 0) {
    console.log(`Die ${a ** 2} ist eine ... und ... 10`);
  }
}
```

---

### Task 6 (Advanced)

- installiere `readlineSync`
- stelle sicher, dass du Module in diesem Projekt verwenden kannst
- Der Benutzer soll folgende Angaben machen können
  - username
  - email
  - firstname
  - age
  - aboNewsletter?
- Überprüfe die getätigten Angaben auf folgendes
  - Der username muss mindestens 6 Zeichen lang sein und darf keine `Leerzeichen` und keine `*` enthalten
  - Die email sollte ein `@` enthalten
  - der firstname soll kleingeschrieben werden bzw. so gespeichert werden und eine Mindestlänge von 2 Buchstaben haben
  - Das Alter soll eine Zahl sein
- Datenverarbeitung

  - Erstelle aus dem 1. Buchstaben des `Usernames` und dem letzten Buchstaben des `Firstname` eine Zeichenkette mit 2 Buchstaben, die groß geschrieben sein soll
    - Beispiel: RN
  - Nehme nun die Länge des `firstname` und addiere das `age` darauf und Potenziere dies mit der Zahl 3
  - nehme diese Zahl und füge ein `#` davor
    - Beispiel: #64000
  - Aus Sicherheitsgründen darf die E-Mail Adresse nicht komplett angezeigt werden
    - Erzeuge einen String, der nur die ersten 3 Buchstaben und ab dem `@` Zeichen anzeigt.
    - Die Mitte soll `***` enthalten
      Beispiel: `mar***@web.de`

  **Output:**

  "Kürzel: RN"

  "Hash: #64000"

  `mar***@web.de`

---

### Task 7

- erstelle folgende Variable
  - `const chars = "abcdefghijklmnopqrstuvwxyz0123456789!-_*"`
- erstelle aus dem String ein Array, das jeden Buchstaben als eigenes Item beinhaltet
- generiere dir mit `Math` eine random Zahl, die einem Index entspricht (4x) und speichere die Zahlen in der Variable password und gib das password im Terminal aus.

Beispiel:

```js
"Password: h";
"Password: b";
"Password: l";
"Password: v";
```

- überprüfe jeden Buchstaben des Passworts ob es ein Sonderzeichen (!-\_\*) ist
  - Sollte eines der Zeichen ein Sonderzeichen sein, füge 1 weiteren char hinzu
  - Sollte kein Zeichen ein Sonderzeichen sein, sorge dafür das random eines der Sonderzeichen eingesetzt wird

---

### Bonus

Erstelle eine neue Datei und versuche Aufgabe 7 mit einer Schleife (Loop) zu lösen.
Nutze hierfür eine normale For-Schleife.

[For-Loop](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/for)
