# Jobs To Be Done: Research & Framework Context

_Compiled for the Automattic for Agencies (A4A) JTBD effort: part of the Designomattic "Design Den" class. Last updated June 2, 2026._

This document collects and summarizes the source material for building A4A's Jobs To Be Done framework: the foundational JTBD theory (Strategyn / Tony Ulwick), the three internal Design Den posts, and Jeff's own proposed layer structure for mapping A4A.

---

## 1. Strategyn: "Jobs-to-be-Done (A Comprehensive Guide)"

Source: https://strategyn.com/jobs-to-be-done/ (Tony Ulwick, Strategyn)

**What it is:** The canonical, foundational explanation of JTBD theory and its accompanying methodology, Outcome-Driven Innovation (ODI). Ulwick originated JTBD in 1990; Clayton Christensen later popularized it.

**Core idea:** People buy products and services to get a "job" done. Levitt's line: "people don't want a quarter-inch drill, they want a quarter-inch hole": captures the shift from a *product* mindset to a *problem* mindset. The job is stable over time even as the products that serve it (records → cassettes → CDs → MP3 → streaming) come and go. That stability makes the job a durable foundation for strategy.

**Three core principles:**

- Jobs are stable; products are not.
- Customer needs are measurable: they are the metrics ("desired outcomes") customers use to judge success. A single market can hold 50–150+ of them.
- Innovation wins when it gets the job done significantly better (~20%+) or more cheaply.

**The ODI process (how the theory is applied), in phases:**

1. Define the customer and the core functional job (a single, solution-free statement).
2. Uncover customer needs / desired outcomes using the Universal Job Map.
3. Gather quantitative data on importance vs. satisfaction to find *underserved* (unmet) and *overserved* needs.
4. Discover hidden segments of opportunity via outcome-based segmentation.
5. Formulate market strategy via the Growth Strategy Matrix.
6. Formulate product strategy aligned to unmet outcomes.

**The Universal Job Map**: every job is made of the same eight steps: Define, Locate, Prepare, Confirm, Execute, Monitor, Modify, Conclude. It depicts what the customer is trying to *get done* (in ideal order), not what they currently *do* (so it's not a journey map or process map). Average jobs have 10–20 steps.

**Three customer roles** (especially relevant for B2B like A4A):

- **Job Executor**: the primary user doing the core job.
- **Product Lifecycle Support Team**: installs, maintains, upgrades, supports.
- **Buyer**: makes the purchase decision.

**Growth Strategy Matrix**: five strategies: Differentiated, Dominant, Disruptive, Discrete, Sustaining: matched to whether segments are underserved, overserved, or non-consumers.

**Why it matters for us:** ODI provides a rigorous, measurable backbone. Christensen's "hire/fire" framing is the intuitive front door; Ulwick's job map + desired outcomes + segmentation is the operational engine. Design Thinking and Lean Startup are complementary: use JTBD/ODI to decide *where* to focus, then those to explore solutions.

---

## 2. Designomattic: "Jobs To Be Done Design Den" (proposal/kickoff)

Source: https://designomattic.wordpress.com/2026/01/21/jobs-to-be-done-design-den/ (by leilabyron, Jan 21, 2026)

The kickoff post proposing the 3-session Design Den series (Design Dens are peer-led internal sessions for designers to build craft). Priority seating for designers; non-designers waitlisted: though several PMs and cross-functional leads (Ali Uğurlu, Mike, Filippo, Jarosław) commented asking to join, signaling broad relevance beyond design.

Proposed syllabus:

- **Session 1: How to Work With JTBD** (facilitated by Ashley Stadille)
- **Session 2: How to Design With JTBD**: WooCommerce case study (Mark Power-Freeman & Veronica Fasulo)
- **Session 3: How to Be a JTBD Owner** (Ashley Stadille): group critique of homework maps

---

## 3. Designomattic: "Session 1 Recap: How to Work With JTBD"

Source: https://designomattic.wordpress.com/2026/04/02/jtbd-design-den-session-1-recap-how-to-work-with-jtbd/ (Apr 2, 2026)

Introduced JTBD from the ground up using CPG examples (nobody wants a hammer; they want to hang a picture).

**The job statement formula:**

> **When [situation / trigger], I want to [motivation / goal] so I can [desired outcome].**

- **Situation**: real-world context that exists whether or not your product does ("when I'm preparing for a sales event"), *not* a product state ("when I open the dashboard").
- **Motivation**: what they're actually trying to do; starts with a verb; product-independent.
- **Outcome**: the end state / the "why," how they know they're done: not the activity.

Worked example: _"When I see an unexpected dip in sales, I want to understand whether it's a distribution problem, a pricing issue, or a competitive response so I can decide the right action and explain it clearly to my team."_

Jeff's own contribution in the session: well-formed statements "almost present themselves as a question rather than a statement, which leaves it open enough to figure out what avenue you want to take."

**Key learnings / traps:** Outcomes are end states, not tasks ("keep track of my stock and fulfill orders" = task; "so I always know what inventory is available to sell" = outcome). Use Claude/AI to *pressure-test* draft statements, not to write them from scratch.

**When to use JTBD:** prioritization, evolving customer segments (especially as AI brings less-technical users in), and keeping teams aligned on the problem space rather than feature-chasing competitors. Useful even for established products.

Also referenced: the **Dotcom JTBD Library** (https://dotcom.wordpress.com/customers/jtbd/).

---

## 4. Designomattic: "Session 2 Recap: How to Design With JTBD"

Source: https://designomattic.wordpress.com/2026/04/16/jtbd-design-den-session-2-recap-how-to-design-with-jtbd/ (Apr 16, 2026)

Moved from theory to practice via the **Commerce in a Box (CIAB)** case study (Veronica Fasulo & Mark Power-Freeman), plus a hands-on map-building workshop (Ashley Stadille).

**CIAB case study highlights:**

- All-in-one commerce solution for non-technical solopreneurs/small businesses (not WooCommerce power users). Grounded in **181 user interviews** across booking, storefront, orders, fulfillment.
- Built a hybrid job map (part JTBD, part journey, part service blueprint): four maps (service & product merchants; services & products shoppers). Helped catch jobs framed too much like tasks.
- Structured the map into **four layers**; ran a collaborative workshop in Denver so engineering, product, design, research, and marketing all co-owned the jobs, micro-jobs, and outcomes. Retro called this alignment one of the project's biggest wins.
- Built a vibe-coded **living reference website** (via Claude Code) so the map was a daily reference, not a Figma artifact only designers touched.
- Ran a prioritization exercise (must-have / nice-to-have / not relevant) at the job level.

**Impact of JTBD on CIAB:**

- **Reversed a prioritization call:** the micro-job "handle offline payments accurately" (e.g., salons) surfaced as a major pain → product reversed course and prioritized POS integration.
- **Shaped design direction:** "understand how my business is performing" revealed scattered data → drove a new payments-focused dashboard.
- **Grounded AI in real jobs** rather than hype (e.g., AI image co-creation, compliance-aware copy).
- **Cultural shift:** product people began asking to **test jobs**, not screens/flows in isolation.
- **Email lifecycle** overhauled by mapping all emails (.com, WooCommerce, Jetpack) against the map.

**Workshop / how to build a map:**

- Jobs must be grounded in real customer evidence, not assumptions; gold standard is direct interviews.
- **Enterpret**: a customer-feedback aggregation tool rolling out across Automattic (support tickets, Reddit, reviews, NPS, internal feedback; eventually interview data). Already used by Woo. Used live with Claude (Enterpret MCP) to surface themes and quantify pain by comment volume (e.g., 12,000+ comments on one theme vs. 1,000+ on another → prioritization clarity).
- Example refined job statement from the demo: _"When I need to add a new capability to my WooCommerce store, I want to know upfront whether a plugin will work with my existing theme and setup so I can extend my store's functionality without risking my live site, wasting money, or losing my clients' trust."_

**Homework:** build out a full JTBD map from a confident job statement, to bring to Session 3 ("How to Be a JTBD Owner," May 13).

---

## 5. Jeff's proposed A4A layer structure (comment #30385)

Source: https://designomattic.wordpress.com/2026/04/16/jtbd-design-den-session-2-recap-how-to-design-with-jtbd/#comment-30385 (Apr 21, 2026)

Jeff's note about A4A: A4A has its own JTBD, but its agencies *also* use Woo, Jetpack, etc., so every one of those products' jobs also applies to A4A's customer base ("so many jobs, so little time"). For the voice-of-customer input, if Enterpret access is an issue, A4A has a fallback system Jeff built to scrub user tickets and thousands of call transcripts at scale.

**The proposed framing: break A4A's JTBD into three layers as a team-wide guide:**

1. **A4A's primary pillars: Earn, Build, Grow.** The program is built around these three; each is a very high-level JTBD for agencies.

2. **Major functions of A4A:** client management, site management, referrals, site migrations, etc. These are mid-level JTBD that roll up to the pillars. (E.g., in order to *Earn*, an agency needs to set up referrals, migrate sites, set up WooPayments, etc.)

3. **Micro functions:** the tiny base-level tasks within each major function (e.g., add client details to a referral, add a logo to a referral, preview a referral before sending).

**Plan of attack:** coupled with user feedback, start with the **top 3 JTBD** and work down the levels, ending up with dozens (or more). (cc: Noam Almos)

> **Note for the build phase:** Layers 1→2→3 map cleanly onto the Strategyn hierarchy: pillars ≈ high-level jobs, major functions ≈ jobs / job groups, micro functions ≈ job steps / desired outcomes. When we write these, each should follow the Session 1 formula (When… I want to… so I can…) and stay solution-free.

---

## Sources

- [Strategyn: Jobs-to-be-Done Comprehensive Guide](https://strategyn.com/jobs-to-be-done/)
- [Designomattic: JTBD Design Den (kickoff)](https://designomattic.wordpress.com/2026/01/21/jobs-to-be-done-design-den/)
- [Designomattic: Session 1 Recap](https://designomattic.wordpress.com/2026/04/02/jtbd-design-den-session-1-recap-how-to-work-with-jtbd/)
- [Designomattic: Session 2 Recap](https://designomattic.wordpress.com/2026/04/16/jtbd-design-den-session-2-recap-how-to-design-with-jtbd/)
- [Jeff's comment #30385: A4A layer structure](https://designomattic.wordpress.com/2026/04/16/jtbd-design-den-session-2-recap-how-to-design-with-jtbd/#comment-30385)
