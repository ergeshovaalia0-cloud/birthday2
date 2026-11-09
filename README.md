# Once Upon a Time... My 20th Birthday

A romantic Disney Princess style birthday invitation built with React, Vite, and CSS animations. The project is ready for local development and Vercel deployment without a backend.

## Features

- animated opening cover
- luxury royal visual style
- princess dress code gallery with interactive selection
- RSVP form with localStorage save flow
- live countdown timer
- music toggle using Web Audio API
- responsive layout for mobile devices
- data stored in JSON files instead of a database

## Project structure

```text
birthday-invitation/
├── public/
│   └── favicon.svg
├── src/
│   ├── components/
│   │   ├── OpeningScreen.jsx
│   │   ├── Invitation.jsx
│   │   ├── EventDetails.jsx
│   │   ├── DressCode.jsx
│   │   ├── PrincessCard.jsx
│   │   ├── Wishes.jsx
│   │   ├── RSVP.jsx
│   │   └── Footer.jsx
│   ├── data/
│   │   ├── event.json
│   │   └── princesses.json
│   ├── styles/
│   │   ├── global.css
│   │   ├── animations.css
│   │   └── responsive.css
│   ├── App.jsx
│   └── main.jsx
├── index.html
├── package.json
├── vite.config.js
├── README.md
└── public/favicon.svg
```

## Install dependencies

```bash
npm install
```

## Run locally

```bash
npm run dev
```

Then open the local URL shown in the terminal, usually `http://localhost:5173`.

## Check production build

```bash
npm run build
```

## Preview production build

```bash
npm run preview
```

## Upload to GitHub

1. Create a new repository on GitHub.
2. In the project folder, run:

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin <your-github-repository-url>
git push -u origin main
```

## Connect to Vercel

1. Open https://vercel.com/
2. Sign in with GitHub.
3. Click `Add New Project`.
4. Import your repository.
5. Keep the default settings for Vite.
6. Click `Deploy`.

Vercel automatically detects React and Vite and publishes the app. No backend or database is required.

## Update date, time, address and name

Edit the content in `src/data/event.json`:

```json
{
  "birthdayLabel": "20th Birthday",
  "dateLabel": "[Укажите дату]",
  "timeLabel": "[Укажите время]",
  "locationLabel": "[Укажите место]",
  "googleMapsLink": "https://www.google.com/maps/search/?api=1&query=...",
  "birthdayDate": "2027-06-20T18:00:00",
  "hostName": "Your Birthday Girl"
}
```

Replace the placeholder values with your actual information and update the event date in `birthdayDate` to match your birthday.

## Notes

- The RSVP form uses `localStorage` for a static site flow.
- For a shared guest list, connect a serverless Vercel Function or an external API.
- Do not add a database to this project because the brief requires a frontend-only deployment.
