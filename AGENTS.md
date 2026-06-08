# AGENTS.md: How to extend the A4A JTBD map

Instructions for anyone (human or AI) adding to or editing this Jobs To Be Done framework. Read `README.md` first for the model. **Follow this exactly: the structure is settled.**

## The model (non-negotiable)

Strict three-level hierarchy, no intermediate tiers:

```
Pillar (Earn / Build / Grow)
  └─ Major function (many, side by side)
       └─ Micro function (many, CTA-level tasks)
```

- Pillars: exactly three: `earn`, `build`, `grow`. Don't add pillars.
- Major functions: the agency's jobs under a pillar. May be conceptual ("Predictable recurring income") or a dashboard area ("Agency Tier"). Always `kind: "anchor"`, `layer: "function"`. Siblings, never stacked.
- Micro functions: granular tasks, usually tied to a specific UI **CTA**. `kind: "task"`, `layer: "micro"`.
- There is **no "supporting" tier** anymore. Earlier drafts used `kind: "supporting"`; these were promoted to major functions. Do not introduce new supporting-kind nodes.

## Job statement formula (every job)

> When [situation], I want to [motivation], so I can [outcome].

- Situation = real-world trigger, independent of the product. Not "when I open X."
- Motivation = a verb-led goal, solution-free.
- Outcome = an end state, not a task.
- Stored as three separate fields (`situation`, `motivation`, `outcome`), not one sentence.

## Process for mapping a new function

1. **Gather ground truth** for the screen/feature:
   - Screenshot(s) of the screen and key sub-screens.
   - Support doc / KB article if one exists.
   - The code. It lives at `/Users/jeffgolenski/wp-calypso/client/a8c-for-agencies` (connected folder). Use Glob/Grep/Read on `sections/<feature>/` to confirm what the page actually does and to inventory the **CTAs** (buttons, links, modals). Use code as reference only: never quote it as customer evidence.
2. **Draft the major-function job** (one anchor) in the formula, mapped to its pillar(s).
3. **Draft the micro jobs**, one per meaningful CTA. Record the exact CTA in the `cta` field.
4. **Confirm with the user in chat** before writing to files.
5. **Write to all three** in lockstep (see below).

## Where to write (keep in sync)

Every job edit must land in **all three** until the project is hosted on GitHub:

1. `a4a-jtbd.json`: the source of truth (pretty-printed, one object per job).
2. `a4a-jtbd-map.html`: the `EMBEDDED_DATA` block near the top of the `<script>` (compact one-line objects). This is the fallback the dashboard uses when opened from disk. **If you skip this, the local dashboard won't show your change.**
3. `A4A-JTBD.md`: the human-readable prose map, under the right pillar/function.

After editing the HTML, sanity-check it:
```
# from the workspace shell, in the project folder
python3 -c "import re;open('/tmp/c.js','w').write(re.search(r'<script>(.*)</script>',open('a4a-jtbd-map.html').read(),re.S).group(1))" && node --check /tmp/c.js
python3 -c "import json;json.load(open('a4a-jtbd.json'))"   # JSON must parse
```

## JSON schema (per job)

```jsonc
{
  "id": "fn-agency-tier",            // stable, unique, kebab-ish. fn-* function, mc-* micro, pillar-* pillar
  "layer": "function",               // "pillar" | "function" | "micro"
  "function": "Agency Tier",         // function name (functions only). Pillars omit; micros use `title`.
  "group": "Agency tier",            // functions only: the dashboard page/area this belongs to. Powers the Page filter. Micros inherit their parent's group.
  "title": "Get my partner badges",  // micros only: the overall job the user is doing (card headline)
  "pillar": ["grow", "earn"],        // string or array; array of >1 renders as "Multi"
  "parent": ["pillar-grow", "pillar-earn"], // id or array; first entry is the primary parent (drives layout)
  "executor": "agency",              // "agency" (primary) | "client" (secondary canvas)
  "kind": "anchor",                  // "anchor" (pillar/function) | "task" (micro)
  "cta": ["Download your badges"],   // micros only: array of the exact UI CTA(s); >1 is denoted on the card
  "situation": "...", "motivation": "...", "outcome": "...",
  "status": "draft",                 // "draft" | "validated"
  "source": ["...", "https://..."],  // reference material (screenshot, KB, code path)
  "evidence": [                       // customer proof; required (>=1) to validate
    { "url": "https://...", "type": "p2|hubspot|zendesk|link", "quote": "..." }
  ],
  "note": "optional clarifier",
  "upcoming": true,                  // optional: feature not yet released. Renders a distinct dashed/striped "Upcoming" state.
  "audience": "nux",                 // optional: "nux" (new user) | "returning". Renders a "New user" / "Returning" badge to differentiate experiences sharing one page (e.g., Overview).
  "intermittent": true,              // optional: availability comes and goes (e.g., a promo/incentive that turns on and off). Renders an "Intermittent" badge.
  "redundant": true,                 // optional: duplicates functionality elsewhere; flagged for the consolidation pass. Renders a "Redundant" badge. Put the overlap details in `note`.
  "gated": true,                     // optional: only available to certain agency tiers (e.g., Agency/Pro/Premier Partners). Renders a "Tier-gated" badge. Put the specific tier condition in `note`.
  "data": {                           // optional: funnel/conversion data for validation. Renders a "Data" section in the panel.
    "metric": "CTA click rate", "placeholder": true, "periodLabel": "Last 30 days",
    "note": "...", "ctaStats": [ { "cta": "...", "views": 3000, "clicks": 1140 } ]
  }
}
```

ID conventions: `pillar-earn`; functions `fn-<slug>`; micros `mc-<function-slug>-<n>`. (Some early function ids are `pillar-<x>-sN` for promoted jobs: leave them; ids are opaque.)

## Validation & evidence

- A job becomes `validated` only with **≥1 evidence entry** (a real P2 / HubSpot / Zendesk URL, ideally with a customer `quote`).
- In the dashboard, evidence and validation are edited in the detail panel; changes save to the browser's localStorage and **Export JSON** downloads the merged file to save over `a4a-jtbd.json`.
- To pull a customer quote from a private source (P2 / Zendesk / HubSpot), use the ContextA8C connectors in chat, then write the quote into the job's `evidence`.

## Dashboard internals (for editing the HTML)

- Layout is **strict bands by layer** (`layerRank`: pillar 0, function 1, micro 2). Card heights are measured at render so bands never overlap. Don't reintroduce depth-based vertical positioning.
- `placedKids()` excludes any `kind: "supporting"` from the canvas. Keep micros as `kind: "task"` so they render and aren't treated as supporting.
- Multi-pillar nodes draw a solid edge to the primary parent and dashed edges to the others.
- Collapsible toggle uses `n._children.some(...)` (independent of collapsed state) so the re-expand control persists.

## Style / UX conventions already settled (don't regress)

- Default **light** mode; mono line-icons for the theme toggle (no emoji).
- JTBD sentences are a single standardized color, **no bold**.
- Card headline: pillars show the pillar name; functions show `function`; micros show their `title` (the job), with the `cta` list in a labeled footer at the bottom.
- Keep the canvas clean: pillars → functions (side by side) → micros (bottom band).

## Roadmap

See `A4A-JTBD-TODO.md` for remaining functions, the GitHub repo + Pages plan, and rewiring Export → PR.
