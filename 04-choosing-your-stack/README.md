---
title: "Chapter 4 — Choosing Your Stack"
nav_order: 4
---

# Chapter 4 — Choosing Your Stack (For the Non-Technical)

![Hero image — described in IMAGES_TODO.md](./assets/04-hero.png)

If you're non-technical, the word "stack" probably feels like the moment in a meeting where you politely nod while someone says "we'll just use a Postgres-Redis-Vercel-tRPC pipeline with edge functions and serverless caching." None of that means anything yet, and that's fine. By the end of this chapter, you'll know exactly which stack matches your MVP, why, and what you should pay for it.

Here's the bigger frame: **the stack you pick will determine whether you launch in 3 weeks or 3 months.** Not your idea. Not your team's talent. The tools.

A 2-person team in 2026 ships what a 10-person team shipped in 2019. That's not hyperbole — it's the consequence of how aggressively modern tooling has eaten manual work. The founders who win are the ones who understand which tools eliminate work, and pick those.

---

> **Quick answer:** For most non-technical founders building a SaaS MVP in 2026, the answer is one of three stacks: **(1) No-code** (Webflow / Bubble / Softr) for $50–$300/mo if your product is forms + simple workflows; **(2) Modern code stack** (Next.js + Supabase + Stripe + Vercel) if your product needs real logic, real-time data, or AI; **(3) Hybrid** (Webflow marketing site + custom backend) if you need a polished public site and a complex app. Pick based on your *product's* needs, not your *founder identity*.

---

## The "What Stack?" decision tree

Before we go deep on each option, here's the 60-second decision tree:

```
START — What does your product mostly do?

├── Mostly form-based or directory-style (e.g. a marketplace, a job board, a CRM)
│   → No-code stack (Webflow, Bubble, Softr, Glide)
│
├── Real-time updates, complex logic, AI, custom data structures
│   → Modern code stack (Next.js + Supabase + Stripe + Vercel)
│
├── A polished public site PLUS a custom application
│   → Hybrid (Webflow/Framer for marketing, code for the app)
│
└── Mobile-first or app-store-required
    → React Native + Supabase, OR Flutter + Firebase
```

That's the whole framework. Now let's go through each so you know what you're picking.

## Option 1 — The No-Code Stack

**Best for:** Marketplaces, directories, simple SaaS, internal tools, MVPs where the core innovation is in the workflow not the technology.

**Tools:** Webflow (site + light app), Bubble (full app), Softr (Airtable-based apps), Glide (mobile-first), Make/Zapier (automations), Stripe (payments).

**Cost:** $50–$300/month for tools. $0–$3,000 if you build it yourself, $1,500–$6,000 if you hire a no-code builder.

**Time to MVP:** 1–4 weeks.

**Pros:**
- Fast. Genuinely fast.
- You can edit and iterate without engineering help.
- Cheap to start.
- "Visual" feedback loop — you see what you're building.

**Cons:**
- Hits a ceiling. Once you have 5,000+ users or need complex logic, you'll likely re-platform.
- Performance can suffer at scale.
- You don't own the code. If Webflow disappears, your product disappears.
- Custom integrations get hacky.

**When it's the right call:** Your product is mostly a clever workflow on top of forms, payments, and basic data. You don't need real-time updates, sophisticated UI, or heavy AI. Examples: a creator's directory, a niche job board, an Etsy-style marketplace, an internal team tool, a beta course platform.

**When it's the wrong call:** You're building something with real-time chat, multi-user collaboration, complex data manipulation, or AI features. You'll fight the tool the entire time, and the result will be brittle.

**Pexa Studio note:** We *will* build no-code MVPs for the right product. If your idea fits this category, we'll often save you money by suggesting it instead of pushing a custom build. Stack should match the product, not the founder's ego.

## Option 2 — The Modern Code Stack

**Best for:** Real SaaS products, AI-enabled apps, anything with custom data, anything you expect to grow past a few thousand users.

**Tools:**
- **Next.js** (React-based framework) for the frontend and a lot of the backend
- **Supabase** (Postgres + auth + storage + realtime, all in one) — replaces what used to take 3 services
- **Stripe** for payments and subscriptions
- **Vercel** for hosting (deploy in 30 seconds, scales automatically)
- **Tailwind CSS** for styling
- **Resend** for transactional email
- **Posthog** or **Plausible** for analytics

**Cost (running):** $0–$50/month for an MVP with 100 users. $50–$300/month at 1,000 users. Stripe takes 2.9% + 30¢ per transaction.

**Cost (build):** $5,000–$30,000 with freelancers, $30,000–$150,000 with a traditional agency. **$3,000–$6,000 with a specialist 21-day MVP team like Pexa Studio.**

**Time to MVP:** 21–60 days depending on complexity and who's building.

**Pros:**
- You own the code. You can move it anywhere.
- It scales. The same stack runs Vercel itself, Linear, Loom, Cursor — products with millions of users.
- Modern tools have eliminated 80% of the boilerplate that used to slow this stack down.
- Real-time features, AI, custom logic — all native.

**Cons:**
- Requires either you knowing how to code OR a developer/agency partner.
- Setup costs more than no-code in dollars (less in time, when done right).
- More moving parts means more things that *can* break (though good defaults make this rare).

**When it's the right call:** Your product has real logic, real-time anything, or you expect to grow into a real software business. This is the right stack for >80% of MVPs we see.

**When it's the wrong call:** Your product is essentially "Airtable with a custom skin and a Stripe button." That's a no-code project.

## Option 3 — The Hybrid Stack

**Best for:** Founders who need a polished public site (for SEO and trust) plus a real custom application underneath.

**Tools:**
- **Framer** or **Webflow** for the marketing site (`yourcompany.com`)
- **Next.js + Supabase + Stripe + Vercel** for the app (`app.yourcompany.com`)

**Cost (running):** Webflow/Framer $20–$40/month + your code stack costs above.

**Cost (build):** Add ~$1,000–$3,000 to the code-stack price for the marketing site, or do it yourself in a weekend with a Framer template.

**Time to MVP:** Same as Option 2 for the app, plus 1–2 days for the site.

**Pros:**
- Marketing team (or you) can edit the site without bothering engineers.
- Site is fast and SEO-friendly out of the box.
- Best of both worlds: polished public face, real app behind it.

**Cons:**
- Two systems to maintain.
- Slightly more complex deployment story.

**When it's the right call:** You expect content marketing or SEO to be part of your acquisition strategy. You want to add new pages, blog posts, and landing pages weekly without an engineer involved.

This is, incidentally, what `pexastudio.com` itself runs on. Marketing site = Framer. Blog and dashboard = Next.js. Each tool doing what it's best at.

## What about Webflow vs Framer?

You'll see both. Quick decision:
- **Framer:** Better for design-forward, modern landing pages with animation. Easier to make beautiful. Younger ecosystem.
- **Webflow:** Better for content-heavy sites, blogs, larger sites with CMS. More mature SEO tooling. Bigger plugin ecosystem.

For an MVP marketing site under 20 pages, either is fine. Pick the one whose templates you find prettier. That's a real heuristic.

## What about other backends? (Firebase, AWS, etc.)

You'll hear advice to use Firebase, AWS, Convex, PlanetScale, Neon, and a dozen other options. Here's the honest take:

- **Firebase:** Mature. Works. But its data model (NoSQL) makes complex queries painful. Most founders eventually re-platform.
- **AWS:** Powerful, but a tar pit for non-technical founders. You'll spend 50% of your build time in the AWS console. Don't.
- **Convex / PlanetScale / Neon / etc:** All fine, none meaningfully better than Supabase for an MVP. Stick with Supabase to reduce decision fatigue.

The best stack is the one you don't have to think about. Modern Next.js + Supabase has won the "don't have to think about it" category for the moment. That'll change in 2 years and it won't matter, because by then you'll have revenue and a developer who can re-platform you.

## What about AI? Do I need OpenAI / Anthropic in my stack?

Only if your *product* needs AI to function. Don't add AI because it's hot. Add AI because your validation revealed that users would benefit from it.

If you do need AI:
- **Anthropic Claude API** for general LLM tasks (writing, summarization, agents, tool use)
- **OpenAI API** for transcription (Whisper) and image generation (DALL-E)
- **Replicate** for arbitrary open-source models you want to fine-tune

Cost: $20–$500/month for an MVP-scale product, depending on volume. Build into your pricing from day one.

## The "what should I pay" cheat sheet

This is the most-asked question in our intro calls. Here are real ranges, rounded honestly:

| Stack | DIY (your time) | Freelancer | Specialist (Pexa Studio) | Traditional agency |
|-------|-----------------|------------|--------------------------|--------------------|
| **No-code** | $0 (3–4 weeks) | $1,500–$6,000 (2–4 weeks) | $1,500–$3,500 (2 weeks) | $5,000–$25,000 (4–8 weeks) |
| **Code stack (MVP)** | Not realistic without coding skills | $5,000–$30,000 (2–6 months) | **$3,000–$6,000 (21 days)** | $30,000–$150,000 (3–6 months) |
| **Hybrid** | Not realistic | $7,000–$35,000 (3–6 months) | $4,000–$8,000 (21–28 days) | $40,000–$180,000 (4–6 months) |

A few things jump out from that table:

- **Specialists beat freelancers on price AND time** because they've built this exact thing 20+ times and know exactly which traps to avoid.
- **Agencies are 5–10x more expensive** without being 5–10x better. They have offices and overhead. You're paying for that.
- **Freelancers can be great**, but the variance is huge. The right freelancer is gold; the wrong one will leave you 60% built and unreachable.

This pricing is exactly why Pexa Studio exists. We saw founders quoted $30,000 for products we knew could be built in 3 weeks for $5,000, and it pissed us off enough to start a company. (See Chapter 1 — *problems you've felt*.)

## Linear's stack — a real example

Linear, the project-management tool worth ~$1B as of 2024, was built by a team of three. Their initial stack:

- Frontend: React (now Next.js)
- Backend: Node + GraphQL
- Database: Postgres
- Hosting: Vercel + their own infrastructure
- Realtime: Custom CRDT system (added later)

Three people. Modern stack. Shipped a product that beat companies with 100x the headcount, partly because they didn't waste time on infrastructure that didn't matter. They picked tools that let them focus on product.

The lesson isn't "use exactly this stack." It's *"a small, tight stack with modern defaults beats a sprawling stack with custom everything, every time."*

> **AI shortcut:** [Prompt It](https://promptit.app) → *"Walk me through the stack decision for my MVP. My product does [X]. My budget is [$Y]. My deadline is [Z weeks]. My technical skill level is [none/some code/full-stack]. Recommend exactly one stack from: no-code, modern code (Next.js+Supabase+Stripe+Vercel), or hybrid. Explain the tradeoff vs. the others."*

## Your Turn

This week. Before you start building.

1. **Run the decision tree.** What does your product mostly do? Forms-and-workflows? Real-time / custom logic? Marketing site + app?

2. **Pick your stack.** No-code, code stack, or hybrid. Don't agonize. Pick the one the decision tree pointed to.

3. **Estimate your build cost.** Use the cheat-sheet table. What's the realistic price for someone to build your MVP at the right quality?

4. **Compare to your budget.** If you have $1,000, you're DIY-no-code or you're not building yet. If you have $3,000–$6,000, a specialist is your sweet spot. If you have $30,000+, you have options — but ask yourself if 5x the budget actually buys you 5x the product.

5. **Make the decision.** Write it down. *"My MVP will be built on [stack], by [me / freelancer / specialist], for $[X], in [Y] weeks."* That's your build plan.

When the decision is made, move to Chapter 5.

## FAQ

<details>
<summary><b>Should I learn to code if I'm a non-technical founder?</b></summary>

Garry Tan's advice on this is unambiguous: yes, learn enough to be dangerous. You don't need to become a senior engineer. You need enough fluency that you can read code, evaluate technical hires, and not be at the mercy of a developer's word. A weekend with a JavaScript course gets you 80% of the way. You'll also have a much better feel for which features are easy and which are nightmares to build.

</details>

<details>
<summary><b>What about WordPress?</b></summary>

WordPress is great for blogs and content sites. It's not great for SaaS products. If your "product" is content + lead magnets, WordPress is fine. If you're building software, skip it.

</details>

<details>
<summary><b>Do I need TypeScript?</b></summary>

If you're using Next.js (which you should be, in the code stack), it comes with TypeScript by default and you should keep it on. TypeScript catches a category of bugs at write-time that would otherwise hit you at runtime. Worth the small upfront learning cost.

</details>

<details>
<summary><b>What about Ruby on Rails / Django / Laravel?</b></summary>

All viable. All slightly slower to ship in than Next.js + Supabase, in our experience, mostly because the surrounding ecosystems (deployment, auth, payments) require more wiring. If you have a developer who's a Rails expert, by all means use Rails. If you don't, default to Next.js + Supabase.

</details>

<details>
<summary><b>Is no-code "real" software?</b></summary>

This question is silly, but it gets asked. Companies running on Bubble have hit $1M+ ARR. The tool doesn't determine whether your business is real — your customers do. That said, most products that grow past 10,000 users eventually re-platform off no-code, because the ceiling is real. Plan for that future migration if no-code is your starting point.

</details>

---

## Ready to Launch Your SaaS?

At [Pexa Studio](https://pexastudio.com) we take non-technical founders from idea to live SaaS in **21 days**. Fixed price **$3k–$6k**. You own 100% of the code.

We default to the modern code stack — **Next.js + Supabase + Stripe + Vercel** — because it's the fastest path to a real, owned, scalable product. But if your idea is a better fit for no-code, we'll tell you that upfront. Stack matches the product.

→ **[Book a free 30-minute intro call](https://cal.com/shakirdmr/free-intro-call)**

*Trusted by founders in US & Europe · 21 days · $3k–$6k · 100% code ownership*

---

← [Chapter 3: Scoping Your MVP](../03-scoping-your-mvp/) · **Next:** [Chapter 5 — Designing for Clarity →](../05-designing-for-clarity/)
