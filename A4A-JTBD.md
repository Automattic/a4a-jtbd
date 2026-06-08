# Automattic for Agencies: Jobs To Be Done Map

_A living, three-layer JTBD map for A4A. Built in the Designomattic "Design Den" practice. The executor throughout is the **agency owner/operator** (the A4A customer), unless otherwise noted._

**Job statement formula:** _When [situation/trigger], I want to [motivation/goal], so I can [desired outcome]._

**Data / measurement:** Micro jobs can carry a `data` field with funnel/conversion metrics (e.g., per-CTA click rate), surfaced in a **Data** section of the dashboard panel to support draft to validated decisions. First example: the Exclusive Offers micro **"Refer a product to a client"** tracks click rate across its 5 CTAs (currently placeholder; to be sourced from ContextA8C analytics).
Situations are real-world and product-independent. Outcomes are end-states, not tasks. Statements stay solution-free.

**The three layers**

1. **Primary pillars**: Earn, Build, Grow. The highest-level jobs an agency hires A4A for.
2. **Major functions**: the dashboard's functional areas; mid-level jobs that roll up to the pillars. _(to be built next)_
3. **Micro functions**: granular tasks within each major function. _(built last)_

Status: Layer 1 drafted from the A4A landing pages, pending validation against customer feedback. Layers 2 & 3 to follow.

---

## LAYER 1: Primary Pillars

### 🟢 Earn: recurring, compounding revenue

**Anchor job**
> When the project-based model leaves my income starting from zero every month, I want to turn work I've already delivered into revenue that recurs on its own, so I can run my agency on predictable income instead of the next sale.

**Major functions** (Layer 2, roll up to Earn)
- **Predictable recurring income**: When a project wraps and my pipeline resets, I want past work to keep paying me, so I can stop depending on constantly winning new projects to stay afloat.
- **Earn from recommendations**: When I recommend the tools and hosting a client needs anyway, I want to be rewarded for that expertise over time, so I can earn from advice I'm currently giving away for free.
- **Profit on products sold**: When I package and price my services, I want to capture margin on the products behind them, so I can grow profit without raising client fees or adding labor.

### 🔵 Build: deliver & operate client sites efficiently

**Anchor job**
> When I'm responsible for many client sites at once, I want to operate all of them reliably from one place, so I can spend my time on client outcomes rather than administrative overhead.

**Major functions** (Layer 2, roll up to Build)
- **Manage everything in one place**: When my sites, licenses, updates, and billing are scattered across tools, I want them unified, so I can manage scale without things slipping through the cracks.
- **Deliver on trusted infrastructure**: When a client needs a fast, secure, scalable site, I want to build on infrastructure I trust, so I can deliver dependable results without becoming a hosting expert myself.
- **Catch issues before clients do**: When something goes wrong on a client site, I want to catch and resolve it before the client notices, so I can protect my reputation and keep their confidence.

### 🟣 Grow: win more of the right business & level up

**Anchor job**
> When I want my agency to grow beyond word-of-mouth, I want qualified demand and recognized credibility to come to me, so I can win better clients without it consuming all my time.

**Major functions** (Layer 2, roll up to Grow)
- **Attract qualified clients**: When I need a steady flow of new business, I want the right clients to find and approach me, so I can grow without living in cold outreach.
- **Prove expertise & credibility**: When I'm competing in a crowded market, I want credible proof of my expertise, so I can earn the trust of higher-value clients.
- **Expand skills & offerings**: When the platform and market keep evolving, I want my team's skills and offerings to stay ahead, so I can expand what we sell and command premium rates.

**Open question for validation:** Build and Grow each carry two distinct motivations (Build = operate efficiently *and* deliver quality; Grow = get demand *and* build standing). Decide against feedback whether either pillar should split into two pillar-level jobs.

---

## LAYER 2: Major Functions
_Derived from the dashboard navigation (Overview, Agency tier, Exclusive offers, Resources and tools, Sites, Marketplace, Purchases, Referrals, Migrations, WooPayments, Plugins, Reports, Partner Directories, Team), each rolling up to one or more pillars._

### ⭐ Overview (one page, two audiences) — rolls up to Earn + Build + Grow
_The Agency Overview is partly dynamic: it serves a different experience to brand-new agencies (NUX) than to returning ones. We map it as two functions, tagged with `audience` (NUX vs Returning) and differentiated on the canvas. Sources: dashboard screenshot, `sections/overview/`._

#### Overview — New User Experience _(audience: NUX)_
> When I've just signed up and land in the dashboard, I want to quickly understand what A4A can do and where to begin, so I can feel confident and start getting value fast.
- **Work through my next steps**: follow a guided checklist of first steps so I make early progress without feeling lost. _CTAs: Add a site · Explore hosting & plugins · Start earning commission on referrals · Invite your team_
- **Set up how I get paid**: add my payout details so I get paid as soon as I start earning. _CTA: Add payout information now_
- **Take the welcome tour**: take a guided tour so I learn the product by seeing it in action. _CTAs: Start tour · Relaunch welcome tour_
- **Get a strategy call to start strong**: book a call with the A4A team for tailored guidance. _CTA: Schedule a call_
- **See what A4A offers**: see the program's value up front so I feel confident committing. _CTAs: Welcome tour intro · Check out the overview page_

#### Overview — Command center _(audience: Returning)_
> When I log in to run my agency, I want a launchpad that surfaces what needs attention and quick ways to act, so I can jump straight to what matters.
- **Resolve account alerts**: see and resolve alerts like missing payout info. _CTA: Add payout information now. (Shown on commission activity.)_
- **Check my tier & influenced revenue**: see tier and influenced revenue at a glance. _CTAs: View tiers · Influenced revenue ⓘ. (Overlaps Agency tier — consolidation candidate.)_
- **Quickly add sites or products**: jump straight into adding from the overview. _CTAs: Add sites · Add products. (Overlaps Sites / Marketplace.)_
- **Catch up on news & updates**: scan recent news, events, and updates. _CTA: News and updates_
- **Accelerate growth with a call**: book a strategy call. _CTAs: Schedule a call · I'm not interested. (Overlaps NUX call.)_
- **Start earning with WooPayments**: set up WooPayments revenue share. _CTA: Earn Revenue Share. (Overlaps WooPayments.)_
- **Get help or replay the tour**: replay the tour or reach support. _CTAs: Relaunch welcome tour · Contact sales & support · Program incentive details_
- **Browse hosting & products from Overview**: explore hosting and products from the overview. _CTAs: Explore WordPress.com · Pressable · Jetpack · WooCommerce. (STAGNANT — duplicates Marketplace; flagged for removal.)_

### ⭐ Agency Tier
_Where agencies see their tier standing and influenced-revenue (IAR) progress, what each tier unlocks, their current benefits, and badge downloads. Rolls up to: **Grow** (primary) + **Earn** (tier progress is revenue-driven). Sources: dashboard screenshot, [tiers & benefits KB](https://agencieshelp.automattic.com/knowledge-base/agency-tiers-and-benefits/), `sections/agency-tier/`._

**Anchor job** _(Grow · Earn)_
> When I'm investing real effort into the A4A partnership, I want to understand my current benefits and what it takes to reach the next level, so I can make the most of them and keep growing.

**Supporting jobs**
- _(Earn · Grow)_ When I'm gauging my momentum, I want to see how much influenced revenue I've generated against the next tier's threshold, so I can tell how close I am and what's left to earn.
- _(Earn)_ When I don't know what actually counts toward my tier, I want to understand how influenced revenue is calculated (referrals, client purchases, WooPayments volume), so I can focus on the activities that move me up fastest.
- _(Grow)_ When I'm weighing whether to push for a higher tier, I want to see exactly what each tier unlocks, so I can judge whether the rewards justify the effort.
- _(Grow)_ When I've earned a tier, I want to understand the requirements to keep it, so I can avoid slipping back and losing benefits I depend on.
- _(Grow)_ When I want to prove my expertise to prospects, I want to download and display my partner badges, so I can stand out and win trust in a crowded market.

**Micro jobs** _(title: statement: CTA[s])_
- **Understand my influenced revenue**: When I see my influenced-revenue number, I want to learn exactly what counts toward it and how it's tallied, so I can trust the figure and know which activities move me up. _CTA: Influenced revenue ⓘ → Learn more_
- **Compare higher tiers**: When I'm eyeing a tier above mine, I want to preview the exact benefits it unlocks, so I can set a concrete goal worth aiming for. _CTA: See what you'll unlock_
- **Review my current benefits**: When I want to remember what I'm entitled to, I want to jump to my current benefits, so I can make sure I'm using everything I've already earned. _CTA: View your benefits_
- **Get my partner badges**: When I've earned a tier with badges, I want to download them, so I can display proof of my status on my site and in pitches. _CTA: Download your badges_
- **Connect with my partner manager**: When I have a Partner Manager, I want to book time with them directly, so I can get strategic help progressing. _CTA: Book time with your partner manager_
- **Understand my tier status**: When I'm told I have early access or a protected tier, I want to understand what that status means and what's expected of me, so I can keep the benefits and stay on track. _CTAs: Learn more (Early access) · Learn more (Tier protected)_
- **Manage my directory profile**: When my tier affects how I show up to prospects, I want to jump to my directory profile, so I can keep my listing current. _CTA: Manage your profile → /partner-directory_
- **Act on a benefit**: When I want to act on a benefit, I want to jump straight from my benefits list to the right tool, so I can do the work without hunting through the dashboard. _CTAs: Manage sites · Create Client Reports · Manage purchase · Make a referral · Add WooPayments (deep-link into other functions)_

### Exclusive Offers
_A searchable, filterable catalog of partner offers, each tagged **Refer** (recurring commission) or **Resell** (bulk discount to resell). Rolls up to: **Earn**. Sources: dashboard screenshot, `sections/exclusive-offers/`._

**Anchor job** _(Earn)_
> When I want to get the most out of my Automattic partnership, I want to see at a glance every exclusive offer available to me, both the discounts that save my agency money and the referral deals that earn me commission, so I can take advantage of the benefits that improve my bottom line.

**Micro jobs** _(title: statement: CTA[s])_
- **Find the right offer**: When I'm not sure which offers apply to my agency, I want to search and filter the catalog by product, offer type, and refer vs. resell, so I can quickly surface the deals worth acting on. _CTAs: Search · Filter (product / offer type / product type)_
- **Refer a product to a client**: When a client needs hosting or tools I'd recommend anyway, I want to refer them through an exclusive offer, so I can earn a recurring commission on the recommendation. _CTAs: Refer WordPress.com · Refer Pressable · Refer WordPress VIP · Refer Woo · Refer Jetpack_
- **Resell at a discount**: When I'd rather bill clients myself, I want to buy hosting or extensions in bulk at a discount and resell them, so I can improve my margins without raising client fees. _CTAs: Save on WordPress.com · Save on Pressable · Save on Woo · Save on Jetpack_
- **Earn on WooPayments volume**: When I build or migrate client stores, I want to set them up on WooPayments, so I can earn a passive share of their payment volume. _CTA: Earn with WooPayments_
- **Check an offer's terms**: When I'm about to commit to an offer, I want to review the program incentive terms, so I can understand the commission, eligibility, and payout before I act. _CTA: View terms_

### Learn (Resources and tools)
_The Resource Center: curated **Top resources** and **Client conversations that work** sections, plus a dynamic **Browse all** library (Search + Filters). Rolls up to: **Grow**. Sources: dashboard screenshot, `sections/learn/resource-center/`._

**Anchor job** _(Grow)_
> When I want to sharpen how I run and grow my agency, I want to find practical guides, playbooks, and training made for agencies, so I can improve how I operate and deliver better work for my clients.

**Micro jobs** _(title: statement: CTA[s])_
- **Get the top recommended resources**: When I don't know where to start, I want the most important resources surfaced up front, so I can act on the highest-value guidance without digging. _CTAs: Download guide · Learn more_
- **Improve my client conversations**: When I want to win and keep more business, I want practical ways to have better client conversations and build trust, so I can guide decisions that lead to new business and extended partnerships. _CTA: Learn more_
- **Find a specific resource**: When I'm looking for help on a specific topic or product, I want to search and filter the full library, so I can quickly find the exact guide, case study, or article I need. _CTAs: Search · Filter (product / resource type). Note: operates over the dynamic, ever-changing "Browse all" library._
- **Open and use a resource**: When I've found a resource that looks useful, I want to read, download, or watch it, so I can apply what I learn to my agency or client work. _CTAs: Learn more · Download guide · Watch video. Note: "Browse all" is dynamic and ever-changing; this generalizes the repeatable actions rather than mapping individual articles._

### Developer tools (Resources and tools)
_Live to all users. Local development, automated deploys, and disposable test/demo environments. Rolls up to: **Build**. Source: `sections/dev-tools/`._

**Anchor job** _(Build)_
> When I'm building and shipping client work, I want local development, automated deploys, and throwaway test environments, so I can move faster and demo safely without risking production.

**Micro jobs** _(title: statement: CTA[s])_
- **Build locally (WordPress Studio)**: When I need to build and test a WordPress site, I want to develop locally with no Docker or server config, so I can start building in one click on Mac or Windows. _CTA: Start building locally_
- **Automate deploys (GitHub Deployments)**: When I want code changes to go live reliably, I want to connect my GitHub repo so every push deploys automatically, so I can ship updates with full history and no downtime. _CTA: Automate your deploys_
- **Generate custom blocks (Telex)**: When I need a custom Gutenberg block, I want to describe it in plain language or upload a design, so I can get a production-ready block plugin without hand-coding. _CTA: Create blocks in minutes_
- **Test in the browser (WordPress Playground)**: When I want to try something in WordPress with zero setup, I want to run WordPress entirely in my browser, so I can experiment or learn, then close the tab with nothing to clean up. _CTA: Launch a browser playground_
- **Spin up a throwaway site (Jurassic.ninja)**: When I need a clean, disposable site to reproduce a bug or demo, I want to spin up a throwaway WordPress site in seconds, so I can test or demo risk-free and walk away with no cleanup. _CTA: Spin up a test site_

### Agent studio (Resources and tools) · ⏳ Upcoming
_Not yet released. AI agents that create PDFs, social graphics, and more for the agency. Rolls up to: **Grow**. Source: `sections/agent-studio/`._

**Anchor job** _(Grow)_
> When I need polished collateral for my agency without design or dev time, I want to use AI agents that produce it for me, so I can ship professional deliverables fast.

**Micro jobs**
- **Create a deliverable**: When I need a PDF, social graphic, or similar asset, I want to brief an AI agent on what I need, so I can get a production-ready deliverable without doing it by hand. _CTAs: New deliverable · Brief an agent_
- **Reuse past deliverables**: When I've created deliverables before, I want to find and build on what I've already made, so I can build on past work instead of starting over. _CTA: Open a deliverable_
- **See how it works**: When I'm new to Agent studio, I want to watch a quick intro of what it can do, so I can understand how to put it to work for my agency. _CTA: Watch "Agent studio in 60 seconds"_

### Benchmarks (Resources and tools) · ⏳ Upcoming
_Not yet released. Anonymous peer comparison across margin, retention, AI maturity, and more. Rolls up to: **Grow**. Source: `sections/benchmarks/`._

**Anchor job** _(Grow)_
> When I want to know whether my agency is healthy and competitive, I want to compare my KPIs against agency peers, so I can see where I'm ahead and where to focus.

**Micro jobs**
- **Submit my quarterly benchmark**: When a new quarter has closed, I want to submit my KPIs (it takes a few minutes and stays anonymized), so I can get into the peer comparison without exposing my details. _CTA: Submit benchmark_
- **See how I stack up**: When I want an honest read on my performance, I want to compare my numbers against peers using A4A and peers who aren't, so I can know exactly where I lead and lag. _CTA: View report_
- **Close the gaps that matter**: When I see metrics where I'm behind, I want to follow the playbooks, templates, and case studies linked to those gaps, so I can take concrete action to close them. _CTA: View recommended playbooks_
- **Know my AI maturity**: When I want to understand how my AI adoption compares, I want to see my 0-100 AI maturity score and tier against my peer set, so I can know what to focus on next. _CTA: View AI maturity score_

### AI and MCP (Resources and tools) · ⏳ Upcoming
_Not yet released. Control how external AI assistants access the A4A account via MCP. Rolls up to: **Build**. Source: `sections/ai-mcp/`._

**Anchor job** _(Build)_
> When I want to run my agency account through AI tools, I want to control how external AI assistants access A4A via MCP, so I can automate work safely on my terms.

**Micro jobs**
- **Enable MCP access**: When I want AI assistants to work with my A4A account, I want to turn on external AI agent access via MCP, so I can open the door to automation when I choose. _CTA: Enable MCP access_
- **Choose which tools AI can use**: When I want to limit what AI can do in my account, I want to review and toggle the available MCP tools, so I can grant only the access I'm comfortable with. _CTA: Available tools_
- **Connect an external AI assistant**: When I've enabled MCP and want to use my own AI assistant, I want to get the instructions to connect it, so I can drive my A4A account from the AI assistant I already use. _CTA: Connect external AI assistant_

### Sites (mapped as five major functions, all roll up to Build)
_The Sites dashboard manages all of an agency's sites from one place. It's broad enough that it maps to five distinct agency jobs. Sources: dashboard screenshots, `sections/sites/`._

#### Manage all my sites _(Build)_
> When I'm responsible for many client sites, I want one place that shows the health of every site, so I can stay on top of them all without logging into each one.
- **Find a site**: search my sites by name or URL to jump to the one I need. _CTA: Search for sites_
- **Focus on what needs work**: filter to the sites that need action so I spend time where it matters. _CTAs: Needs attention · Needs setup · Development · Favorites · Status filter_
- **Flag my key sites**: mark important sites as favorites to keep them one click away. _CTA: Favorite (star)_
- **Open a site to dig in**: open a site's detail panel to see and manage everything in one place. _CTA: Open site (click name)_
- **Take a quick action on a site**: use the quick-actions menu without leaving the list. _CTAs: View site · Visit WP Admin · Site settings · Copy this site · Remove site_

#### Add & set up sites _(Build)_
> When I take on a new site or client, I want to bring it into my dashboard or spin up a new one, so I can manage it alongside everything else.
- **Connect an existing site**: connect a site I run elsewhere without rebuilding it. _CTAs: Via the Automattic plugin · Via WordPress.com · Via Jetpack_
- **Create a new hosted site**: spin one up on managed hosting and start building. _CTAs: WordPress.com · Pressable_
- **Start a free development site**: develop now and only pay when I launch. _CTA: Create a site now (5 free licenses)_
- **Finish setting up a pending site**: complete a waiting license's setup to get it live. _CTA: Needs setup → Create site now_
- **Launch a development site**: prepare a dev site to take it live cleanly. _CTA: Prepare for launch_

#### Keep sites secure & online _(Build)_
> When a client trusts me with their site, I want to protect it from data loss, threats, and downtime, so I can prevent problems and recover fast when they happen.
- **Add protection to a site**: turn on backups, scanning, and uptime monitoring before something goes wrong. _CTAs: + Add Backup · + Add Scan · Enable Monitor_
- **Recover a site from backup**: restore from a backup or clone it to get back to working fast. _CTAs: Create backup now · Restore · Copy this site_
- **Find and fix threats**: scan a site and resolve threats to keep it clean. _CTAs: Scan now · Fix threat · Ignore_
- **Monitor uptime and get alerted**: monitor a site and set how I'm alerted so I know the moment it's down. _CTAs: Monitor toggle · Configure (interval / notifications)_

#### Keep sites fast _(Build)_
> When site speed affects my client's results, I want to measure and improve performance, so I can deliver fast sites and prove it.
- **Add Boost to a site**: turn on Boost to improve speed without manual tuning. _CTA: + Add Boost_
- **Check a site's performance**: run a performance test on mobile or desktop for a page to see real-world scores. _CTAs: Test again · Mobile / Desktop · Page selector_
- **Act on recommendations**: see the specific recommendations to know what to fix. _CTA: View all recommendations_

#### Maintain & operate sites _(Build)_
> When I run a site day to day, I want to keep it current and understand how it's doing, so I can keep it healthy and show clients value.
- **Keep plugins updated**: see what needs updating and update it to keep the site secure. _CTAs: Plugins (N Updates) → Manage in wp-admin_
- **Review a site's activity**: review the activity log to understand what changed and when. _CTA: View activity_
- **Check a site's stats**: check traffic and stats to understand engagement and report to clients. _CTAs: Stats → View full stats_
- **See and configure hosting**: view host, PHP, and WordPress version and adjust settings. _CTAs: Hosting tab · Hosting configuration · Change domain · Site settings_
- **Organize sites with tags**: tag and group sites to find and organize them my way. _CTA: Details → Add tag_

### Marketplace (mapped as four major functions; spans Build + Earn)
_The Marketplace is both the direct-purchase storefront (Build) and the referral engine for commissions (Earn); the "Refer products" toggle switches between modes. Sources: dashboard screenshots, `sections/marketplace/`._

#### Choose hosting _(Build + Earn)_
> When a client needs hosting, I want to compare Automattic's options and find the right plan, so I can put them on infrastructure that fits their needs and budget.
- **Compare hosting options**: compare WordPress.com, Pressable, and VIP side by side. _CTAs: Standard (WordPress.com) · Premier (Pressable) · Enterprise (VIP)_
- **Size the right plan**: size by installs, traffic, or storage. _CTAs: Display by WordPress installs / Traffic / Storage · Signature 1-10 / 11-17 / Premium 1-11_
- **See my current footprint** _(Build)_: see how many WordPress.com sites and which Pressable plans I own. _CTAs: "You own N sites" · Your current Pressable plan · Manage in Pressable_
- **Get expert help choosing**: book a demo with the hosting team. _CTAs: Schedule a demo · Request a demo_

#### Find products & extensions _(Build + Earn)_
> When a site needs a capability it doesn't have, I want to find the right product or extension, so I can add exactly what it needs.
- **Search & filter the catalog**: narrow to products that fit. _CTAs: Search · Filters (category / type / price)_
- **Choose a variant & quantity**: pick the right tier and amount. _CTAs: Variant selector · Quantity / bundle size_
- **Add to cart or referral**: move it toward purchase or a client referral. _CTAs: Add to cart · Add to referral_
- **See product details**: decide before adding. _CTA: View details_

#### Buy for my portfolio _(Build + Earn)_ — direct-purchase mode
> When I want to provision hosting or products myself, I want to buy them directly (in bulk when it pays off), so I can manage and bill them on my own terms.
- **Build & review my cart**: buy exactly what I intend. _CTAs: Cart · Remove_
- **Buy in bulk for resale margin**: buy at agency pricing to improve resale margin. _CTAs: Site / quantity slider · Add N sites to cart_
- **Assign a purchase to a site**: put a license to work where it's needed. _CTA: Assign to site (at checkout)_
- **Check out & pay**: complete the purchase. _CTAs: Checkout · Add payment method · Pay_

#### Refer to a client to earn _(Earn)_ — referral mode
> When a client needs something I can recommend, I want to refer it through A4A, so I can let them pay directly while I earn a commission.
- **Turn on refer mode**: build a referral instead of a direct purchase. _CTA: Refer products toggle_
- **Add an item to a referral**: assemble the package the client will pay for. _CTA: Add to referral_
- **See my estimated commission**: understand the upside before sending. _CTA: Your estimated commission_
- **Personalize the referral**: send a branded, trustworthy request. _CTAs: Client's email · Custom message · Your logo (Use profile logo / Upload / Send without logo / Replace file)_
- **Preview the referral email**: make sure it's right before sending. _CTA: Preview referral email_
- **Send or share the referral**: get it in front of the client. _CTAs: Send to Client · Copy referral link_
- **Refer enterprise (VIP) hosting**: earn on an enterprise deal I couldn't host myself. _CTA: Refer your client to VIP hosting_

### Purchases (mapped as four major functions; spans Build + Earn)
_The Purchases hub manages licenses and billing. Sources: dashboard screenshot, `sections/purchases/`._

#### Manage my subscriptions _(Build + Earn)_
> When I've bought products and hosting through A4A, I want to see and manage all my subscriptions in one place, so I can track what I'm paying for and who it's for.
- **Find a license**: search and filter by status. _CTAs: Search · All active / Unassigned / Assigned / Revoked_
- **Inspect a license**: expand for code, dates, owner, renewal. _CTAs: Expand row · Copy license code_
- **Issue a new license**: start a new purchase. _CTA: Issue new license. (Routes to Marketplace — overlaps Buy for my portfolio.)_
- **Download a license or product**: get the license/extension files. _CTAs: Download · Download Jetpack CRM Extensions_
- **Revoke a license**: stop paying for what I don't use. _CTAs: Revoke · Revoke bundle_

#### Put a subscription to work _(Build)_
> When I have a subscription I haven't used yet, I want to assign it to a site or spin up a new one, so I can put what I bought into service.
- **Assign a license to a site**: activate the product where it's needed. _CTAs: Assign · Assign license_
- **Create a WordPress.com site from a license**: spin up a site from an unused plan. _CTA: Create site. (Routes to Sites needs-setup — overlaps Add & set up sites.)_
- **Manage a hosted license in Pressable**: run the hosting where it lives. _CTA: Manage in Pressable ↗_
- **Configure a WordPress.com site**: change domain, hosting, settings. _CTAs: Set up site · Change domain · Hosting configuration · Edit in WP Admin · Prepare for launch. (Overlaps Sites Maintain & operate.)_
- **Upgrade a hosting plan**: give a site more resources. _CTA: Upgrade_

#### Track client referrals _(Earn)_
> When I've referred products to clients, I want to see which licenses belong to which client, so I can keep my referral relationships straight.
- **Spot referral licenses**: tell owned vs referred at a glance. _CTAs: Referral badge · Assigned / Unassigned tabs_
- **See who owns a referred license**: keep client records accurate. _CTAs: "[client] owns this" · Owned by (details). (Managed by the client; agency actions limited.)_

#### Manage billing & payments _(Build + Earn)_
> When I'm responsible for what my agency pays, I want to manage payment methods and review billing, so I can keep purchases funded and accounted for.
- **Manage payment methods**: keep a valid card on file. _CTAs: Payment methods ↗ · Add new card · Set as primary · Delete. (External via WordPress.com.)_
- **Review billing history**: reconcile spend. _CTA: Billing History ↗. (External via WordPress.com.)_
- **Pay or download an invoice**: stay current and keep records. _CTAs: Pay · Download_

### Referrals (mapped as four major functions; all Earn)
_The referrals & commissions hub: track earnings, inspect/act on each client referral, set up payouts, and learn how commissions work. Sources: dashboard screenshot, `sections/referrals/`._

#### Track my referrals & earnings _(Earn)_
> When I refer products to clients, I want to see all my referrals and what I'm earning in one place, so I can keep tabs on my commission income.
- **See my payouts & earnings at a glance**: payouts, estimated quarterly earnings, pending orders. _CTAs: All time referral payouts · Estimated earnings (current / previous quarter) · Pending referral orders_
- **Scan all my client referrals**: track each client's status and value. _CTAs: Client / Purchases / Pending orders / Estimated commissions / Subscription status · Column settings (gear)_
- **Export my commissions**: reconcile or report my own way. _CTA: Download CSV_
- **Start a new referral**: get a new commission opportunity going. _CTAs: New referral / Make a referral. (Routes to Marketplace referral mode — overlaps Marketplace Refer.)_

#### Inspect & manage a referral _(Earn)_ — the View details panel
> When I want to know where a client's referral stands, I want to open its details and act on it, so I can move it forward and keep it accurate.
- **Check a referral's status & products**: know where it stands. _CTAs: View details · Referrals tab (Status · Products)_
- **Nudge a pending referral**: prompt the client to finish. _CTAs: Resend email · Copy link_
- **Archive a referral**: keep my list clean. _CTA: Archive_
- **Review the client's purchases**: understand the order behind the commission. _CTA: Purchases tab (Product · Site · Assigned on · Total)_
- **Assign a purchased product to a site**: put what they bought into service. _CTA: Assign to site. (Overlaps Purchases / Sites assignment.)_
- **See this client's commissions**: understand what the relationship earns. _CTA: Commissions tab_

#### Set up & manage payouts _(Earn)_ — Payout settings
> When I'm earning commissions, I want to set up how I get paid, so I can actually receive my money.
- **Connect my bank to get paid**: start receiving payouts. _CTAs: Connect your bank (Tipalti) · Add / Edit my details_
- **Complete tax details**: stay payable and compliant. _CTA: Tipalti tax form_
- **Check my payment status**: fix anything blocking payouts. _CTA: Payment status — Confirmed / Not Payable / Suspended / Blocked / Closed_

#### Understand referral earnings _(Earn)_ — FAQ
> When I want to know how commissions work, I want clear answers on earnings and eligibility, so I can maximize what I earn and stay eligible.
- **Learn how much I can earn**: focus on the most valuable referrals. _CTA: FAQ — How much can I earn?_
- **Understand eligibility & terms**: stay qualified. _CTA: FAQ — Eligibility requirements_
- **See the payout schedule**: plan around payout timing. _CTA: Payout schedule ↗_

### Migrations (mapped as three major functions; spans Build + Earn)
_Move client sites to better hosting and (intermittently) earn migration commissions. Two flags worth noting on the canvas: the commission incentive is **Intermittent**, and the hosting-selection + payout pieces are **Redundant** with Marketplace and Referrals. Sources: dashboard screenshot, `sections/migrations/`._

#### Migrate client sites to better hosting _(Build + Earn)_
> When a client is on subpar hosting, I want to move their site to WordPress.com or Pressable, so I can give them better performance and reliability.
> _Note: the "Decide which host fits" step overlaps Marketplace "Choose hosting"; the migration work itself (concierge, self-migrate guides, tracking) is unique to this page._
- **Decide which host fits** _(⚑ Redundant — nearly identical to Marketplace "Choose hosting")_: _WordPress.com vs Pressable · Compare on Marketplace · Schedule a demo · Create a development site_
- **Have Automattic migrate for me (concierge)**: _Concierge service · Start migrating your sites_
- **Self-migrate to WordPress.com**: _Self migrate to WordPress.com (6-step guide)_
- **Self-migrate to Pressable**: _Self migrate to Pressable (7-step guide)_
- **Track a migration in progress**: _"Migration in progress" badge · Migrate to this site. (Surfaces in Sites too.)_

#### Earn commissions on migrations _(Earn)_ · ⚑ Intermittent
> When I migrate client sites, I want to tag them and track their commission status, so I can get paid for the migrations I bring over.
> _Note: the migration incentive runs intermittently (e.g., ended Aug 31, 2025; promo windows reopen). Eligibility and commission amounts vary by period._
- **Tag migrated sites for commission**: _Tag sites for commission · Tag my self-migrated sites_
- **Track commission status**: _Commissions table (Site · Date added · Review status: Pending / Confirmed / Ineligible / Paid)_
- **Request (re)verification**: _Request verification · Request another verification_
- **Untag a site**: _Untag site_
- **See expected migration commission**: _Migration commissions expected in Q# · Sites pending review_

#### Set up migration payouts _(Earn)_ · ⚑ Redundant
> When I've earned migration commissions, I want to set up how I get paid, so I can receive my migration payouts.
> _Note: same Tipalti payout backend as Referrals "Set up & manage payouts." Consolidation candidate._
- **Connect my bank for migration payouts** _(Redundant — identical to Referrals payout setup)_: _Connect your bank (Tipalti) · Add my bank information_
- **Check my payment status**: _Payment status badge_

### WooPayments (mapped as four major functions; mostly Earn)
_Set up WooPayments on client stores and track the revenue-share commissions. Closely parallels Referrals (shared Tipalti payouts; a near-identical commission tracker). Sources: dashboard screenshot, `sections/woopayments/`._

#### Set up WooPayments on client sites _(Earn + Build)_
> When a client runs a store I manage, I want to get them onto WooPayments, so I can earn a share of their payment volume.
- **Add WooPayments to a site**: start the setup that unlocks commissions. _CTA: Add WooPayments to site_
- **Finish a site's setup**: get it live and eligible to earn. _CTAs: Continue setup · Install and activate the plugin_
- **Open a site's WooPayments admin**: finish or adjust configuration. _CTA: Visit WP Admin_

#### Track WooPayments earnings _(Earn)_
> When clients process payments through WooPayments, I want to track the commissions across their sites, so I can see what I'm earning.
> _Note: structurally similar to Referrals/Migrations commission views, but this is the only place to track WooPayments revenue share specifically (distinct data) — not flagged redundant._
- **See my commissions at a glance**: _Total WooPayments commissions paid · Estimated current quarter earnings to date_
- **Track each site's transactions & commissions**: _Site table (Transactions · Commissions paid · Timeframe commissions · WooPayments status)_
- **Check a site's commission eligibility**: understand which sites actually earn. _Commission eligibility: Eligible / Not eligible + reason (rejected Stripe account, internal account, existing merchant connected >30 days)_
- **Download a site's commissions report**: _Download commissions report_

#### Learn about WooPayments revenue share _(Earn)_ — Overview
> When I'm deciding whether to push WooPayments, I want to understand the revenue share and benefits, so I can pitch it to clients and earn.
- **Understand the revenue share**: 5 bps new clients; 2-3 bps existing. _CTAs: How Revenue Share works · See full terms_
- **Get benefits to share with clients**: _Benefits to share with your client (copy)_
- **Explore WooPayments further**: _Explore on WooCommerce.com ↗ · Contact us to learn more_

#### Set up WooPayments payouts _(Earn)_ · ⚑ Redundant
> When I've earned WooPayments commissions, I want to set up how I get paid, so I can receive my payouts.
> _Note: same Tipalti payout backend as Referrals & Migrations payouts. Consolidation candidate._
- **Connect my bank for WooPayments payouts** _(Redundant — shared Tipalti)_: _Connect your bank (Tipalti) · Add my bank information_
- **Check my payment status**: _Payment status badge_

### Plugins (mapped as two major functions; all Build)
_Manage plugins across all client sites (fleet view) and per site (the expanded detail panel). The list/detail UI is delegated to calypso `my-sites/plugins`; A4A adds routing + a "Jetpack required" prerequisite. Sources: dashboard screenshots, `sections/plugins/`._

#### Keep plugins current across all sites _(Build)_ — the fleet list
> When I manage plugins across many client sites, I want to see and update them from one place, so I can keep every site current without logging into each.
- **See every installed plugin across my sites**: _Installed plugins list (name · Sites count · Update available)_
- **Find a plugin**: _Search · Filter_
- **Update plugins that need it**: _Update available (N) · Update to version X.X.X. (Sites surfaces a per-site update count that points here.)_
- **Switch view & columns**: _List / table toggle · Column settings (gear)_
- **Act on plugins in bulk**: _Select plugins · Bulk actions_
- **Enable Jetpack to manage plugins** _(prerequisite)_: _"Jetpack required for plugin management" banner_

#### Manage a plugin site-by-site _(Build)_ — the expanded detail panel
> When I need fine control over one plugin, I want to manage it per site, so I can activate, update, or install it exactly where it's needed.
- **See where a plugin is installed**: _Open plugin (click title) → "Installed on N sites"_
- **Activate or deactivate per site**: _Active toggle_
- **Control autoupdate per site**: _Autoupdate toggle_
- **Update a plugin on a site**: _Update_
- **Install a plugin on more sites**: _"Available on" → Install_
- **Take other per-site plugin actions**: _Per-site kebab (e.g., remove)_

### Reports (Beta) (mapped as three major functions; all Grow)
_Two surfaces plus a flow: a discovery/marketing page that frames the problem and sells reporting (`/reports/overview`), a 3-step build-and-send wizard (`/reports/build`), and a dashboard of previously sent reports (`/reports/dashboard`). Only live WordPress.com or Pressable sites using Jetpack are supported. Sources: dashboard screenshots, `sections/reports/`._

#### Show clients the value of my work _(Grow)_ — the discovery page
> When my clients can't see the ongoing work I do behind the scenes, I want to prove my agency's impact with clear, professional reporting, so clients stay informed, confident, and invested in our relationship.
- **Understand why client reporting matters** _(New user)_: _"Why share reports?" content · View example report_
- **Start my first report**: _Build a new report_

#### Build and send a client report _(Grow)_ — the 3-step wizard
> When a reporting period has closed and a client expects an update, I want to assemble and send a polished report in a few guided steps, so the client receives a professional snapshot without me building it by hand.
- **Choose a site to report on**: _Step 1 · Choose a site to report on (live WP.com/Pressable + Jetpack only)_
- **Set the timeframe and recipients**: _Step 1 · Report date range · Client email(s) · Also send to your team_
- **Choose which stats to include**: _Step 2 · 8 stat options · Prepare report (more data types coming soon)_
- **Add a personal intro message**: _Step 2 · Intro message (optional)_
- **Preview before sending**: _Step 3 · Send me a preview_
- **Send the report to my client**: _Step 3 · Send to client now_
- **Schedule recurring report delivery** _(Upcoming)_: _Marketing copy only ("Coming soon"); no UI yet_

#### Track reports I've sent _(Grow)_ — the dashboard
> When I send reports to many clients over time, I want to see what I've sent, to whom, and when from one dashboard, so I stay on top of client communication and never lose track.
- **See all my reports by site**: _Reports Dashboard (site · report count · latest status · last generated)_
- **Review a site's report history**: _Open site → per-report status · timeframe · created · client emails_
- **Resend or send myself a copy**: _Send to client · Send me a copy_
- **Reuse a past report**: _Duplicate report → build flow pre-filled (only place to duplicate a prior report)_
- **Delete a report**: _Delete report (if already scheduled, may still go out)_

### Partner Directories (Tier-gated; mapped as two major functions; all Grow)
_Tier-gated: only Agency, Pro, and Premier Partners can apply. Two distinct features that share a messy IA: (1) **directory listing**: apply → complete a public profile → publish to the WordPress.com / WooCommerce.com / Jetpack.com / Pressable.com (+ VIP) directories; and (2) **lead matching** (Upcoming: feature-flagged + pilot agencies): an internal preferences profile that matches clients to agencies. Several fields (services, industries/business types, languages, min budget) are collected in both: consolidation candidates. Sources: dashboard screenshots, `sections/partner-directory/`, KB: agency-directory-listings._

#### Get my agency listed in partner directories _(Grow · Tier-gated)_ — apply → profile → publish
> When prospective clients can't find my agency among the WordPress/Woo/Jetpack/Pressable community, I want to appear in Automattic's public partner directories, so clients discover and trust my agency without me chasing them.
- **Discover & start the directory program** _(New user)_: _Overview onboarding card → Let's do it_
- **Share my expertise & apply** _(Step 1)_: _Edit expertise · Submit my application (services, products, directory choices, sample client sites, customer feedback)_
- **Track my application status per directory**: _Pending / Approved / Not approved · Update my expertise (on rejection)_
- **Complete my public profile** _(Step 2)_: _Finish profile · Save public profile (name, email, website, bio, location, logo, industries, services, products, languages, availability, min budget)_
- **Publish my profile** _(Step 3)_: _Publish · Done_
- **View & edit my live listing**: _Edit expertise · Edit profile · View your agency's profile (on each approved directory)_

#### Get matched with the right client leads _(Grow · Tier-gated · Upcoming)_ — lead matching preferences
> When I want a steady flow of clients that actually fit my agency, I want Automattic to match me to clients whose projects suit my strengths, so I receive qualified leads instead of chasing mismatched work.
- **Tell us my ideal client profile**: _Lead matching preferences (11-question form: regions/languages, business types & sizes, hosting/platforms, project types, budget/timeline, decision-making, site management)_
- **Set my availability for leads**: _Accepting new clients toggle → Eligible / Not eligible_
- **Save & stay eligible for leads**: _Save preferences · Update preferences_

### Team (mapped as one major function; Build)
_A simple area: manage who can access the agency dashboard and at what level. Two roles only (Agency owner vs Team member). Sources: dashboard screenshots, `sections/team/`, KB: team members._

#### Run my agency with a team _(Build)_ — members, invites, roles
> When my agency has more client work than I can manage alone, I want to bring teammates into the dashboard with the right level of access, so the right people can manage sites and referrals without handing over full control.
- **Invite a teammate**: _Invite a team member → Send invite (email or WordPress.com username + optional message)_
- **See who's on my team**: _Active members / Invited tabs (user · role · added; invite status)_
- **Manage a pending invite**: _Resend invite · Cancel invite (Invite pending / Invite expired)_
- **Control what a teammate can do**: _Agency owner vs Team member (members can't delete sites, remove payment methods, cancel/revoke licenses, or remove users)_
- **Remove a team member**: _Remove team member (requires a4a_remove_users)_
- **Hand off the agency**: _Transfer ownership (can't be undone; owner becomes a regular member)_
- **Leave an agency I'm part of**: _Leave agency (owner must re-invite; one dashboard at a time)_
- **Join an agency I'm invited to**: _Accept invite link → joins dashboard (one agency at a time)_

### Global (always-available; mapped as two major functions; Build)
_Actions a user can take from **any** page via the sidebar, not tied to one feature. Two entry points: the **avatar** (bottom-left) expands an account menu, and the **help icon** (bottom-right) toggles the Help Center. Not redundant: these are always-accessible utilities. Sources: dashboard screenshots, `components/sidebar/header/`._

#### Manage my account & profile _(Build · Global)_ — the avatar menu
> When I need account, profile, and support actions no matter where I am in the product, I want to reach them from the avatar menu on any page, so I can manage my relationship with the platform without hunting for settings.
- **Share feedback on the product**: _Provide feedback (modal; hidden for client users)_
- **Contact support**: _Contact support (modal; also reachable via Help Center)_
- **Read the Knowledge Base**: _View Knowledge Base ↗ (external)_
- **Manage my WordPress.com profile**: _Manage your profile ↗ (wordpress.com/me)_
- **Review the Platform Agreement**: _Platform Agreement ↗ (external)_
- **Sign out**: _Sign out_

#### Get help anytime _(Build · Global)_ — the help icon
> When I hit a question or problem while working anywhere in the product, I want to open help without leaving what I'm doing, so I find answers or reach support in context.
- **Open the Help Center**: _Help (?) icon → toggles Help Center panel (docs + contact support)_

---

## LAYER 3: Micro Functions
_Built last: granular tasks within each major function (e.g., add agency logo to a referral, remove a team member's access, modify and resend a client report)._

---

## CLIENTS (secondary user)
_The majority of this map is for **agencies** (our primary user). However, A4A also has to support the agency's **clients** in a limited capacity: primarily around product purchases (e.g., paying for a referral cart, completing checkout, managing a subscription the agency set up). This section holds the jobs that belong to the **client** as executor, kept separate from the agency jobs above._

_To be built: examples to validate: "When my agency sends me a cart of products my site needs, I want to pay for them quickly and securely, so I can get my site running without back-and-forth." Layers (functions / micro-tasks) for clients to follow._

---

## Sources
- [Automattic for Agencies: Home](https://automattic.com/for-agencies/)
- [A4A: Earn](https://automattic.com/for-agencies/earn/)
- Companion docs: `A4A-Layer-Foundation-Source.md`, `JTBD-Research-and-Framework-Context.md`
