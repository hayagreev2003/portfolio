# Hari Rama Hayagreev — Portfolio

Personal portfolio site showcasing my work as a full-stack developer building geospatial climate-intelligence platforms and AI multi-agent systems.

**Live:** https://hayagreev2003.github.io/portfolio/

## Sections

- **Hero** — intro, rotating roles and a link to my resume
- **Skills** — frontend, geospatial/visualisation, backend, data, AI/LLM and cloud tooling
- **Experience** — timeline of roles
- **Projects** — filterable cards (Web Apps / AI & ML) with a detail modal and live links
- **Education**
- **Footer** — quick navigation plus LinkedIn and GitHub links

## Tech Stack

- [React 18](https://react.dev/) (Create React App)
- [styled-components](https://styled-components.com/) for styling and theming
- [MUI](https://mui.com/) (icons, timeline components)
- [typewriter-effect](https://www.npmjs.com/package/typewriter-effect) for the hero roles
- [gh-pages](https://www.npmjs.com/package/gh-pages) for deployment to GitHub Pages

## Getting Started

Requires Node.js and npm.

```bash
git clone https://github.com/hayagreev2003/portfolio.git
cd portfolio
npm install
npm start
```

The dev server runs at http://localhost:3000.

## Updating Content

All content lives in [`src/data/constants.js`](src/data/constants.js):

| Export        | What it controls                                      |
| ------------- | ----------------------------------------------------- |
| `Bio`         | Name, roles, intro text, resume, GitHub and LinkedIn  |
| `skills`      | Skill groups and their logos                          |
| `experiences` | Experience timeline entries                           |
| `education`   | Education entries                                     |
| `projects`    | Project cards (`category`: `web app` or `machine learning`) |

Images (`image` / `img`) and project links (`github` / `webapp`) are optional; cards hide them when absent. Local images go in `src/images/` and are imported at the top of `constants.js`.

Colours are defined in [`src/utils/Themes.js`](src/utils/Themes.js). The favicon and app icons are in `public/`.

## Scripts

| Command          | Description                                   |
| ---------------- | --------------------------------------------- |
| `npm start`      | Run the development server                    |
| `npm run build`  | Create a production build in `build/`         |
| `npm test`       | Run tests in watch mode                       |
| `npm run deploy` | Build and publish `build/` to the `gh-pages` branch |

## Deployment

The site is hosted on GitHub Pages from the `gh-pages` branch. The `homepage` field in `package.json` sets the base path (`/portfolio`).

```bash
npm run deploy
```

## Contact

- LinkedIn: [hari-ramahayagreev](https://www.linkedin.com/in/hari-ramahayagreev-565a72200/)
- GitHub: [hayagreev2003](https://github.com/hayagreev2003)
