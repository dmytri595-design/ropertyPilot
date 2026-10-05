# Live Deployment

## GitHub Pages
The repository contains a GitHub Actions Pages workflow using:
- actions/checkout
- actions/configure-pages
- actions/upload-pages-artifact
- actions/deploy-pages

Repository setting required:
Settings → Pages → Build and deployment → Source → GitHub Actions

Expected project URL:
https://dmytri595-design.github.io/ropertyPilot/

## Static deployment boundary
The public build is a browser-first prototype. Real AI credentials, customer data, authentication, database access, cloud object storage, billing and CRM/property portal credentials must remain server-side in production.

## Alternative
The repository can also be imported into Vercel as a static site with no build command and . as the output directory.
