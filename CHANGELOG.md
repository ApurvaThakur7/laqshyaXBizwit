# Laqshya × Bizwit AI — Proposal Changelog

Track every version and what changed. Add a new block at the top for each version.

---

## v3.0 — 19 Jul 2026 — Scope & effort framing

**Status:** Latest

- **R7 (Proof of Play & Client Portal) is now the only Code-Based module.** R13 Finance MIS changed to Hybrid, R14 HR Automation changed to Low-Code — architecture table rows and requirement card footers updated together.
- **Fixed pricing removed.** The "Investment" column is now **Relative Effort**, with bands by approach: Low-Code = ₹, Consulting = ₹, Hybrid = ₹₹, Code-Based = ₹₹₹. Same bands on all 14 requirement card footers; the ₹28,00,000 total row is gone.
- **Readability fix in the red challenges card.** The global `.red` text-colour utility was bleeding into the "Operations & Execution" column, turning its bold item titles red-on-red (invisible) and making rows look misaligned. Titles are now white and the arrows align with them.
- **Gradient accents (minimal).** The CTA's purple→pink→orange gradient now also appears on the scroll progress bar, the executive-summary stat numbers, and the pillar letters on hover.
- **Brand lockup redesigned.** "× BIZWIT AI" is now a 12px bold white sub-mark with a red ×, balanced under LAQSHYA in nav and footer.
- **Gradient extended.** Also on the hero word "System", section-heading accent words, hero stat numbers and approach mini-stats.
- **WhatsApp CTA.** "Book the discovery workshop" (mailto) replaced with "Let's begin →" opening Priyank's WhatsApp chat directly (+91 73764 05488), with the number linked below the button.
- **Self-serve pricing block.** All ₹ effort bands and the column/card label now come from one clearly-marked `PRICING` block at the top of the page script — editable in one place without touching the rest of the file.
- **Real module pricing added (excl. GST).** Label is now **Investment**: R1 ₹3L (Hybrid), R2 ₹1.5L, R3 ₹2L, R4 ₹50K (Consulting · 4 sessions, Change Mgmt removed), R5 ₹5L, R6 ₹1.5L, R7 ₹12L, R8 ₹1.8L (Low-Code), R9 ₹2.8L, R10 ₹2.2L, R11 ₹2.2L, R12 ₹5L (Code-Based), R13 not quoted (future), R14 ₹3.7L. GST note added inside the architecture table.
- **R5 rewritten as AI Calling & Media Intelligence** — AI agent calls media owners, builds the database, frontend ranks the best owners per location. Hybrid build.
- **R8 renamed Invoice Preparation** (Low-Code); **R12 now Code-Based**; approach mini-stat updated to 2 code modules.
- **R14 HR Automation is live scope** — two levels (resume screening + AI interview agent), marked Deployed, future tag now only on R13.
- **90-day delivery timeline** added to "How the engagement works", replacing the two-components line.
- **Visual fixes:** delivery phase numbers 01–08 now gradient (were invisible dark-on-dark); red commercials card heading now white (was red-on-red).
- **Legal line** added to the footer: prepared exclusively for Laqshya Media Group, for its consideration and acceptance; not a binding offer.

**Planned next (v4):**
- Proof-of-work gallery — clicking a Proof card opens its screenshots / recordings in a lightbox (assets pending).

---

## v2.0 — 18 Jul 2026 — Pricing & polish

**Status:** Superseded by v3.0

- Per-module investment added: every requirement card (R1–R14) now shows **Investment ₹2,00,000**.
- Architecture table gains an **Investment** column and a total row: **₹28,00,000 for 14 modules**.
- Nav bar gets a solid blurred background once scrolled, so the logo and links no longer merge with page content.
- Fixed the Next Steps button sitting lower than the other nav links (class collision with the bottom CTA section).

**Planned next (v3):**
- Proof-of-work gallery — clicking a Proof card opens its screenshots / recordings in a lightbox (assets pending).

---

## v1.0 — 18 Jul 2026 — First draft (for internal review)

**Status:** Superseded by v2.0

- Full rebuild in Laqshya's actual brand: black canvas, white bold Archivo type, signature red (#ED1C24), target-dot logo + reticle motif.
- All 14 requirements across 4 pillars (A Knowledge & Enablement, B Core Operations, C Growth & Creative, D Enterprise Expansion).
- Sections: hero, executive summary, business/verticals, campaign lifecycle, challenges, pillars, requirements A–D, architecture table, proof section, approach, delivery plan, commercials, next steps.
- Proof section maps Bizwit's already-built systems to each requirement.
- Cost-efficient hybrid framing; reference to Laqshya's existing SHARP planner.
- Real Laqshya stats (27 years, 17 offices, 350 people, 1000+ brands).
- Commercials shown as structure only, no figures.

**Open feedback / to decide:**
- Hero headline sizing (currently oversized for impact).
- Exact brand red hex (confirm against brand guide / Firecrawl).
- Whether to add ballpark commercial numbers.

---

<!-- ## v2.0 — [date] — [summary]
- change 1
- change 2
-->
