# A4A Jobs To Be Done: Living Framework

A living, evidence-grounded map of **Automattic for Agencies (A4A)** as a hierarchy of Jobs To Be Done. Built in the Designomattic "Design Den" practice. The map is meant to stay alive: every time the product ships something new, the corresponding job gets added or updated.

**Live map:** https://automattic.github.io/a4a-jtbd/

## What this is

A4A is a relationship tool that helps agencies earn recurring revenue, run many client sites from one place, and grow their business. This project captures everything an agency can do in that product as a single, structured set of Jobs To Be Done, then renders it as an interactive map you can pan, zoom, search, and filter.

A Job To Be Done describes a real customer goal, free of any specific solution, using one formula: **when** [situation], **I want to** [motivation], **so I can** [outcome]. Framing the product this way keeps us focused on what the agency is actually trying to accomplish, so we can judge each feature and CTA by the job it serves.

## How the map is broken down

The map is organized along three dimensions, which are exactly the ones explained in the dashboard's **ⓘ Key** (bottom-left legend).

**Layers (the levels of the map, top-down):**

1. **Pillar (Layer 1):** the highest-level, durable jobs. Everything below rolls up to these.
2. **Function (Layer 2):** the major functional areas (Sites, Referrals, Migrations, and so on) that roll up to a pillar.
3. **Micro (Layer 3):** the granular, CTA-level tasks within a function (e.g., add an agency logo to a referral, remove a team member's access).

**Pillars (the high-level jobs an agency hires A4A for):**

- **Earn:** turn project work into predictable income that recurs on its own (commissions, revenue share, resale margins).
- **Build:** deliver and operate many client sites reliably from one place on infrastructure the agency trusts.
- **Grow:** win more of the right business and level up through qualified demand, credibility, and expertise.
- **Multi-pillar:** a job that meaningfully serves more than one pillar at once (e.g., onboarding spans all three).

**Job states and flags (badges on a card):**

- **Draft / Validated:** where a job sits on its path to being backed by evidence.
- **New user / Returning:** jobs for the first-run experience and jobs for the steady state.
- **Upcoming:** a feature that has not shipped yet (also drawn as a dashed, striped card).
- **Intermittent:** availability comes and goes, like a promo or incentive that turns on and off.
- **Redundant:** duplicates functionality elsewhere and is flagged for the consolidation pass (see the job's note).
- **Tier-gated:** available only to certain agency segments (e.g., Agency, Pro, Premier).

## Purpose

This map currently mirrors the **current experience 1:1** with the product: it captures every task a user can perform across the dashboard. That completeness is deliberate, but it is the starting point, not the goal.

The real goal is to **reduce and focus** the JTBD so we can streamline the product and the experience. A complete map makes overlap visible: when the same underlying job shows up in multiple places (e.g., "refer a product" living in Exclusive offers, Marketplace, and Referrals), the map should surface that duplication so we can consolidate it. Use the map to ask, for any cluster of jobs: which of these are truly distinct customer jobs, and which are the same job exposed in several spots that we could merge or remove? Mapping everything is how we find what to cut.

Concretely, the map helps us: spot overlapping / redundant jobs to consolidate; identify low-value or low-conversion jobs to de-emphasize or retire; and keep the team aligned on the smaller set of jobs that actually matter. The **Page** filter in the dashboard (and the planned low-conversion highlighting) exist to support exactly this kind of pruning.

## The model (this is the standard: don't deviate)

Three strict levels, top-down. **Nothing sits between them.**

1. **Pillars**: the three high-level jobs an agency hires A4A for: **Earn**, **Build**, **Grow**. One card each.
2. **Major functions**: the agency's jobs under each pillar (both conceptual jobs like "Predictable recurring income" and dashboard areas like "Agency Tier"). Many per pillar, sitting **side by side**. One card each.
3. **Micro functions**: the granular, usually CTA-level tasks within a major function (e.g., "Download your badges"). Many per function, each rolling up to its parent function.

Rules:
- Every micro rolls up to exactly one major function; every major function rolls up to one or more pillars.
- Major functions are **siblings, never stacked**.
- A job may map to more than one pillar (`pillar` is a list): shown as **Multi**.
- The primary user is the **agency**. The agency's **client** is a secondary user (mainly product purchases) and lives on its own canvas.

## Job statement format

Every job follows the Design Den formula and stays solution-free:

> **When** [situation / real-world trigger], **I want to** [motivation / goal], **so I can** [desired outcome / end state].

- Situation exists whether or not the product does (not "when I open the dashboard").
- Outcome is an end state, not a task.

## Data / measurement

Micro jobs can carry a `data` field holding funnel/conversion metrics (e.g., per-CTA click rate). The dashboard renders these in a **Data** section of the detail panel to help judge whether a job is being completed and where the drop-off is. The first example lives on the Exclusive Offers micro "Refer a product to a client" (5 CTAs, placeholder click rates). Real numbers will be sourced from ContextA8C analytics; see AGENTS.md for the field shape and `A4A-JTBD-TODO.md` for the wiring plan.

## Evidence & validation

Jobs start as **draft** and become **validated** only when backed by at least one real customer source (P2 post, HubSpot call, or Zendesk ticket), ideally with a customer quote. This happens in the dashboard's detail panel; see AGENTS.md for the workflow and persistence notes.

## Files

| File | What it is |
|------|------------|
| `a4a-jtbd.json` | **Source of truth.** Structured, machine-readable list of every job. Drives the dashboard. |
| `a4a-jtbd-map.html` | **The interactive dashboard.** Open in a browser. FigJam-style pan/zoom canvas, light/dark, Agency/Client toggle, filters, draft→validated workflow, Export JSON. |
| `A4A-JTBD.md` | **Human-readable map.** The same jobs in prose, organized by layer. |
| `A4A-JTBD-TODO.md` | Roadmap: remaining functions to map, the GitHub repo plan, persistence/PR wiring, Zendesk evidence pass. |
| `A4A-Layer-Foundation-Source.md` | Source material: pillar offering (landing pages) + dashboard nav functions. |
| `JTBD-Research-and-Framework-Context.md` | Background on JTBD theory (Strategyn/Ulwick) and the Design Den sessions. |
| `AGENTS.md` | Conventions and step-by-step process for anyone (human or AI) adding to the map. |

## Using the dashboard

Open `a4a-jtbd-map.html` in a browser.

- **Drag** to pan, **scroll** to zoom, **⤢** to fit.
- **Click a card** for full detail, evidence, and the validation controls.
- **⊟ / +N** on a card collapses/expands its micros.
- Top bar: **Agency / Client** canvases, **Pillar / Status / Page** filters, **light/dark**, **Export JSON**. The **Page** filter (default "All pages") focuses a single dashboard area — e.g., "Marketplace" keeps its functions + micros + the pillars they roll up to in focus and grays out the rest.
- **ⓘ Key** (bottom legend) explains the pillars and layers.

When opened directly from disk, the dashboard reads an **embedded copy** of the data (browsers block local file fetches). When served (e.g., GitHub Pages), it reads `a4a-jtbd.json` live. **Until it's hosted, edits to jobs must be made in both `a4a-jtbd.json` and the embedded block in the HTML**: see AGENTS.md.

## Repository & hosting (GitHub Pages)

This project lives at **`github.com/Automattic/a4a-jtbd`**. The interactive map is hosted on **GitHub Pages**:

- **Live map:** https://automattic.github.io/a4a-jtbd/ (redirects to `a4a-jtbd-map.html`, which reads `a4a-jtbd.json` live)

`index.html` is a small redirect to the map so the Pages root opens it directly. `.nojekyll` tells Pages to serve the files as-is (no Jekyll processing). The canonical, editable dashboard file remains `a4a-jtbd-map.html`.

### First-time setup (run once, from this folder, by someone with access to the Automattic org)

```bash
# 1. Point at the repo and push (SSH avoids the HTTPS password issue)
git init
git add -A
git commit -m "Initial import"
git branch -M main
git remote add origin git@github.com:Automattic/a4a-jtbd.git
git push -u origin main

# 2. Enable Pages: Settings → Pages → Source: Deploy from a branch → main / (root)
```

### Updating later

```bash
git add -A && git commit -m "Update jobs" && git push
```

Pages redeploys automatically on push to `main`.

## Where this is headed

A GitHub repo as the hosted source of truth, with the dashboard on GitHub Pages reading `a4a-jtbd.json` directly, and Export rewired to open a PR: so validating or adding a job updates the canonical map with no manual file juggling. See `A4A-JTBD-TODO.md`.
