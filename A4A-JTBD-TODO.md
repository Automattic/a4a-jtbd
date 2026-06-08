# A4A JTBD: To-Do & Next Steps

_Running notes for where this work is headed after the current mapping sessions._

## Up next (added end of session)
- [x] Review Overview JTBD for **returning users** — rebuilt Overview as two functions (NUX + Command center) with proper CTA micros and an `audience` badge (New user / Returning) on the canvas
- [x] Finish all remaining **agency** pages (Purchases, Referrals, Migrations, WooPayments, Plugins, Reports, Partner Directories, Team, Global) — done; only the **Client canvas** remains
- [x] Map the **Client (secondary user) canvas** — one client pillar ("Get and run the products my agency set me up with") + 4 functions (Get started from my referral / Pay for what my agency recommended / See and manage my subscriptions / Manage my billing) + micros; `executor: client`, new "Client portal" group, client pillar color. Pillar/Page/State filters hide in Client mode; Status stays.
- [x] Get this into **GitHub** (repo as source of truth + Pages hosting) — live at github.com/Automattic/a4a-jtbd; map hosted at https://automattic.github.io/a4a-jtbd/ (reads a4a-jtbd.json live)
- [ ] Record a **demo** of the dashboard
- [ ] Share progress with **Ashley and Noam**
- [ ] Clean up the **panel details UI** (the right-hand detail drawer)
- [x] Fix **canvas rendering on zoom** — fixed: `will-change: transform` was kept on permanently, caching the layer at 100% and stretching the bitmap (blurry text) on zoom. Now `will-change` is toggled only during active pan/zoom and dropped ~180ms after, so the browser re-rasterizes crisply at the current zoom. _(If any blur remains at extreme zoom, revisit with a re-render-at-scale approach.)_

## Dashboard UI (done this session)
- [x] Added a reusable **Tier-gated** badge (legend Key + AGENTS.md schema)
- [x] Widened micro cards + `white-space:nowrap` on badges so multi-badge cards don't grow taller
- [x] **Page filter** list sorted alphabetically ("All pages" pinned on top)
- [x] **ⓘ job-count breakdown** popover in the header: tallies Pillars / Major functions / Micro functions + Total (live per Agency/Client view)

## In progress (current sessions)
- [x] Finish **Layer 2: Major Functions** JTBD for all dashboard areas _(all agency areas complete; Client canvas still to do)_:
  - [x] Overview: New User Experience (first-time / onboarding)
  - [x] Overview: steady state (command center)
  - [x] Agency tier
  - [x] Exclusive offers
  - [x] Resources and tools (Learn; Developer tools; + upcoming: Agent studio, Benchmarks, AI and MCP)
  - [x] Sites (mapped as five major functions: Manage / Add & set up / Secure & online / Fast / Maintain & operate)
  - [x] Marketplace (mapped as four major functions: Choose hosting / Find products / Buy for my portfolio / Refer to a client)
  - [x] Purchases (mapped as four major functions: Manage my subscriptions / Put a subscription to work / Track client referrals / Billing & payments — major functions framed as "subscriptions"; micro tasks keep "license" language)
  - [x] Referrals (four major functions: Track referrals & earnings / Inspect & manage a referral / Set up & manage payouts / Understand referral earnings)
  - [x] Migrations (three major functions: Migrate to better hosting / Earn commissions on migrations / Set up migration payouts — added **Intermittent** + **Redundant** badge states; flagged overlaps with Marketplace hosting & Referrals payouts for consolidation)
  - [x] WooPayments (four major functions: Set up on client sites / Track earnings / Learn about revenue share / Set up payouts — flagged the tracker + payouts as Redundant with Referrals/Migrations)
  - [x] Plugins (two major functions: Keep plugins current across all sites / Manage a plugin site-by-site)
  - [x] Reports (Beta) (three major functions: Show clients the value of my work / Build and send a client report / Track reports I've sent; flagged "Schedule recurring delivery" Upcoming)
  - [x] Partner Directories (Tier-gated; two major functions: Get my agency listed in partner directories / Get matched with the right client leads; added a reusable **Tier-gated** badge; lead matching flagged Upcoming; flagged the listing/lead-matching field overlap as an IA-consolidation candidate)
  - [x] Team (one major function: Run my agency with a team; 8 micros covering invite, member/invite list, pending-invite management, roles, remove, transfer ownership, leave, and accept-invite)
  - [x] Global (always-available sidebar actions; two major functions: Manage my account & profile (avatar menu) / Get help anytime (help icon); new "Global" page group)
- [x] Build **Layer 3: Micro Functions** under each major function _(done for every function mapped so far; continue for remaining functions)_
- [x] Flesh out the **Clients (secondary user)** section — done on its own Client canvas
- [ ] Validate all layers against incoming customer feedback (Enterpret / A4A ticket + transcript synthesis)
- [ ] Resolve open question: should Build and Grow each split into two pillar-level jobs?
- [ ] **(Jeff)** Scour Zendesk later to find evidence: pull supporting tickets/quotes to validate draft jobs

## Next: living GitHub repo
- [ ] Stand up a GitHub repo as the **source of truth** for the JTBD map
- [ ] Store jobs in a **structured, machine-readable format** (e.g., JSON or YAML) so they can drive a visual: not just prose markdown
  - Proposed schema per job: `id`, `layer` (pillar / function / micro), `pillar` (earn/build/grow), `parent` (id), `executor` (agency / client), `situation`, `motivation`, `outcome`, `source`, `status` (draft/validated), `evidence` (feedback links)
- [ ] Keep human-readable `A4A-JTBD.md` in sync (or generate it from the structured data)
- [ ] Define an easy update workflow so anyone can add/edit a job via PR
- [ ] **Wire up persistence properly.** The visual map currently can't write to the file from the browser, so edits (status + evidence) save to localStorage and the **Export JSON** button downloads the merged `a4a-jtbd.json` to save over the file manually. Once this lives on GitHub, rewire **Export → open a PR** (or commit via the GitHub API) so validating a job updates the source of truth directly, no manual file swap.

## Data instrumentation (measure success / conversion per micro job)
- [x] Add a `data` field to jobs and a **Data** section in the dashboard panel. First example built on the Exclusive Offers micro **"Refer a product to a client"**: per-CTA click rate (placeholder), shown as labeled bars with clicks/views and a "Placeholder" badge.
- [ ] **(Jeff)** Pull **real** funnel/conversion data to replace the placeholder (CTA click rates for the 5 refer CTAs).
- [ ] Wire **ContextA8C** (Tracks / analytics) to source live CTA click + conversion data; map each `cta` to its Tracks event (e.g., `calypso_a4a_exclusive_offers_cta_click` with `offer_id`).
- [ ] **(Jeff)** Sync with **data engineering** on an aggregate-funnel solution. Note: the ContextA8C Tracks tool is **per-user only** (queries one `user_login`/`wpcom_user_id`), so it can't produce population-level click/conversion rates. The mc.a8c.com funnel view (e.g., funnel #61050) is auth-gated + JS-rendered, so it can't be fetched programmatically. Need an export or an aggregate query path.
- [ ] Decide: snapshot data into `a4a-jtbd.json` periodically, or have the hosted dashboard pull live.
- [ ] Roll the `data` pattern out to other high-value micros to support draft → validated decisions (data complements customer-quote evidence).
- [ ] **Low-conversion alerting in the dashboard.** When a CTA's conversion/click rate falls below a threshold, visually flag the job (e.g., turn the card red / show a warning badge) so weak spots jump out at a glance. Define the threshold(s), decide per-CTA vs. whole-job rollup, and make it work alongside the existing pillar/status filters and the Upcoming state.

## Then: dynamic visual map
- [ ] Build an interactive **HTML visualization** of the three-layer hierarchy (pillars → functions → micro)
  - Likely a collapsible tree / nested map; click a node to see the full job statement, executor, status, and evidence
  - Filter by pillar, executor (agency vs. client), or status (draft vs. validated)
  - Reads directly from the structured data file so it never goes stale
- [ ] Host it (e.g., GitHub Pages) so the team can reference it daily: inspired by the Woo CIAB "living reference site"
- [ ] **Update-on-the-fly goal:** whenever we launch something new in the product, add/update the job in the data file → visual map and repo update automatically

## Open questions to decide later
- [ ] Data format: JSON vs. YAML
- [ ] Visualization approach: hand-rolled HTML/JS (e.g., D3) vs. a lightweight framework vs. Mermaid
- [ ] Who owns updates and review (job ownership / maintenance cadence)
