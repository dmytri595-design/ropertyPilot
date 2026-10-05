# API Contract

PropertyPilot keeps external capabilities behind explicit adapter contracts.

## AI
```
PropertyPilotAdapters.ai.generateListing(property, brand, template)
PropertyPilotAdapters.ai.generateSeo(property, brand)
PropertyPilotAdapters.ai.generateSocial(property, brand)
PropertyPilotAdapters.ai.generateEmail(property, brand)
PropertyPilotAdapters.ai.translate(text, language, context)
PropertyPilotAdapters.ai.analyzeImages(property)
```

The current implementations are local/demo adapters.

## Other adapters
```
storage.saveProperty(property)
storage.saveImage(image)
storage.saveContent(content)
email.send(message)
auth.login(credentials)
db.query(request)
db.save(entity)
crm.push(payload)
```

## Production boundary
```
Browser → Secure Backend API → Provider Adapter
                         ↘ Database / Storage / Audit Log
```

The browser must never contain provider API keys.

## Error contract
Production adapters should return:
- code
- message
- retryable
- requestId
- safe user-facing detail

Do not expose stack traces, provider secrets or cross-tenant data.
