---
title: Pokemon Team Builder
publishDate: 2019-12-01 00:00:00
img: /assets/pokemon-team-builder-home.webp
img_alt: Cards showing each individual pokemon and information
description: |
  A nostalgic, data-driven web app for building your dream Pokémon team — built with Astro, TypeScript, and the PokéAPI.
tags:
  - Dev
  - Astro
  - Design
---

##### Pokémon Team Builder

**Project Type:** Personal / Learning Project  
**Tech Stack:** Astro, TypeScript, Vanilla JavaScript, PokéAPI, LocalStorage

##### Overview

The Pokémon Team Builder is a web application that helps users build their ideal team of Pokémon using real-time data from the [PokéAPI](https://pokeapi.co/). It’s designed to make team planning simple, fun, and informative for casual fans and strategists alike.

This project is an **ongoing build** meant to showcase my full-stack JavaScript skills, particularly with Astro and clean front-end UX. It also reflects my passion for interactive, data-driven interfaces.

---

##### Features

- **Pokémon Grid Display**  
  Renders a list of Pokémon using data fetched from PokéAPI, including name, artwork, types, and stats.

- **Type-Based Styling**  
  Pokémon types, weaknesses, resistances, and immunities are color-coded for clarity and aesthetic consistency.

- **Stat Modals**  
  Each Pokémon card includes a “View Stats” button that opens a custom modal displaying:

  - Base stats
  - Weaknesses
  - Resistances
  - Immunities

- **Team Building Sidebar**  
  Users can build a team of up to 6 Pokémon:

  - “Add to Team” buttons instantly populate the sidebar
  - Pokémon are saved in **localStorage**, preserving the team on refresh
  - Team slots show sprites and names
  - Click to remove a Pokémon from the team instantly

- **Responsive Layout**  
  Designed to work well on both desktop and mobile with flexible grid layout and side panel.

---

##### Future Features (Planned)

- Filter Pokémon by generation, type, or region
- Team export and share functionality (e.g. JSON download or share link)
- Improved UI animations and transitions
- PvP stat comparisons and synergy indicators
- Backend integration to store teams per user

---

##### Goals

- Practice modern front-end patterns using Astro and TypeScript
- Learn how to consume and transform REST API data effectively
- Build scalable, component-driven UI logic
- Improve DOM scripting skills without relying on frameworks
- Create something fun and nostalgic to engage users

---

##### Status

This project is **actively being developed**. The core team builder and modal interface are in place, and additional features will be added in phases.

<!--[🔗 View Live Project](https://yourdomain.com/pokemon-builder)-->

[💻 GitHub Repository](https://github.com/Webzel/pokemon-team-builder)
