# 🚀 Jaime Molina — Personal Portfolio & Blog

[![Website](https://img.shields.io/badge/Website-mrlaley.github.io-007bff?style=flat-square&logo=github)](https://mrlaley.github.io)
[![Tech Stack](https://img.shields.io/badge/Built%20With-Astro%206.x-ff5d01?style=flat-square&logo=astro)](https://astro.build/)
[![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)](LICENSE)

This repository contains the source code for my personal portfolio and blog, hosted on GitHub Pages: **[mrlaley.github.io](https://mrlaley.github.io)**. 

Built using **Astro**, this website serves as a technical showcase of my academic projects, software engineering philosophies, and personal reflections on technology, computer science, and life.

---

## 👨‍💻 About Me

I am a **Technical Computer Science Student** at the **University of Twente** (Netherlands), specializing in Software Engineering, Distributed Systems, Algorithms, and Cybersecurity. Originally from Spain, I have a global mindset, with multilingual capabilities (fluent in Spanish, French, and English).

My approach to engineering is centered on solving complex challenges through logical thinking, rigorous methodology, and resilient design. Beyond writing code, I am highly interested in multi-cultural team organization, agile leadership, and sports.

---

## 🛠️ Tech Stack & Features

*   **Framework:** [Astro](https://astro.build/) — For blazing fast, content-driven websites.
*   **Content Management:** Markdown and MDX for rich, interactive blog posts and project details with custom schemas.
*   **Styling:** Vanilla CSS with custom theme variables, dark mode aesthetics, and modern transitions.
*   **SEO & Optimizations:**
    *   100/100 Lighthouse performance score.
    *   Automatic XML Sitemap generation (`@astrojs/sitemap`).
    *   RSS Feed support (`@astrojs/rss`).
    *   SEO-friendly metadata, canonical URLs, and Open Graph tags.
*   **Typography:** Atkinson Hyperlegible font (locally integrated for accessibility and readability).

---

## 📁 Repository Structure

```text
├── public/                  # Static assets (images, profile pictures, icons)
├── src/
│   ├── assets/              # Web assets (fonts, global graphics)
│   ├── components/          # Reusable Astro & UI components (Header, Footer, BaseHead)
│   ├── content/             # Structured data (Collections)
│   │   ├── blog/            # Blog posts (MD/MDX files categorized)
│   │   └── projects/        # Detailed reports of engineering projects
│   ├── layouts/             # Page layouts (BlogPost, ProjectPost)
│   ├── pages/               # Core routing pages (Index, About, Blog, Projects, 404)
│   ├── styles/              # Global stylesheet variables and base rules
│   └── consts.ts            # Global constants (site title, description)
├── astro.config.mjs         # Astro configuration file
├── package.json             # Dependencies and build scripts
└── tsconfig.json            # TypeScript configuration
```

---

## 🚀 Featured Projects

All project write-ups are located in `src/content/projects/` and rendered dynamically under the `/projects` route:

1.  🤖 **AI Dutch Chatbot** (`chatbot-dutch.md`)
    *   An intelligent conversational assistant leveraging modern LLM architectures, fine-tuning, and robust chat interface design.
2.  🗺️ **Integrated Navigation** (`integrated-navigation.md`)
    *   A navigation system modeled in UML, focusing on algorithmic pathfinding, clean code, and robust system architecture.
3.  🚀 **RoboTeam Twente** (`roboteam-twente.md`)
    *   Contributed to the multi-agent control software for autonomous robotic systems participating in RoboCup.
4.  🎲 **Go Game** (`go-game.md`)
    *   Implementation of the traditional game of Go using concurrent Java systems, strong object-oriented architectures, and AI opponents.
5.  🎨 **Graph Coloring** (`graph-coloring.md`)
    *   A detailed exploration of solving NP-complete graph coloring problems through efficient algorithms, heuristics, and performance analysis.
6.  🌐 **Custom Network Protocol** (`custom-network-protocol.md`)
    *   Design and implementation of a custom transport-layer protocol for reliable data transfer over unreliable networks.
7.  📊 **Social Media Analytics** (`social-media-analytics.md`)
    *   A full-stack analytics platform built to extract, clean, and visualize user engagement patterns.

---

## ⚙️ Local Development

### 1. Prerequisites
Ensure you have **Node.js** (version 22.12.0 or higher) installed on your system.

### 2. Installation
Clone the repository and install dependencies:
```sh
git clone https://github.com/MrLaley/mrlaley.github.io.git
cd mrlaley.github.io
npm install
```

### 3. Run Development Server
Start the local server at `http://localhost:4321`:
```sh
npm run dev
```

### 4. Build for Production
Build the optimized static files into the `dist/` directory:
```sh
npm run build
```

### 5. Preview Locally
Preview the production build locally:
```sh
npm run preview
```

---

## 🌐 Deployment to GitHub Pages

This portfolio is configured to publish automatically to **GitHub Pages** using **GitHub Actions**.

The main configurations are:
*   `astro.config.mjs`: `site` parameter configured to `https://mrlaley.github.io`.
*   Deployment is triggered automatically on pushes to the `main` branch via the workflow in `.github/workflows/astro.yml`.

---

## 📬 Contact & Connect

*   **Portfolio:** [mrlaley.github.io](https://mrlaley.github.io)
*   **LinkedIn:** [Jaime Molina García](https://www.linkedin.com/in/jaime-molina-garcía-0b75b73a8)
*   **Email:** [jaime.molina.tcs@gmail.com](mailto:jaime.molina.tcs@gmail.com)

---

*Made with ❤️ by Jaime Molina. Powered by Astro.*
