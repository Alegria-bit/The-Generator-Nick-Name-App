# Nickname Generator Web App

A simple Node.js + Express + EJS web application that generates creative nicknames by combining a random adjective and noun.

## 🚀 Project Overview

- Built with `Node.js`, `Express`, and `EJS` templating.
- Uses `body-parser` to parse form data.
- Serves a static front-end via `public/` and styled using Bootstrap + custom CSS.
- Contains a large internal word list for generating nickname pairs.

## 📁 Repository Structure

- `index.js`: main server app.
- `package.json`: Node metadata and dependencies.
- `views/index.ejs`: homepage template with generated nickname output.
- `views/partials/header.ejs`, `views/partials/footer.ejs`: shared page layout.
- `public/styles/main.css`: custom styling.

## 🛠️ Installation

1. Clone repository

```bash
git clone <repo-url>
cd "The-Generator-Nick-Name-App"
```

2. Install dependencies

```bash
npm install
```

## ▶️ Run locally

```bash
npm start
# or
node index.js
```

Open browser at `http://localhost:3000`

## 🎮 Usage

1. Open the app in your browser.
2. Click `Generate Name` to produce a new nickname from a random adjective + noun.
3. Use `Home Page` to reset the view.

## 🧩 Application Behavior

- GET `/`: renders `index.ejs` with default header text.
- POST `/submit`: chooses a random word from `adj` and `noun` arrays; renders `index.ejs` with generated nickname.

## 🔧 Dependencies

- `express` ^4.18.2
- `ejs` ^3.1.9
- `body-parser` ^1.20.2

## 🧪 Testing

No test suite is included at present. You can validate manually:

- start server
- submit nickname generation form
- see generated nickname

## 📌 Notes

- The app uses a hard-coded array for adjectives and nouns inside `index.js`.
- Customize `adj` and `noun` arrays to include more nickname possibilities.

## 🫶 License

MIT / ISC (as defined in `package.json`).
