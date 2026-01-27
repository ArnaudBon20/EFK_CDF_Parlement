This Scriptable widget displays recent parliamentary interpellations that explicitly mention the Swiss Federal Audit Office:

🇫🇷 Contrôle fédéral des finances (CDF)

🇩🇪 Eidgenössische Finanzkontrolle (EFK)

The widget automatically checks Curia Vista (parlament.ch) once per day and highlights new interpellations as well as the three most recent ones.

✨ Features

🔍 Searches Curia Vista in:

French: “Contrôle fédéral des finances”

German: “Eidgenössische Finanzkontrolle”

🆕 New interpellations listed on a single line (numbers only)

📄 Three latest interpellations displayed below

🌍 Automatic FR / DE language detection

🔗 Tap the widget to open the corresponding Curia Vista search

💾 Local cache to detect what is new since the last update

⏰ Automatic daily update (default: 00:30)

🧩 What the Widget Displays
Le CDF au Parlement
Nouvelles: 25.3012 / 25.2987
25.3012
25.2987
25.2874


or (German):

Die EFK im Parlament
Neu: 25.3012
25.3012
25.2987
25.2874


Only interpellation numbers are shown – no dates, no titles.

⚙️ Requirements

📱 iOS / iPadOS

📦 Scriptable

🚀 Installation

Install Scriptable from the App Store

Create a new script

Paste the full JavaScript code into the editor

Save the script (e.g. CDF_EFK_Parliament_Widget)

Add a Scriptable widget to your home screen

Select the script

🌐 Language Selection

The widget detects the language automatically based on your device locale.

You can force the language via the widget parameter:

fr → French

de → German

Example:
Long-press the widget → Edit Widget → Widget Parameter → de

🔄 Update Logic

The widget refreshes once per day at 00:30

Previously seen interpellation numbers are stored locally

Any newly detected numbers appear under “New / Nouvelles / Neu”

You can adjust the update time in the script:

const UPDATE_HOUR = 0;
const UPDATE_MINUTE = 30;

🔗 Data Sources

Curia Vista (French):
https://www.parlament.ch/fr/ratsbetrieb/suche-curia-vista

Curia Vista (German):
https://www.parlament.ch/de/ratsbetrieb/suche-curia-vista

⚠️ Disclaimer

This widget uses publicly available HTML pages from parlament.ch.
Parsing relies on page structure and keywords (“Interpellation / Interpellationen”), which may change over time.

📄 License

MIT License
Free to use, adapt, and improve.
