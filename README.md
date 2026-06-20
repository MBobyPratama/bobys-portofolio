# Muhammad Boby Pratama — Developer Portfolio

Welcome to my personal developer portfolio website! This project is a highly-optimized, retro-designed showcase of my work, experience, education, and technical skills. Built on **Astro** and **Tailwind CSS**, it features a fully-responsive layout, modular component structures, and search engine optimization.

---

## 🚀 Tech Stack

* **Framework**: [Astro](https://astro.build/) (Static Site Generation)
* **Styling**: [Tailwind CSS](https://tailwindcss.com/)
* **Language**: [TypeScript](https://www.typescript.org/) & JavaScript
* **CMS Config**: [PagesCMS](https://pagescms.org/) (via `.pages.yml` file-based Git integration)

---

## 🛠️ Project Structure & Data Collections

The content on this website is managed dynamically using Astro's content layer and collections:
* **Projects** (`src/content/projects/`): Showcases key development works like *Skillo Backend* and *SEA Salon*.
* **Experience** (`src/content/resume/experience.yaml`): Detailed timeline of my professional roles.
* **Education** (`src/content/resume/education.yaml`): University and education background details.
* **Certifications** (`src/content/resume/certifications.yaml`): Active software development and database credentials.
* **Skills** (`src/content/skills-and-tools/skillsAndTools.yaml`): Organized stack layout categorizing languages, backend frameworks, databases & ORMs, frontend, and developer tools.

---

## ⚙️ Commands

All commands should be executed from the root of the project:

| Command | Action |
| :--- | :--- |
| `npm install` | Installs project dependencies |
| `npm run dev` | Starts local development server at `localhost:4321` |
| `npm run build` | Builds your static production site to `./dist/` |
| `npm run preview` | Previews the build output locally |

---

## ✍️ Editing Content with PagesCMS

This repository is pre-configured with [PagesCMS](https://pagescms.org/). To manage data:
1. Log in to PagesCMS using your GitHub account.
2. Link the repository `bobys-portofolio`.
3. Use the CMS dashboard sidebar to visually edit or add projects, experiences, certifications, education, and skills. Saves will automatically generate commits and push them to your repository, triggering your Vercel/Netlify host to rebuild.
