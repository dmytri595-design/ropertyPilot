# Data Model

| Entity | Purpose | Prototype |
|---|---|---|
| User | Identity and role | Seeded demo |
| Agency | Tenant / real estate business | Settings-level demo |
| Property | Source property record | Implemented |
| PropertyImage | Photo metadata | Browser data |
| GeneratedContent | Generated/editable block | Embedded on Property |
| Translation | Localized output | Embedded on Property |
| Template | Generation structure | Implemented |
| BrandSettings | Brand voice / contact | Implemented |
| Publication | Publication status | Property status field |
| GenerationHistory | Generation/edit/translation events | Local |
| AnalyticsEvent | Product activity | Local |
| Document | Future supporting asset model | Planned |

Production Property fields:
id, agencyId, title, address, city, country, type, listingPurpose, price, currency, beds, baths, floorArea, lotArea, floor, yearBuilt, parking, furnished, condition, features, notes, contact, status, templateId, createdAt, updatedAt.

Production GeneratedContent should be normalized with id, propertyId, format, body, status, version, model, promptVersion, sourceFactHash, authorId, createdAt, updatedAt, approvedAt.

Every production record should carry a tenant boundary and use server-side authorization.

## Listing purpose and templates

The prototype supports `For Sale`, `For Rent`, `Short Stay`, and `Commercial Lease` as property-level listing purposes. The generation adapter uses that value to shape SEO copy, social wording, and email subject/body. Template IDs are `luxury`, `residential`, `rental`, `commercial`, `development`, `vacation`, and `investor`. These are local generation rules, not a live model prompt or proof of copy performance.
