# Precision Home Solutions — Project State

Recovered from the original Claude Code desktop session (2026-10-03/04). This file is the
source of truth for picking the work back up in a new session. Keep it updated as pages ship.

## Business facts (approved)

- **Business:** Precision Home Solutions — veteran-owned residential improvement & remodeling contractor
- **Contact:** Branden Skorcz · 256-617-8718 (`tel:+12566178718`) · branden@precisionhomesal.com
- **Domain:** PrecisionHomesAL.com
- **Facebook (only social):** https://www.facebook.com/profile.php?id=100091217414624
- **Service area:** Huntsville, Madison, Athens, Madison County, and surrounding North Alabama communities
- **Trust statements:** Veteran Owned & Operated · Licensed & Insured · 26+ Years of Experience
  (experience is NOT the company's age; no founding date)
- **Tagline (exact):** QUALITY WORK. HONEST SERVICE. LASTING RESULTS.
- **Estimates:** free within normal service area; delivered as a digital document with a cost breakdown
- **Payment:** typically 50% before work / 50% on completion (may vary with scope); cash, check,
  credit/debit, Venmo, Cash App, Zelle
- **Fences:** wood only — wood privacy, wood-and-wire farm fence, wood gates. **No chain-link.**
- **HOA:** handles HOA approvals for fence projects
- **Decks:** pressure washes decks

### Never invent
Reviews, ratings, project counts, pricing, turnaround times, financing, warranties, street address,
map pin, business hours, other social accounts, staff details, certifications.

## Brand / design

- Navy (structure, primary text, dark sections), white/off-white (content), muted gold (CTAs, icons, accents)
- Distinctive heading font + simple body font; generous spacing; restrained motion; respect reduced-motion
- Dark-section outline buttons: translucent fill, white border/text, solid white + navy text on hover
- Reference direction: ELM Construction (primary), H&C Design-Build, Sun Design Remodeling,
  McDonald Remodeling, Murray Lampert — inspiration only, no copying

## Copy brief for service pages (reuse every time)

Sabri Suby / Dan Kennedy–style conversion copy aimed at real homeowner fears (will they show up,
will they upsell me, will they actually fix it, will they overcharge, is it safe, regret picking the
wrong company). Plain, conversational, average reading level. Question-style H2/H3s; first sentence
under each heading answers the question on its own (AI Overview / Gemini extraction). State services,
who they're for, where, problems solved, and limitations. Cities only in hero, Service Area, and one
FAQ — do not repeat geo in every paragraph. No keyword stuffing. Claim only what photos/Branden confirm.

Standard service-page structure: Hero (H1, CTA + call) → trust strip → "Before You Hire Anyone"
(fear-busting list, first item = free itemized digital estimate) → service sections with real photos /
before-after pairs → Service Area → FAQ → "Tell Us About Your Project" estimate form → global footer.

## Platform: Divi 4.27.9 on SiteGround staging

Staging: https://davids1258.sg-host.com · Royal MCP endpoint: `https://davids1258.sg-host.com/wp-json/royal-mcp/v1/mcp`
(cloud sessions need `davids1258.sg-host.com` in the environment's allowed domains, plus Royal MCP added as a connector).

Built via the **Royal MCP** WordPress plugin (OAuth/API key; key was posted in chat — **rotate it**).
Royal MCP cannot write Divi page settings, CF7 form settings, Rank Math settings, or install plugins.

| Page | WP ID | Status | Focus keyword | Planned slug |
|---|---|---|---|---|
| Home | 11 | draft | — | (front page) |
| Fence & Deck | 54 | draft | fence company Huntsville AL | /fence-company-huntsville-al/ |
| Bathroom Remodeling | 64 | draft | bathroom remodeling Huntsville AL | /bathroom-remodeling-huntsville-al/ |
| Kitchen Remodeling | 84 | draft | kitchen remodeling Huntsville AL | /kitchen-remodeling-huntsville-al/ |
| Property Maintenance | 106 | draft | property maintenance Huntsville AL | /property-maintenance-huntsville-al/ |

Other staging objects:
- Divi Library: PHS Global Header (32), PHS Global Footer (33) — assigned in Theme Builder ✅
- CF7 form "Free Estimate Request" (42) — 9 fields + 3 photo uploads ✅
- Primary Menu: Home, Services, About, Service Area, Contact (section anchors)
- Brand CSS lives in Appearance → Customize → Additional CSS (~17 KB, scoped)
- Home: Featured Work + Reviews sections are **disabled** until real content exists
- Media IDs: bathroom 57–62, 73 · kitchen ~75–83 · maintenance 93–105

## Workflow decision

All pages stay **draft** until every page is built; the owner then edits them in Divi before publishing.
Once a page has been hand-edited, never regenerate/overwrite its full layout — read the live content
first and make targeted edits only.

## Remaining pages

1. Painting (incl. drywall, popcorn ceiling removal) — **needs photos**
2. Pressure Washing — **needs photos**
3. Home Remodeling (attic-to-office conversion, wood accent wall, laundry cabinets, hot tub pad,
   fire pit cleanup photos already set aside for this)
4. About, Contact, Our Work/portfolio (later phase)
5. After publishing: link Home service cards + menu to service pages; enable Featured Work

## Open setup (wp-admin, manual)

- [ ] CF7 Mail tab: To = branden@precisionhomesal.com (remove david@… after testing);
      File attachments = `[project-photo-1]` `[project-photo-2]` `[project-photo-3]`
- [ ] CF7 Messages tab: paste custom messages (from CF7-PASTE.md — needs recovery from the Mac)
- [ ] Rank Math → Titles & Meta → Local SEO → Email = branden@precisionhomesal.com
- [ ] SMTP plugin on precisionhomesal.com + spam protection (Turnstile/reCAPTCHA/Akismet)
- [ ] Real test submission with photo attached
- [ ] Replace About placeholder photo with real owner/crew photo
- [ ] Check slugs, publish, set Home as front page (Settings → Reading)
- [ ] Rotate Royal MCP key

## Open questions for Branden

- Hidden-damage promise on Bathroom & Kitchen (customer sees it and approves changes before work continues)
- Shower/tub updates as part of bathroom work
- Kitchen: "most homeowners stay in the house"; does he replace sinks, not just reset them
- Maintenance: plumbing scope ("faucets, fixtures, small leaks"; refers bigger jobs to a licensed plumber),
  "repairs and replaces doors", pressure-washing surfaces, recessed lighting
- Confirm "Licensed & Insured" wording
- Brighter real shower/tub photo to replace stock Bathroom hero

## Source files from the original session (not yet in this repo)

These were in a temporary folder on the Mac and need to be copied here if they still exist:
`divi/build_layout.py`, `build_decks_fences.py`, `build_bathroom.py`, `build_kitchen.py`,
`build_maintenance.py`, `custom.css`, `DIVI-SETUP.md`, `CF7-PASTE.md`, `HANDOFF.md`,
`precision-home-solutions.zip` (block-theme version, superseded by Divi).
