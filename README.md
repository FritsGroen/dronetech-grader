# DroneTech Grader

De **DroneTech Grader** is een Node.js-applicatie voor het digitaal nakijken van studentinzendingen.  
De tool is bedoeld als praktische beoordelingshulp voor opdrachten binnen **dronetechniek / techniekonderwijs** en kan gebruikt worden via een webinterface, GitHub Pages en Microsoft Teams.

## Doel van dit project

Met deze Grader kan een docent of beoordelaar:

- studentinzendingen laten analyseren
- AI-ondersteunde feedback laten genereren
- scores en opmerkingen controleren en aanpassen
- meerdere inzendingen achter elkaar laten nakijken
- de tool gebruiken via browser of als tab in Microsoft Teams

De applicatie is opgezet als een lichte en praktische oplossing voor intern onderwijsgebruik.

---

## Architectuur

De Grader bestaat uit twee delen:

### 1. Frontend
- draait als statische webpagina
- kan gehost worden via **GitHub Pages**
- bevat de gebruikersinterface voor:
  - chat / beoordeling
  - starten van nakijkacties
  - tonen van resultaten
  - aanpassen van score en feedback

### 2. Backend
- draait lokaal op een mini-pc of andere server
- gebouwd met **Node.js + Express**
- verwerkt aanvragen van de frontend
- communiceert met de OpenAI API
- kan via **ngrok** tijdelijk publiek bereikbaar worden gemaakt
- bevat de eigen logica voor beoordeling en routering

---

## Belangrijkste functies

- Nakijken van losse inzendingen
- Nakijken van meerdere inzendingen
- AI-gegenereerde feedback
- Scorevoorstel per student
- Handmatige controle door docent
- Werkt in browser
- Werkt als Microsoft Teams-tab
- Frontend en backend los van elkaar te beheren

---

## Technische stack

- **Node.js**
- **Express**
- **HTML / CSS / JavaScript**
- **OpenAI API**
- **GitHub Pages** voor frontend
- **ngrok** voor veilige tijdelijke publieke backend-url
- **Microsoft Teams** voor embed als tab

> Dit project gebruikt **Node.js**, dus geen Python-backend.

---

## Voorbeeldopzet

```text
DroneTech-Grader/
│
├── backend/
│   ├── server.js
│   ├── .env
│   ├── package.json
│   └── ...
│
├── frontend/
│   ├── index.html
│   ├── manifest.json
│   └── ...
│
└── README.md
