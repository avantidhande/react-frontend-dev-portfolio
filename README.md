Avanti Dhande – React Portfolio 

A minimal, multilingual, mobile‑friendly portfolio built with Create React App and Sass.Forked from the excellent react‑frontend‑dev‑portfolio and customised for my own needs.

🚀 Live Demo

https://avantidhande.github.io/react-frontend-dev-portfolio/

🌟 Highlights

Multilingual – content pulled from JSON files so adding a new language is just another JSON file.

Mobile‑first & responsive – looks great on phones, tablets and desktops.

Light / Dark modes – built‑in theme switcher with localStorage persistence.

Data‑driven – all About / Skills / Experience / Projects sections live in public/data/*.json.

Clean & minimal – easy to read, easy to extend.

One‑click deploy – GitHub Pages ready via npm run deploy.

🛠 Getting Started

Tested with Node v20+ (uses the --openssl-legacy-provider flag for Webpack‑4 compatibility).

# 1  Clone the repo (or download the ZIP)
git clone https://github.com/avantidhande/react-frontend-dev-portfolio.git
cd react-frontend-dev-portfolio

# 2  Install dependencies
npm install

# 3  Fix the homepage path for local dev
#    Either delete the line entirely or set it to a single dot (.) in package.json

# 4  Start the dev server
npm start
#    Now browse to http://localhost:3000 and customise data/components.

Deployment to GitHub Pages

Set the correct homepage URL in package.json before deploying:

{
  "homepage": "https://avantidhande.github.io/react-frontend-dev-portfolio/"
}

Ensure the gh-pages package is installed (already in devDependencies).

From the project root run:

npm run deploy

This will build a production bundle and push it to the gh-pages branch.Your site will be live at the URL above within a minute.

Windows / PowerShell users: the build and start scripts already include NODE_OPTIONS=--openssl-legacy-provider for Node 17+ compatibility. No extra steps required.


📝 Customising Content

Text / links / images → edit the JSON files in public/data/.

Add skills / projects → append objects in the relevant JSON arrays.

Colours & fonts → tweak SCSS variables in src/themes/.

Add sections → create a component in src/components/ and register it in App.js.
