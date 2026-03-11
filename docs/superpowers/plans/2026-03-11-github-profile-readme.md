# GitHub Profile README Redesign Implementation Plan

> **For agentic workers:** REQUIRED: Use superpowers:subagent-driven-development (if subagents available) or superpowers:executing-plans to implement this plan. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Rewrite the GitHub profile README to be clean, readable, and informative — with a hero banner, about blurb, tech stack badges, GitHub stats cards, and featured projects.

**Architecture:** Single `README.md` rewrite using standard GitHub markdown, shields.io badges, and github-readme-stats. Three unused SVG files are deleted. The ponokai.svg banner is retained as-is.

**Tech Stack:** GitHub Markdown, shields.io badge API, github-readme-stats API

**Spec:** `docs/superpowers/specs/2026-03-11-github-profile-readme-design.md`

**Git:** All git operations (commits, push) are handled by the user. Claude makes only file edits and deletions.

---

## Chunk 1: Cleanup and Hero + About

### Task 1: Delete unused SVG files

**Files:**
- Delete: `introduction.svg`
- Delete: `linkedin.svg`
- Delete: `shawilly.dev.svg`

- [ ] **Step 1: Delete the three unused SVG files**

Delete `introduction.svg`, `linkedin.svg`, and `shawilly.dev.svg` from the repo root. These are no longer referenced by the new README.

---

### Task 2: Write Hero + About sections

**Files:**
- Modify: `README.md` (full rewrite)

- [ ] **Step 1: Replace README.md with Hero and About sections**

Replace the entire contents of `README.md` with:

```markdown
<div align="center">
  <a href="https://github.com/shawilly/ponokai">
    <img src="ponokai.svg" width="800" height="400" alt="ponokai color scheme">
  </a>

  <h2>Shane Williams · Senior Full-Stack Engineer</h2>
  <p>Building scalable systems at the intersection of IoT, cloud, and developer tooling</p>

  <a href="https://github.com/shawilly">
    <img src="https://img.shields.io/badge/GitHub-shawilly-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub">
  </a>
  <a href="https://www.linkedin.com/in/shanewilliamsdev">
    <img src="https://img.shields.io/badge/LinkedIn-Shane%20Williams-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
  </a>
  <a href="https://shawilly.dev">
    <img src="https://img.shields.io/badge/Website-shawilly.dev-ff8c9a?style=for-the-badge&logo=firefox&logoColor=white" alt="Website">
  </a>
</div>

---

## About

5+ years building enterprise production systems. Currently architecting IoT energy management platforms at ResourceKraft — real-time data from thousands of devices. Previously scaled tooling at BioRender for 4M+ scientists worldwide.
```

---

## Chunk 2: Tech Stack + Stats + Projects

### Task 3: Add Tech Stack section

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Append Tech Stack section to README.md**

Append after the About section:

```markdown

---

## Tech Stack

**Languages**

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat&logo=go&logoColor=white)
![Lua](https://img.shields.io/badge/Lua-2C2D72?style=flat&logo=lua&logoColor=white)

**Frontend**

![React](https://img.shields.io/badge/React-61DAFB?style=flat&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat&logo=nextdotjs&logoColor=white)
![Expo](https://img.shields.io/badge/Expo-000020?style=flat&logo=expo&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=flat&logo=tailwindcss&logoColor=white)
![Sass](https://img.shields.io/badge/Sass-CC6699?style=flat&logo=sass&logoColor=white)

**Backend**

![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=nodedotjs&logoColor=white)
![Fastify](https://img.shields.io/badge/Fastify-000000?style=flat&logo=fastify&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat&logo=express&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-FF4438?style=flat&logo=redis&logoColor=white)
![InfluxDB](https://img.shields.io/badge/InfluxDB-22ADF6?style=flat&logo=influxdb&logoColor=white)
![MQTT](https://img.shields.io/badge/MQTT-660066?style=flat&logo=mqtt&logoColor=white)

**Cloud & Infra**

![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat&logo=amazonwebservices&logoColor=white)
![GCP](https://img.shields.io/badge/GCP-4285F4?style=flat&logo=googlecloud&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat&logo=nginx&logoColor=white)
![Keycloak](https://img.shields.io/badge/Keycloak-4D4D4D?style=flat&logo=keycloak&logoColor=white)
![Turborepo](https://img.shields.io/badge/Turborepo-EF4444?style=flat&logo=turborepo&logoColor=white)

**Tools**

![Neovim](https://img.shields.io/badge/Neovim-57A143?style=flat&logo=neovim&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black)
![Fish](https://img.shields.io/badge/Fish-4aaa48?style=flat&logo=fishshell&logoColor=white)
```

---

### Task 4: Add GitHub Stats section

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Append GitHub Stats section to README.md**

Append after the Tech Stack section:

```markdown

---

## GitHub Stats

<table align="center">
  <tr>
    <td>
      <img src="https://github-readme-stats.vercel.app/api?username=shawilly&show_icons=true&count_private=true&bg_color=333648&title_color=ff8c9a&text_color=f8e7b0&icon_color=98d4e7&border_color=393e53" alt="GitHub Stats">
    </td>
    <td>
      <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=shawilly&layout=compact&bg_color=333648&title_color=ff8c9a&text_color=f8e7b0&icon_color=98d4e7&border_color=393e53" alt="Top Languages">
    </td>
  </tr>
</table>
```

> **Note:** github-readme-stats uses Vercel's public deployment. If cards show "This deployment has been banned" or rate limiting, self-deploy via the [github-readme-stats docs](https://github.com/anuraghazra/github-readme-stats#deploy-on-your-own) or use the official instance with a PAT.

---

### Task 5: Add Featured Projects section

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Append Featured Projects section to README.md**

Append after the GitHub Stats section:

```markdown

---

## Featured Projects

**[ponokai](https://github.com/shawilly/ponokai)** — Pastelly Monokai color scheme for Vim/Neovim
`Vim Script` `Lua`

**[shell-quest](https://github.com/shawilly/shell-quest)** — Pirate-themed CLI learning game for kids
`Go`

**[react-simple-devicons](https://github.com/shawilly/react-simple-devicons)** — React SVG dev icon library
`TypeScript`
```

---

## Final Verification (after user pushes)

Visit `https://github.com/shawilly` and confirm:
- ponokai banner at top, links to ponokai repo ✓
- Name, title, tagline, three hero badges ✓
- About paragraph ✓
- Tech Stack — all five badge groups with logos ✓
- GitHub Stats — two cards with ponokai colours ✓
- Featured Projects — three entries with inline code tags ✓
