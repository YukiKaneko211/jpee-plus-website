# JPEE+ Official Website

The official website for the **JPEE+ Project**, cultivating grassroots connections between Japan and Europe, based in Estonia.

- **Project Status:** On-going
- **Live Site:** [https://jpee-plus.com/](https://jpee-plus.com/)
- **Original Repository:** [jpee-pub/website](https://github.com/jpee-pub/website)
- **My Project Role:** Lead Frontend Developer, UI/UX Designer & Brand Asset Creator

---

## Project Context & Credit

> [!NOTE]
> This repository is a personal fork of the original [JPEE+ Official Website Repository](https://github.com/jpee-pub/website) managed by the [JPEE+ project account](https://github.com/jpee-pub). It is showcased here to highlight my skillset, role, and responsibilities within the JPEE+ team.

I lead the ongoing frontend & UI/UX development, brand asset creation, and site maintenance for the official JPEE+ website under the direction of [Maria Nawatani](https://www.linkedin.com/in/maria-nawatani-a264337b/) of OÜ Roua, the organization behind the JPEE+ project.

Since the project team includes non-technical and non-designer members, I am responsible for designing visual content, maintaining site updates, and managing web infrastructure.

## Design Strategy & Visual Identity

Combining my background in design with frontend engineering, I planned the project implementation with a focus on speed-to-market and iterative growth:

### Phase 1: Speed-First Execution & Continuous Iteration (Current)
- **Minimum Viable Launch:** As discussed below, the visual ideas for the site were more diverse, but in this phase, I prioritized the release of an official project site with the necessary information and minimum appearance to maintain the credibility of the project.
- **AI-Assisted Design & Refinement:** 
  - Generated an initial layout draft in Figma using AI prompts to establish a quick structural baseline ("modern, professional corporate site without being overly formal").
  - Refined and customized the AI output into more natural and engaging design suited for public release using official brand assets.
- **Brand Identity & Logo:** Designed the official JPEE+ logo
  - using a primary color palette derived from the flags of the EU and Japan to build a consistent visual identity.
  - motif like starts and sakura petals are inspired by EU flag and Japanese culture.
  - snows and swallow design comes from our project foundation in Estonia.
  <img height="100" alt="jpee+_logo_tra" src="https://github.com/user-attachments/assets/45c71265-532e-44a2-bb95-338088ebbeb6" />
- **Content Expansion:** Regularly introduced dedicated sub-pages such as [eesti-portal](https://jpee-plus.com/eesti-portal) and [JPEE+ Lab](https://jpee-plus.com/jpee-plus-lab) while maintaining quick release cycles.
- **Dynamic Content Integration & Troubleshooting:**
  - Expanded the workflow from early AI prompt-assisted coding to leveraging IDE-integrated tools (Cursor).
  - Implemented a dynamic "Latest News" section that automatically fetches and renders recent content from our [YouTube channel](https://www.youtube.com/@jpee-plus) and [Note account](https://note.com/jpee_plus) via `rss2json`.
  - Resolved production-only routing and fetch issues by correctly configuring static asset routing priorities in `netlify.toml` and `public/_redirects`.

### Phase 2: Scalability & Mascot Integration (Planned)
- **Brand Mascots:** Planning the integration of modern, pop-culture-inspired mascots to symbolize our bridge between Japan and Europe.
  - **Human-style character:** Represents both online and real-world connection with a futuristic design using our brand colors.
  <img height="200" alt="Illustration6 2 (1)" src="https://github.com/user-attachments/assets/99b2d059-687a-40f5-a97d-37d6b3216d04" />
  
  - **Chibi/Mini character:** Features a Nordic motif inspired by our foundation in Estonia.

  <img height="200" alt="J_front" src="https://github.com/user-attachments/assets/c4473253-412e-40f7-b7d6-45b06feb0c67" />
- To avoid delaying the initial site launch, mascot creation was scheduled for Phase 2 while the core platform was released first.

## Technical Stack & Infrastructure

- **Framework:** React
- **Language:** TypeScript
- **Styling:** Tailwind CSS
- **Design & Graphic Tools:** Figma, Adobe Express, Affinity, Clip Studio Paint EX
- **Hosting & Infrastructure:** Netlify (Automated CI/CD via `main` branch), Cloudflare (DNS, CDN, Routing)
- **Email Operations:** Cloudflare Email Routing + Gmail Alias (`contact@jpee-plus.com`)

Beyond frontend development, I configured and managed the full platform infrastructure:

- **DNS & CDN Management (Cloudflare):** Managed domain configuration (`jpee-plus.com`), routing rules, and caching optimization for static pages on top of the Netlify host.
- **Custom Domain Email Setup:** Configured Cloudflare Email Routing with Gmail SMTP aliases, enabling professional inbound and outbound communication for `contact@jpee-plus.com` without added infrastructure costs.

---

## Development Workflow & Branch Strategy

Because cross-functional collaboration with non-developer team members takes place on Asana and Discord, GitHub is primarily utilized for version control, automated deployments, and code stability.

- **Netlify CI/CD Integration:** Merges to the `main` branch automatically trigger production builds and deployments via Netlify.
- **Branching Model:** Feature updates and experimental builds are tested in separate branches before being merged into `main`.
