# 📊 CDF / EFK – Parliament Interpellations Widget (Scriptable)

This Scriptable widget displays recent parliamentary interpellations that explicitly mention the Swiss Federal Audit Office:

- 🇫🇷 Contrôle fédéral des finances (CDF)
- 🇩🇪 Eidgenössische Finanzkontrolle (EFK)

The widget automatically queries Curia Vista (parlament.ch) once per day and highlights new interpellations as well as the three most recent ones.

---

## Features

- Searches Curia Vista for references to:
  - “Contrôle fédéral des finances” (French)
  - “Eidgenössische Finanzkontrolle” (German)
- Displays newly detected interpellations on a single line (numbers only)
- Displays the three most recent interpellations
- Automatic language detection (FR / DE)
- Tap the widget to open the corresponding Curia Vista search
- Local caching to detect new interpellations between updates
- Automatic daily update (default time: 00:30)

---

## Requirements

- iOS or iPadOS
- Scriptable app  
  https://apps.apple.com/app/scriptable/id1405459188

---

## Installation

1. Install the Scriptable app from the App Store.
2. Create a new script in Scriptable.
3. Paste the full JavaScript code of this repository into the editor.
4. Save the script (for example: `CDF_EFK_Parliament_Widget`).
5. Add a Scriptable widget to your home screen.
6. Select the saved script in the widget settings.

---

## Language Selection

The widget automatically detects the device language.

You can force the language by setting a widget parameter:

- `fr` → French
- `de` → German

---

## Update Logic

- The widget checks Curia Vista once per day at 00:30.
- Previously detected interpellation numbers are stored locally.
- Newly detected interpellations are highlighted in the widget.

You can change the update time directly in the script:

```js
const UPDATE_HOUR = 0;
const UPDATE_MINUTE = 30;

---

## Data Sources

Curia Vista (French):
https://www.parlament.ch/fr/ratsbetrieb/suche-curia-vista

Curia Vista (German):
https://www.parlament.ch/de/ratsbetrieb/suche-curia-vista

--

## Disclaimer

This widget relies on publicly available HTML pages from parlament.ch.
Changes to page structure or wording may require updates to the parsing logic.
