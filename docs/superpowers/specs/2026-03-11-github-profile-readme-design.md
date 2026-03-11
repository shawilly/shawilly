# GitHub Profile README Redesign

**Date:** 2026-03-11
**Repo:** github.com/shawilly/shawilly

## Overview

Redesign the GitHub profile landing page README to be clean, readable, and informative. Replace all custom SVGs (except the ponokai banner) with standard markdown + shields.io badges and github-readme-stats cards.

## Sections

### 1. Hero
- Ponokai banner (`ponokai.svg`) retained at the top, centered
- Text header below: name + title (`Shane Williams · Senior Full-Stack Engineer`)
- Tagline: "Building scalable systems at the intersection of IoT, cloud, and developer tooling"
- Inline icon/badge links: GitHub profile, LinkedIn, shawilly.dev

### 2. About
Three sentences, factual and tight:
> 5+ years building enterprise production systems. Currently architecting IoT energy management platforms at ResourceKraft — real-time data from thousands of devices. Previously scaled tooling at BioRender for 4M+ scientists worldwide.

### 3. Tech Stack
Shields.io flat badges grouped by category:
- **Languages:** TypeScript, JavaScript, Go, Lua
- **Frontend:** React, Next.js, Expo, Tailwind CSS, Sass
- **Backend:** Node.js, Fastify, Express, PostgreSQL, MongoDB, Redis, InfluxDB, MQTT
- **Cloud & Infra:** AWS, GCP, Docker, Nginx, Keycloak, Turborepo
- **Tools:** Neovim, Git, Linux, Fish

### 4. GitHub Stats
Two `github-readme-stats` cards centered side by side:
- GitHub Stats card (stars, commits, PRs, issues, contributions)
- Top Languages card

Both use a dark theme consistent with the ponokai banner aesthetic.

### 5. Featured Projects
Three pinned open source projects as a markdown list with links:
- **[ponokai](https://github.com/shawilly/ponokai)** — Pastelly Monokai color scheme for Vim/Neovim · `Vim Script` `Lua`
- **[shell-quest](https://github.com/shawilly/shell-quest)** — Pirate-themed CLI learning game for kids · `Go`
- **[react-simple-devicons](https://github.com/shawilly/react-simple-devicons)** — React SVG dev icon library · `TypeScript`

## Files Changed
- `README.md` — full rewrite
- `introduction.svg` — removed
- `linkedin.svg` — removed
- `shawilly.dev.svg` — removed
- `ponokai.svg` — retained

## Design Principles
- No custom SVG animations beyond the ponokai banner
- Readable on both light and dark GitHub themes (dark stat card theme)
- Scannable in under 10 seconds
- No redundant or decorative elements
