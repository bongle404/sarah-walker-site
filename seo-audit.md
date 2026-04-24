# Dr Sarah Walker — SEO Audit & Optimisation Plan
*Date: 2026-03-15 | Compiled from Brave SERP data, Firecrawl site audit, AI visibility analysis, local SEO research*
*Note: No DataForSEO volume data — balance insufficient. All rankings confirmed via live Brave Search.*

---

## Executive Summary

Dr Walker has one meaningful organic ranking — position 5 for "ISTDP therapy Gold Coast" — and is invisible everywhere else. The new site is structurally 10x better than her current one, but launching it without content and schema work will only marginally improve her position. ISTDP is a niche with low competition and official directory dominance, and trauma psychology in Gold Coast is winnable with a single well-structured page. The path to a full practice is content + local signals, not a better website alone.

---

## Current Rankings (Confirmed via Brave Search)

| Keyword | Current Rank | Ranking Page |
|---------|-------------|--------------|
| ISTDP therapy Gold Coast | **#5** | /about-drwalker/ |
| ISTDP therapist near me Australia | **#1 (via directory)** | Listed on istdp.com.au |
| Clinical psychologist Gold Coast | Not ranking | — |
| Psychologist Robina Gold Coast | Not ranking | — |
| Trauma therapy Gold Coast | Not ranking | — |
| Complex trauma psychologist Gold Coast | Not ranking | — |
| Clinical supervision psychologist QLD | Not ranking | — |
| Medicare psychologist Gold Coast | Not ranking | — |

---

## Key Competitors

| Domain | Strength | Keywords They Own |
|--------|----------|-------------------|
| goldcoastpsychologycentre.com.au | #1 for all generic Gold Coast terms | Clinical psychologist GC, Robina |
| goldcoastpsychologists.com | Trauma specialist hub | Trauma, complex trauma, PTSD Gold Coast |
| redmangallpsychologists.com.au | Multi-location, location-specific pages | Robina, generic GC |
| kategreenhalgh.com.au | Solo practitioner SEO done well | Robina psychologist, Medicare |
| robinatherapy.com.au | ISTDP-specific page (same clinic as Sarah) | ISTDP Gold Coast, ISTDP therapy |
| istdp.com.au | Official directory | All ISTDP national terms |

**Critical:** robinatherapy.com.au (where Sarah practices) ranks ahead of her own domain for ISTDP Gold Coast. Her practice is outranking her personal site.

---

## Current Site vs. New Site

| Element | drsarah-walker.com | sarah-walker-site.vercel.app |
|---------|-------------------|------------------------------|
| Page title | "Home - Dr Sarah Walker" | "Dr Sarah Walker \| Senior Psychologist \| Gold Coast" ✅ |
| H1 tag | **Missing** 🔴 | Present ✅ |
| Homepage word count | ~300 words 🔴 | ~3,500 words ✅ |
| Meta description | Generic ⚠️ | Keyword-specific ✅ |
| FAQ section | None 🔴 | 8 questions ✅ |
| Testimonials | None | 3 present ✅ |
| Services page | **404 error** 🔴 | Complete ✅ |
| GP referral info | None | Detailed section ✅ |
| AI crawler access | Fully open ✅ | Needs verification |
| Schema markup | OG tags only 🔴 | Not yet added 🔴 |
| Blog/content hub | None 🔴 | None 🔴 |
| Local business schema | None 🔴 | None 🔴 |

---

## What Must Be Added Before Launch

### 1. Schema Markup

**Physician / LocalBusiness schema** — add to `<head>` of index.html:
```json
{
  "@context": "https://schema.org",
  "@type": ["Physician", "LocalBusiness"],
  "name": "Dr Sarah Walker",
  "description": "Clinical psychologist specialising in ISTDP, complex trauma, and eating disorders. Robina, Gold Coast.",
  "url": "https://drsarah-walker.com",
  "telephone": "07 5575 8855",
  "address": {
    "@type": "PostalAddress",
    "streetAddress": "Suite 4, 249 Scottsdale Drive",
    "addressLocality": "Robina",
    "addressRegion": "QLD",
    "postalCode": "4226",
    "addressCountry": "AU"
  },
  "hasCredential": ["MPsych(Clin)", "DPsych(Clin)", "ISTDP Accredited Therapist"],
  "medicalSpecialty": ["Psychiatry", "Psychology"]
}
```

**FAQPage schema** — unlocks Google rich results. Map each FAQ from the existing accordion:
```json
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "[FAQ question text]",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "[FAQ answer text]"
      }
    }
  ]
}
```

### 2. AI Crawler Access
Confirm new site's robots.txt does not block: GPTBot, PerplexityBot, ClaudeBot, anthropic-ai, Bingbot.
Current site has a clean open robots.txt — new site should match.

### 3. Dedicated Service Pages (separate URLs)
Every competitor with a ranking niche uses a dedicated URL. robinatherapy.com.au/istdp appears in 4 of 5 ISTDP searches because of this. The new site has inline sections but no `/istdp/`, `/trauma/`, `/supervision/` pages.

---

## Content Priority — 4 Pages That Will Move Rankings

| Page | Target Keywords | Word Count | Est. Ranking Timeline |
|------|----------------|------------|----------------------|
| `/istdp/` | "ISTDP therapy Gold Coast", "what is ISTDP Australia" | 1,500 | 3–4 months |
| `/complex-trauma/` | "complex trauma psychologist Gold Coast", "trauma therapy Gold Coast" | 1,200 | 3–5 months |
| `/clinical-supervision/` | "clinical supervision psychologist Queensland" | 900 | 4–6 months |
| Blog: "What to expect from ISTDP" | Long-tail + AI citation | 1,200 | Ongoing |

Each page needs:
- Question-format H2 headings (better AI extraction)
- Statistics or outcome data with cited sources (+40% AI citation rate)
- FAQ block at bottom (maps to FAQPage schema)
- Internal link to booking page

---

## Local SEO Checklist

| Action | Status | Priority |
|--------|--------|----------|
| Google Business Profile — claim and verify (Robina) | Unknown — likely not optimised | 🔴 High |
| GBP categories: "Clinical Psychologist" + "Psychologist" | Unknown | 🔴 High |
| Google reviews (target 15+, competitors have 20–40+) | Unknown | 🔴 High |
| ISTDP Australia directory — confirm link points to new site | ✅ Listed | ⚠️ Verify link |
| HealthShare listing | ✅ Confirmed | ⚠️ Check completeness |
| Psychology Today Australia | Not confirmed | 🟡 Medium |
| APS Find a Psychologist | Not confirmed | 🟡 Medium |
| Healthdirect listing | Unknown | 🟡 Medium |

---

## AI Search Visibility

She is cited via her ISTDP Australia directory listing, not from her own content. Her site isn't yet rich enough to be extracted by AI engines directly.

**What creates citations (based on what's ranking):**
1. Long-form educational content with clinical detail (robinatherapy.com.au/istdp ranks in 4/5 ISTDP searches)
2. Directory authority backlinks (istdp.com.au citing her is a strong signal)
3. FAQPage schema
4. Question-format H2 headings on service pages

The ISTDP explainer page is the single best AI visibility investment.

---

## 90-Day Action Plan

### Month 1 — Foundation (before/at launch)
- [ ] Add Physician + LocalBusiness schema to index.html
- [ ] Add FAQPage schema to index.html
- [ ] Verify robots.txt allows all AI crawlers
- [ ] Launch new site (migrate drsarah-walker.com domain)
- [ ] Claim and fully complete Google Business Profile (Robina)
- [ ] Verify ISTDP Australia directory listing links to new domain

### Month 2 — Content that moves rankings
- [ ] Publish `/istdp/` page (1,500 words, FAQ block, schema)
- [ ] Publish `/complex-trauma/` page (1,200 words, FAQ block)
- [ ] Submit both pages via Google Search Console

### Month 3 — Fill remaining gaps
- [ ] Publish `/clinical-supervision/` page (900 words)
- [ ] Publish first blog post ("What to expect in your first ISTDP session")
- [ ] List on Psychology Today Australia + APS Find a Psychologist
- [ ] Begin requesting Google reviews from existing clients

### Ongoing
- One long-form article per month targeting a condition keyword (eating disorders, personality disorders, medically unexplained symptoms)
- Monitor and maintain ISTDP Australia directory listing
