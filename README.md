# PropertyPilot — AI Real Estate Listing Engine

PropertyPilot is a working browser-first SaaS MVP for real estate agents and agencies. One property record powers a complete marketing package: title, listing description, SEO copy, Facebook ad, Instagram caption, short listing, buyer email, social caption, translations and key highlights.

## Product
**Positioning:** Working SaaS prototype with production-ready integration architecture.
**Demo user:** Jordan — fictional Demo Administrator. The actual owner/developer is Dmitry.
**Demo disclosure:** All seeded properties, agencies, contacts, prices and addresses are fictional. AI generation, image analysis and translation use local/mock adapters. No provider API key is required.

## Core workflow
Dashboard → Create Property → Upload Photos → Enter Facts → Generate Marketing Package → Review & Edit → Translate → Copy / Print / Export → Published / Archived.

## Implemented
- Dashboard with property KPIs and recent activity
- Property creation form with photo previews
- Property database with search and status filtering
- Property detail page with photo gallery
- Eight major generated content formats plus key highlights
- Editable outputs with copy/regenerate
- Mock/local AI generation and translation adapters
- Seven-language translation workspace
- Reusable templates
- Brand Voice settings
- Analytics based on actual prototype state
- JSON export/import
- Browser persistence and invalid-data recovery
- Print / Save as PDF marketing package
- Integration map and adapter contracts
- Responsive SaaS UI
- GitHub Actions validation and GitHub Pages workflow
- Cover artwork and acquisition documentation

## Technology
HTML5, CSS3, Vanilla JavaScript, LocalStorage, GitHub Actions, GitHub Pages. No frontend framework or runtime dependency.

## Local development
```bash
python -m http.server 8080
```
Then open http://localhost:8080/.

## Integration architecture
```text
PropertyPilot UI
  ├─ PropertyPilotAdapters.ai.generateListing(...)
  ├─ PropertyPilotAdapters.ai.generateSeo(...)
  ├─ PropertyPilotAdapters.ai.generateSocial(...)
  ├─ PropertyPilotAdapters.ai.generateEmail(...)
  ├─ PropertyPilotAdapters.ai.translate(...)
  ├─ PropertyPilotAdapters.ai.analyzeImages(...)
  ├─ storage
  ├─ email
  ├─ auth
  ├─ db
  └─ crm
```

Production target:
Browser → Secure Backend API → AI / Vision / Translation providers → PostgreSQL / object storage → Email / CRM / Property portals.

Never put provider secrets in the static frontend.

## Production boundaries
**Implemented now:** UI, property workflow, content generation workflow, editable outputs, local persistence, templates, analytics, export, responsive design and integration architecture.
**Ready for buyer integration:** real AI, image analysis, translation provider, authentication, database, image storage, email, CRM, property portal integrations, monitoring, billing and enterprise security controls.

## Acquisition
Indicative asking price: **USD 5,000 one-time**.
Suggested milestones: **40% / 30% / 20% / 10%**.
Buyer receives the source, repository, application, documentation, UI assets, demo data and integration contracts, subject to the final agreement and third-party/open-source exclusions.

## Public demo
After GitHub Pages is enabled:
https://dmytri595-design.github.io/ropertyPilot/

## Repository note
The repository was created as `ropertyPilot` with the initial P omitted. The product inside is branded **PropertyPilot**. This README documents the actual repository name.
