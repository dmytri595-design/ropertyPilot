# PropertyPilot — Buyer Brief

## Product in one sentence

PropertyPilot is a browser-first real-estate content workspace that turns one structured property record into a consistent set of listing, SEO, social, email, and highlight copy for an agent or agency to review and export.

## Why it may be relevant to an acquirer

The product offers a working front-end workflow and an extensible product foundation for a real-estate agency, proptech platform, listing portal, property CRM, or property-marketing agency. A buyer with an existing audience and distribution could adapt the workflow to its brand, connect production services, and test demand with its customer base.

The project is not presented as a business with proven traction. Its potential value is the implemented user journey, content-format coverage, editable output workflow, starter UI, and integration boundaries.

## What can be explored today

- Property portfolio with search and status filtering.
- Property creation from structured facts, local photo previews, and a fictional sample-property workflow.
- Sale, rent, short-stay, and commercial-lease purpose labels that shape SEO copy, email subject/body, social text, and hashtags.
- Seven selectable content templates: luxury, residential, rental, commercial, new development, vacation, and investor.
- Eight core marketing formats: title, full description, SEO copy, Facebook ad, Instagram caption, short listing, buyer email, and social caption; plus a separate key-highlights output.
- Editable text and structured social/email blocks, text export, copy helper, approval state, regeneration, and local activity history.
- Seven-language translation workspace with explicit mock-adapter disclosure.
- Local status tracking for Draft, Ready, Published, and Archived. A Published status is a local label only; no property portal is contacted.
- Settings for agency brand voice, templates, CTA, contact details, and currency.
- JSON workspace export/import and print / Save as PDF marketing package.
- Responsive UI, vanilla JavaScript, CSS, local persistence, and GitHub Pages deployment workflow.

## Assets

- **Demo:** https://dmytri595-design.github.io/ropertyPilot/
- **Repository:** https://github.com/dmytri595-design/ropertyPilot
- **README:** https://github.com/dmytri595-design/ropertyPilot#readme
- **Acquisition listing:** docs/ACQUISITION_LISTING.md
- **Product overview:** docs/PRODUCT_OVERVIEW.md
- **Integration contract:** docs/API_CONTRACT.md
- **Data model:** docs/DATA_MODEL.md
- **Production checklist:** docs/PRODUCTION_CHECKLIST.md

The repository name is literally `ropertyPilot` (the initial P is missing); the application is branded PropertyPilot.

## Current stage and limitations

PropertyPilot is a local-first prototype / pre-launch / pre-revenue. No customer, active-user, conversion, or revenue claims are made.

AI content generation, photo analysis, translation, database, storage, authentication, email, CRM, and portal integrations are local or mock adapter implementations. Generated copy is deterministic demo text, not a live AI inference. Translation output is not a production translation. The property workspace persists in the current browser's localStorage; photo previews are local browser processing and are not uploaded. The Published status is not connected to an external portal. Demo properties, people, contact details, prices, locations, and listing facts are fictional.

## Plausible buyer roadmap

1. Interview current users of the buyer's agency/portal product and define the actual target workflow.
2. Connect an authenticated backend, agency/tenant isolation, database, and private object storage.
3. Add a real model provider behind the server-side adapter, including cost controls, prompt/version management, and factuality evaluation.
4. Add reliable image upload, image licensing/consent checks, production translation, and document/media storage.
5. Add selected CRM, email, and property portal integrations, only where buyer demand justifies the effort.
6. Add auditability, access controls, billing if appropriate, monitoring, and customer support processes.

This is a suggested roadmap, not functionality included in the current prototype.

## Commercial context

The repository's acquisition copy proposes an initial seller asking price of **USD 5,000**, which is a seller-set negotiation position rather than an independent valuation. A deal should be priced against technical diligence, buyer fit, rights actually transferable, and the amount of production work the buyer expects to fund.

## IP, licensing, and media diligence

The repository contains a custom no-license notice rather than an open-source license. However, the project also references illustrative remote demo photos from third-party image URLs. Those image assets and their underlying rights should not be represented as included exclusive IP. Before a transaction, explicitly document the scope of source code, documentation, branding, domains, deployment assets, and any third-party media/licensing exclusions. An acquisition agreement should be reviewed by qualified counsel. Do not claim that the prototype itself has been legally audited.

## Best-fit buyer

The strongest fit is likely an existing real-estate SaaS, property CRM, listing portal, agency group, or property-marketing service that can integrate the workflow into an existing customer relationship rather than acquire the project solely on an unproven standalone growth thesis.
