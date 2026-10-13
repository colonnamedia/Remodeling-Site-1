# FireWorks Project Handoff — Residential Remodeling Template

## Product snapshot

| Field | Value |
|---|---|
| Demo brand | Foundry & Frame Remodeling — fictional sample |
| Industry | Residential remodeling / general contracting |
| Demo market | Pittsburgh-area structure; every location is marked sample |
| Repository | `colonnamedia/Remodeling-Site-1` |
| Production preview | `https://remodeling-site-1.vercel.app` |
| Storefront status | Intended: Featured + Available on Home and Website Collection |
| Build price | **$2,499 one-time** |
| Hosting | **Standard: $499/year primary** or $59.99/month |
| Domain | **$20/year** |
| Search status | `noindex, nofollow`; robots disallows crawling until a real client is verified |

## Why this is a separate template

The current FireWorks catalog had construction-adjacent Landscaping and Roofing templates but no remodeling product. This template reuses their reliable static build, service-area, gallery-safety, local validation, and handoff patterns. It is not a cosmetic duplicate: remodeling needs room-specific education, broader project coordination, budget/timeline qualification, privacy-conscious photos, a permissioned before/after system, and a consultation provider gate.

## Pages and routes

| Route | Purpose | Primary CTA |
|---|---|---|
| `/` | Craftsman-led overview and service entry points | Start a Project Estimate |
| `/kitchens` | Kitchen planning, scope, and coordination | Plan a Kitchen Project |
| `/bathrooms` | Bathroom planning, systems, and accessibility | Plan a Bathroom Project |
| `/projects` | Whole-home service page plus honest gallery framework | Preview Whole-Home Intake |
| `/process` | Six-stage sample workflow and expectation-setting | Start the Demo Intake |
| `/service-areas` | Legitimate grouped local coverage structure | Preview Location Intake |
| `/estimate` | Full project qualification demo | Validate Demo Request |

## Reusable sections

- Original craftsman hero with desktop copy space and mobile-safe subject crop
- Room-specific service cards and detailed scope maps
- Four-step homepage process and six-step process page
- Whole-home/connected-space scope grid
- Concept gallery with explicit non-project labels
- Permissioned project-record and matching before/after placeholders
- Grouped service-area hub with verification language
- Estimate intake, local image preview, provider gate, CTA panel, responsive header/footer
- WebSite, Service, CollectionPage, HowTo, ContactPage, canonical, Open Graph, Twitter, sitemap, and demo robots scaffolding

## Estimate form fields and behavior

Fields: first/last name, email, phone, project type, municipality or ZIP, budget range, timeline, one-or-more priorities, 30-character project scope, up to four optional JPG/PNG/WebP images under 6 MB, consultation preference, contact window, and a honeypot.

The JavaScript validates locally and creates temporary browser object URLs for image previews. It explicitly does **not** send or store the inquiry, upload images, book a consultation, send a message, create a CRM record, or take payment. A selected consultation type changes explanatory text only.

## Supported and proposed integrations

No production integration is active in the master template.

| Integration | Status | Launch requirement |
|---|---|---|
| Vercel static hosting | Supported | Project connection and successful production build |
| Form email/CRM | Proposed | Client-selected provider, credentials, field mapping, spam control, consent/privacy, delivery/error testing |
| Scheduling | Proposed | Client-selected provider, real availability rules, service-area/fit gate, confirmations, cancellation behavior, end-to-end testing |
| Photo upload/storage | Proposed | Approved storage provider, access rules, file scanning/limits, privacy notice, retention/deletion policy, upload/error testing |
| Analytics/tag manager | Proposed | Client accounts, consent requirements, conversion definitions, test events |
| Payments | Out of scope | Separate approval and secure provider implementation; never implied by the demo |

## Required client inputs

Legal/display business name; logo and colors; verified phone, email, hours, service territory, credentials, insurance/license wording where applicable, actual services and exclusions, project minimums, consultation policy, scheduling process, design/trade relationships, permits/engineering responsibilities, contract/change-order/warranty language, permissioned project photos, photo credits and releases, verified project narratives, real testimonials with approval, privacy policy, lead destination, provider credentials supplied securely, and final domain.

## Price rationale

The $2,499 build price covers seven responsive pages, three original optimized image assets plus storefront crop, room-specific conversion copy, editable local SEO metadata/schema, a permissioned gallery and before/after framework, a detailed conditional project intake, client-side photo preview, and an integration safety gate. It exceeds the $999 minimum because it requires substantially more page, form, content, and QA work than a simple lead-generation site.

Hosting is separate and not discounted: Standard $499/year primary or $59.99/month. Domain is $20/year. Small Business ($299/year or $39.99/month) and Advanced (from $899/year or $99.99/month) remain catalog options but Standard is the appropriate default for this static multi-page template.

## Optional add-ons — priced separately

- Form-to-email or basic CRM connection: from $349 plus provider fees
- Scheduling connection with fit/service-area gate: from $349 plus provider fees
- Secure project-photo upload/storage: from $299 plus provider/storage fees
- Real project gallery onboarding: $125 per project record; five-project package $499
- Additional verified service-area page: $199 each
- Copy migration or case-study writing: scoped after source review
- Analytics and conversion configuration: from $249
- Advanced integrations or client portal: custom quote; likely Advanced hosting

Hosting, domains, integrations, third-party fees, and add-ons are not discounted.

## Verification checklist

- `npm run check`: validates seven pages, metadata, JSON-LD, one H1, alt text, demo robots, prohibited claims, required assets, estimate fields, provider gate, and gallery framework.
- `npm run build`: creates static `dist/` and copies optimized local assets.
- Browser QA: desktop and mobile navigation, every route, hero crops, project images, form validation, photo selection, provider gate, and no horizontal overflow.
- Deployment QA: production routes, asset responses, security headers, clean URLs, storefront demo URL/image, Featured/Available status, and complete checkout pricing.

## Publication record — 2026-10-13

- Template source commits: `ac24f734462f4d146e08095a4292840b427f9dba` (site source) and `e735b65b97f3cdb9946b7ee2cbbaa179c77015b6` (original optimized imagery).
- FireWorks storefront commit: `192dc5db97017b94694e9372666f71611ff1837a`.
- Vercel production URL verified: `https://remodeling-site-1.vercel.app/`.
- All seven production routes returned the expected unique title and single H1; every referenced image reported a nonzero natural width; desktop pages reported no horizontal overflow.
- The live form preselected Kitchen from the query string, exposed ten initially invalid controls, updated the in-home consultation provider gate, and completed with the explicit local-only no-send/no-upload/no-store/no-book/no-payment status.
- FireWorks Website Collection verified the 1200×630 storefront image, Residential Remodeling category, Featured and Available badges, $2,499 build, $499/year or $59.99/month Standard hosting, $20/year domain, live demo, feature list, and separate add-on copy.
- FireWorks Home verified the same Featured and Available card, image source, category, and pricing.
- Store Checkout verified $2,499 one-time, annual hosting selected at $499/year, $59.99/month alternative, $20/year domain, $3,018 due today before optional add-ons, and separately priced catalog add-ons.
- Responsive behavior is implemented at 900px and 620px with mobile navigation, one-column form/layout changes, hero subject crop, and stacked CTA/footer rules. The available cloud browser did not expose a narrow viewport control, so a direct 390px production screenshot remains the only visual QA item to repeat during the next customer customization.

## Future design variants

1. **Architect-led:** lighter editorial system, drawings/material palettes, design-service emphasis.
2. **Craft-forward:** darker woodshop palette, millwork and hand-detail imagery.
3. **Family-home:** brighter photography, occupied spaces, phased-renovation education.
4. **Accessible living:** universal-design content, verified credentials, and accessibility planning prompts.

Never publish a future variant with generated concept images presented as the contractor's completed work.
