# HumanCap SAS - Official Website

Static website accompanying the official launch of HumanCap SAS, a Senegalese simplified joint-stock company specializing in vocational training, consulting services, and Excel-based applications. Currently in development (Phase 1 static, Phase 2 dynamic planned).

## Context

HumanCap SAS is a simplified joint-stock company (SAS in French) under Senegalese law, based in Dakar. The company is legally incorporated and currently in its official launch phase. It is led by Fadouga Brooklyn Diallo, President of HumanCap SAS.

This website serves as the company's official communication platform, presenting its services, showcasing its activities, and centralizing prospect contact. Its primary audiences include students, professionals seeking upskilling, women in career transition, institutional partners, and the general public in Senegal.

## Status

The project is in Phase 1 (static build). Sprint 1 is complete.

### Completed

- Project requirements documented (technical specifications and visual prototype)
- Technical stack decisions finalized (HTML5, vanilla CSS, vanilla JavaScript, no frameworks)
- Local repository initialized and development environment configured
- Three of five pages delivered: homepage, catalogue, contact
- All delivered pages W3C-validated and semantically structured
- Working internal navigation across all pages
- Functional HTML5 forms with native validation (certificate verification on homepage, contact form on contact page)

### Upcoming

- Sprint 2: remaining pages (news, FAQ), accessibility enhancements (skip-link, basic ARIA), and semantic refinements
- Sprint 3-4: CSS implementation (cascade, box model, Flexbox, Grid, custom properties, responsive design)
- Sprint 5: vanilla JavaScript for UI interactions, HTML5 form validation, and lazy loading
- Sprint 6: accessibility audit, basic SEO (Open Graph metadata), structured code comments, Phase 2 preparation

### Phase 2 (planned)

Backend integration in PHP (admin panel with CRUD, functional contact and registration forms), payment gateways (Wave, Orange Money, Mixx by Yas), and a chatbot. Out of scope until Phase 1 is delivered.

*Last updated: June 23, 2026*

## Tech Stack

The stack is intentionally minimalist, prioritizing web standards and fundamentals over framework dependencies.

### Phase 1 (current)

- HTML5 (semantic markup, native form validation)
- CSS3 (vanilla, no preprocessor, no framework)
- JavaScript (vanilla, ES6+)
- Git for version control

### Phase 2 (planned)

- PHP (server-side rendering, form processing, admin panel)
- Possibly MySQL or SQLite for data persistence (to be confirmed as the project evolves)

### Tooling

- Visual Studio Code as the editor (with project-specific configuration in `.vscode/settings.json`)
- Live Server extension for local development with hot reload
- cSpell with French dictionary for spell checking
- W3C Markup Validator for HTML conformance

### Documentation references

- [MDN Web Docs](https://developer.mozilla.org) for HTML, CSS, and JavaScript
- [php.net](https://www.php.net) for PHP (Phase 2)

## Project Structure

The project follows a conventional static website layout, with pages at the root and shared assets under `assets/`.

```text
humancap-site/
├── .vscode/
│   └── settings.json
├── assets/
│   ├── css/
│   │   └── style.css
│   ├── fonts/
│   ├── images/
│   └── js/
│       └── main.js
├── pages/
│   ├── actualites.html
│   ├── catalogue.html
│   ├── contact.html
│   └── faq.html
├── .gitignore
├── cspell.json
├── index.html
└── README.md
```
## Local Setup

Follow these steps to run the project locally.

### Prerequisites

- Git for cloning the repository
- A code editor (Visual Studio Code recommended)
- A modern web browser
- Optionally, the Live Server extension for VS Code for hot reload during development

### Installation

1. Clone the repository.
1. Navigate to the project folder.
1. Open it in your editor.

```bash
git clone <repository-url>
cd humancap-site
code .
```

### Running the site

Open `index.html` in VS Code and click "Go Live" in the bottom-right corner of the status bar. The site opens automatically in your default browser at `http://127.0.0.1:5500`.

If Live Server is not installed, you can also open `index.html` directly in a browser by double-clicking the file. Note that some behaviors (relative paths, and PHP-based features in Phase 2) will not work correctly in that mode.

## Code Conventions

These conventions are enforced project-wide for consistency and maintainability.

### Formatting

- Indentation: 2 spaces, no tabs
- Encoding: UTF-8
- End of line: LF (Unix line endings)
- Trailing whitespace removed on save
- Final newline at end of file

### Languages

- Code (variable names, CSS class names, file names, code comments, Git commit messages): English
- User-facing content (visible text on the website): French

### Naming

- CSS classes: kebab-case (e.g., `formation-card`, not `formationCard`)
- File names: kebab-case (e.g., `formation-informatique-standard.jpg`)
- HTML IDs: kebab-case (e.g., `id="recherche-certificat"`)

### Git workflow

- [Conventional Commits](https://www.conventionalcommits.org) style for commit messages (`type: description in imperative present tense`)
- One commit per logical unit of change
- Common types used: `feat`, `chore`, `fix`, `docs`

### Editor

- Project-specific VS Code settings stored in `.vscode/settings.json` (versioned with the project, applies to anyone cloning the repo)

## Author

**Mame Ibra Georges SENE**

Web developer in training, currently in the third year of a Bachelor's degree in Applied Mathematics and Computer Science (Mathematics specialization) at Université Numérique Cheikh Hamidou Kane. This project is an opportunity to put into practice the concepts learned at university while building a real client deliverable, developed as a paid project for HumanCap SAS.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
