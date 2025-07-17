---
title: Internal Employee Portal
publishDate: 2020-03-02 00:00:00
img: /assets/Portal-Login.webp
img_alt: Portal login screen card with button to login
description: |
  I built an internal employee portal for Catapult Creative, designed to centralize tools, calendars, and documentation.
tags:
  - Dev
  - Design
  - User Testing
---

While working at Catapult Creative, I built an internal employee portal designed to centralize essential tools, resources, and documentation for the team. The goal was to replace scattered bookmarks and Slack links with a single, well-organized hub that employees could rely on daily. The portal helped streamline internal workflows, improved access to key information, and reduced friction across departments.

The project was built using Astro, with a custom React component to integrate the company’s shared Google Calendar directly into the interface. I also created a page that dynamically pulled content from the company's main Google Drive folder, allowing employees to browse shared files without leaving the portal. For internal documentation, I leveraged Astro’s Starlight theme to build a clean, searchable knowledge base — making it easy for the team to find onboarding guides, process docs, and reference materials in one place.

##### My Role

I led the project from start to finish, including planning, development, and deployment. I collaborated with team leads to understand the most common internal pain points, then designed a solution that balanced ease of use with technical flexibility.

I built the core front-end using Astro for fast performance and clean architecture. A custom React component was used to integrate the company’s shared Google Calendar, allowing users to view upcoming meetings and events without switching tools. I also handled the Google Drive API integration, giving the team direct access to shared folders and documents from within the portal. For documentation, I implemented Astro’s Starlight theme and structured content for easy navigation and long-term maintainability.

##### Process

The project began with a needs assessment, where I gathered feedback from various team members on their day-to-day challenges with finding internal resources. I wireframed an initial layout for the portal, focusing on clarity, speed, and easy access to core tools.

Once approved, I developed the project incrementally. First, I created the base layout in Astro and styled the UI using Tailwind CSS. I then built and tested the React-based calendar integration using Google’s Calendar API. For file access, I implemented a serverless function to securely pull data from Google Drive, and formatted it for easy browsing. Finally, I set up the documentation section using Astro Starlight and migrated internal docs into Markdown format with a clear sidebar structure.

##### Tech Stack

The portal was secured using Google OAuth, allowing only employees with a company email address to log in. This not only restricted access to internal users but also enabled smooth integration with services like Google Calendar and Drive. The project was built with the following technologies:

- Astro
- Javascript
- React
- Google APIs
- Astro Starlight (Documentation)

<details>
  <summary>Technical Details</summary>

- **Server-Side Rendering with Astro**: Unlike typical static Astro builds, this portal was configured for full server-side rendering (SSR). This ensured that all content was protected behind authentication, and no pages were statically exposed to unauthenticated users.

- **Google OAuth Integration**: The entire site is gated by Google OAuth 2.0, scoped to the company’s domain. Users must log in with a valid company email to access any content. Once authenticated, users are redirected to the dashboard and their Google profile avatar is displayed in the top-right corner alongside a logout button.

- **Dashboard UI**: The post-login landing page is a dashboard featuring interactive cards that route users to different internal resources. Sections include access to Google Drive, Developer Docs, Design Docs, Intern Docs, General Info, and Employee Contact Info.

- **Drive & Docs Pages**: The Google Drive page connects to the company’s shared folder via the Google Drive API, using secure access through OAuth credentials. Documentation pages (Dev, Design, Intern) are organized and served using Astro Starlight, allowing for structured, searchable content written in Markdown.

</details>

<details>
  <summary>Challenges & Lessons Learned</summary>

- **Balancing SSR with Astro’s Static Defaults**: Configuring Astro for full server-side rendering required a shift from its default static-first mindset. Ensuring that dynamic routes were protected and authenticated properly involved digging into custom middleware and fine-tuning server behavior — a great learning experience in adapting frameworks beyond their defaults.

- **OAuth Flow and Session Management**: Implementing Google OAuth across the entire app introduced complexity in managing user sessions, redirects, and route protection. It deepened my understanding of authentication flows and secure session handling in a server-rendered context.

- **Google API Permissions**: Working with the Calendar and Drive APIs meant navigating OAuth scopes, service account access, and rate limits. I gained hands-on experience handling API credentials securely and ensuring consistent access without exposing sensitive data.

- **Scalable Structure for Internal Docs**: Creating a documentation system that was easy for non-devs to update and navigate required careful planning. Using Astro Starlight taught me the value of investing in structured content early on, especially when knowledge sharing is a key part of the platform’s purpose.

- **User Experience Considerations**: Because this was a tool employees would use daily, I focused heavily on simplicity and ease of navigation. Iterating on the dashboard layout and visual hierarchy helped reinforce how even internal tools benefit from thoughtful UX.

</details>
