# opremodeling.com — OnPoint Pros Remodeling LLC

Bathroom-remodeling brand site (the "discovery" half of the two-brand strategy:
`OnPoint Pros` at onpointprostx.com = branded-search asset + wide services;
**OnPoint Pros Remodeling** = bathroom-remodel discovery, pairs with the
"OnPoint Pros Remodeling" GBP profile).

Static site, same stack as onpoint-landing (GitHub Pages + Cloudflare).

## Deploy checklist (not yet done)
1. Create GitHub repo (`gh repo create opremodeling --public --source . --push`)
2. GitHub Pages: deploy from `main` branch root — CNAME file already present
3. Cloudflare: add opremodeling.com zone, CNAME → `<user>.github.io`, proxy on
4. Buy/point domain opremodeling.com
5. Google Search Console: verify domain property, submit sitemap.xml
6. Link the "OnPoint Pros Remodeling" GBP profile's website field → https://opremodeling.com

## Decisions still open (flagged 2026-07-12)
- **Phone**: RESOLVED 2026-07-12 — dedicated brand number (214) 888-8758
  everywhere (nav, hero, quick-answer, closer, footer, schema, llms.txt).
  Use this same number on the "OnPoint Pros Remodeling" GBP profile for NAP match.
- **Lead form**: v1 is call-CTA only. To add a form, reuse the GHL webhook pattern
  from ~/dev/bathroom-offer.
- Pricing bands come from real quote data (74 quotes, see onpoint-followup skill
  learnings) — keep honest, update when the data moves.

## Content rules (same as onpoint-landing)
No fabricated claims/counts, no review/aggregateRating JSON-LD (GSC penalty),
real reviews only (currently 2 real quotes from the family GBP profile, labeled
as such), single H1, canonical + quick-answer block for GEO.
