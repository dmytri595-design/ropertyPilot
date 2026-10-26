# Production Checklist

## Backend
- [ ] Secure backend API
- [ ] PostgreSQL or equivalent
- [ ] Agency / tenant isolation
- [ ] RBAC
- [ ] Audit logs
- [ ] Background jobs for large generation requests
- [ ] Server-side rate limiting

## AI / Translation
- [ ] Preserve the selected listing purpose in all generated outputs
- [ ] Add factuality checks so sale/rent phrasing cannot contradict the property record
- [ ] Evaluate template behavior against human-reviewed sample listings
- [ ] Select provider(s)
- [ ] Server-side secret manager
- [ ] Prompt and model versioning
- [ ] Cost controls
- [ ] Factuality evaluation
- [ ] Human approval gates
- [ ] Vision model
- [ ] Production translation provider

## Media
- [ ] Confirm photo ownership / usage permission before publication
- [ ] Do not treat illustrative demo photo URLs as customer assets
- [ ] Secure object storage
- [ ] Image resize/transcoding
- [ ] Malware/content checks
- [ ] Signed URLs
- [ ] CDN strategy
- [ ] Photo ordering persistence

## Security / Privacy
- [ ] Real authentication
- [ ] Enterprise RBAC / SSO
- [ ] TLS
- [ ] Encryption at rest
- [ ] Secret management
- [ ] XSS/CSRF protections
- [ ] Backups and restore tests
- [ ] Privacy policy / DPA
- [ ] Data retention / deletion controls

## Integrations
- [ ] Email provider
- [ ] CRM
- [ ] Property portals
- [ ] Social publishing if required

## Commercial / Operations
- [ ] Define exactly what Published status means for each integration; local prototype status alone must not imply external publication
- [ ] Billing
- [ ] Usage metering
- [ ] Terms of service
- [ ] Monitoring
- [ ] Incident response

## Explicit non-claims
The prototype does not claim production authentication, live provider-backed AI, production image storage, real translation quality, connected portals, billing, enterprise SLA or validated marketing performance.
