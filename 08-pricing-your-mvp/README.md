---
title: "Chapter 8 — Pricing Your MVP"
nav_order: 8
---

# Chapter 8 — Pricing Your MVP

![Hero image — described in IMAGES_TODO.md](./assets/08-hero.png)

Pricing is where most non-technical founders panic. They've built a thing. Strangers are starting to use it. Now they have to put a number on it — and the number feels like an opinion they're about to share with the entire internet.

There's a reason this feels hard: pricing is half math, half psychology, and most founders haven't been taught either side. So they default to one of two failure modes: **price too low** ("I don't want to scare people away") or **don't price at all** ("free until we figure it out"). Both are mistakes that cost real money — sometimes for years.

This chapter is about how to set a real price on Day 1. Not a guess. A defensible number. One that proves your idea has value, attracts the right kind of users, and gives you the data you need to raise it later.

---

> **Quick answer:** Charge from day one. Even one paying user proves more than a hundred surveys. The fastest way to a defensible price: figure out **how much your product saves the user** in time or money, then price at **roughly 10% of that value**. Most B2B MVPs land at **$30–$200/month**. Most consumer tools at **$5–$15/month**. Avoid free-forever plans at MVP stage — they attract users who will never convert and dilute the signal you most need: are real people willing to pay you?

---

## Why charging from Day 1 matters

There's a temptation to "launch free, monetize later." Almost every founder considers it. Here's why it's almost always wrong:

**Free users aren't users.** They're a metric you can use to feel good. They tell you nothing about whether your product is actually valuable, because the threshold for "I'll click sign up" is much lower than the threshold for "I'll give you my credit card." A free user is a maybe. A paying user is a yes.

**Free attracts the wrong people.** Users who sign up for free apps tend to (a) churn within a week, (b) demand features as if they were paying, and (c) not refer others. Paying users are the opposite — they stick longer, give better feedback, and refer because they have skin in the game.

**Pricing is data.** Every conversion (or non-conversion) at your price point is a data point telling you whether your value proposition is real. You can't get that data without a price. Run free and you'll be flying blind for months.

**It's harder to raise prices than start at the right place.** Once you've trained users to expect free, charging later feels like a betrayal — even if you're charging modestly. Users churn, complain publicly, and the founder folds. Better to start with a real number and adjust if needed.

There are exceptions — viral consumer products, network-effect businesses, products where the free tier is the marketing — but if you're not certain you're one of those, you're not. Charge from Day 1.

## How to set your price (the value-based formula)

The single most useful pricing framework: **price as a function of the value you create.**

Step 1 — Figure out what your product is worth to the user, concretely. Not "we make their workflow better." Specifically:
- How many hours per week does the user save?
- How many dollars per month does the product save them, or earn them?
- What were they paying before — for the freelance fix, the broken alternative, or the time loss?

Step 2 — Multiply that value by ~10%. That's a defensible price.

**Example.** A bookkeeping tool that saves a small business 4 hours a week. The bookkeeper bills $50/hour. The product saves them $200/week, or roughly $800/month in billable time recovered. Ten percent of $800 = **$80/month**. That's a reasonable starting price.

**Example 2.** A consumer tool that helps writers organize research. It saves them maybe 2 hours a week of fumbling through Google Docs. Their time isn't billed, but they value it at maybe $25/hour. That's $200/month of value. Ten percent = **$20/month** — but consumer products generally price below B2B by a factor of 2–3x, so a more realistic landing is **$8–$12/month**.

The 10% rule isn't arbitrary. It's the rough threshold at which a customer feels like they're getting a *deal*, while you're getting paid enough to run a real business. Below 10%, customers don't perceive value (you're "too cheap to be real"). Above 30–40%, customers start hesitating ("hmm, do I really need this?"). Ten percent is the comfort zone.

## The four common MVP pricing models

Pick the one that matches your product. Don't invent a new one.

### Model 1 — Flat monthly subscription

**$X/month.** One price. One feature set. No tiers.

**Best for:** Most B2B MVPs. Simple. Predictable revenue. Easy to communicate.

**Real ranges at MVP stage:** $19, $29, $49, $79, $99/month. Round numbers work better than $24.99.

**Pros:** Simple. Conversion-friendly. Easy to project revenue.

**Cons:** You leave money on the table from power users who'd pay more. Easy to address later by adding a higher tier.

This is the right default. Start here.

### Model 2 — Tiered subscription (Free / Pro / Team)

A free tier with limits, a paid tier ($X/mo), and a team/enterprise tier ($X+ flat or per-seat).

**Best for:** Products that genuinely benefit from a freemium funnel — high-virality consumer apps, dev tools where the free tier is the marketing channel, products with strong network effects.

**Pros:** Lets users try before they buy. Captures different willingness-to-pay levels.

**Cons:** Most of your users land on free and stay there. Building three feature sets at MVP stage is over-scoping. **Avoid this at MVP unless your specific business model demands it.**

If you do go tiered, the rule is: free tier is *useful but limited*, paid tier is *what most users actually want*, team tier is *what real businesses want*. Don't make free useless (then no one signs up) or too good (then no one upgrades).

### Model 3 — Usage-based / metered

Pay per use. $0.01 per API call, $1 per generated report, $5 per gigabyte stored.

**Best for:** Infrastructure products, AI tools (where compute costs matter), products where customer value is directly proportional to usage.

**Pros:** Naturally aligns price with value. Power users pay more, casual users pay less.

**Cons:** Harder to predict revenue. Harder for users to budget. Confusing at the buy decision ("how much will I actually pay?").

If your product is AI-heavy and your costs scale with usage, this might be right for you. Otherwise, a flat subscription is simpler.

### Model 4 — One-time payment / lifetime deal

Pay once, use forever. $99, $299, $499 one-time.

**Best for:** Tools that don't have ongoing infrastructure costs, plug-ins, single-purpose utilities.

**Pros:** Easy buying decision. No churn to fight. Higher up-front cash.

**Cons:** No recurring revenue. Hard to predict business growth. Doesn't work for products with ongoing infra costs.

Some indie hackers run this model and do well — Tinybuild, Carrd, and many side-project tools. But for most SaaS MVPs, recurring is the right structure for a real business.

## What to put on your pricing page

Less than you think. The full template:

```
[Headline: One line that clarifies the value]
"$X/month — billed monthly" (or "billed annually, save 20%")

[3–5 bullet points of what's included — outcomes, not features]
[A primary CTA: "Start your trial" / "Book a demo" / "Sign up"]

[A small reassurance line: "Cancel any time, no questions asked"]

[An FAQ — 4–5 of the most common pricing questions]
```

That's it. No 5-tier comparison table. No "contact us" enterprise tier on Day 1 (you don't have enterprise customers). No "everything you need to scale to a billion dollars" promise.

Pricing pages are where over-design destroys conversion. Less is more.

## Should you offer a free trial?

Yes. With caveats.

**The right free trial:**
- 7–14 days, not 30. Most users decide in 48 hours; longer trials just delay the decision.
- No credit card required to start (this is the modern standard for MVPs).
- A built-in nudge to convert before trial ends — email reminder at Day 5, Day 7, Day 12.

**What to avoid:**
- Free-forever tier (different from a trial — see Model 2).
- Trials longer than 14 days. You're just postponing the no.
- Asking for a credit card to start. This kills sign-up conversion by 60%+ at MVP stage. Add it later, when your funnel is stable.

The credit-card-required vs. not-required debate has been settled by countless modern SaaS launches: at MVP stage, no card. Once you have brand and product-led growth working, you can switch and your conversion will be fine.

## How to handle "I want to talk to you before I pay"

Some users — especially in B2B — want a conversation before signing up. This is normal. Don't fight it.

The right structure:
- Pricing page lists your standard price clearly
- Add a small line: *"Have specific questions? [Book a call](#)"*
- The call link goes to your Cal.com (or similar) — 20-minute slots, free
- During the call, you don't negotiate the price. You answer their questions and let them sign up at the standard price afterward.

This converts better than offering "custom pricing" or hiding your prices behind a contact form. Real prices on the page + an option for a conversation = highest conversion.

## When to raise (or lower) your price

Founders ask this constantly. Here's the honest answer:

**Raise when:**
- You have 20+ paying customers and at least 10 of them say "honestly, you could charge more for this"
- Your conversion rate is high enough that you can absorb 20–30% fewer signups for higher revenue
- You add a major feature that materially expands what the product does

**Lower when:**
- (Almost never.) Lowering price rarely solves a conversion problem — usually the issue is positioning, audience, or product clarity.

If you're not sure whether to raise prices: try raising them for new customers only. Existing customers stay on the old price. If the new conversion rate stays similar, the new price is correct. If it drops too much, revert.

## The Basecamp lesson — flat pricing as a feature

Basecamp famously charges a single flat fee per company (not per user). Most B2B SaaS charges per seat. Basecamp's flat structure is *itself a marketing differentiator* — they tell prospects that with their pricing, you don't have to think twice about adding the entire team.

The lesson isn't "everyone should copy Basecamp's flat pricing." It's that **pricing structure is part of your product positioning.** When everyone in your category prices one way, pricing differently can become a strategic edge.

For most MVPs, though: do not innovate on pricing structure at Day 1. Pick a familiar structure (Model 1, flat monthly subscription) and a defensible price (the 10% rule). Innovate later, after you have data.

> **AI shortcut:** [Prompt It](https://promptit.app) → *"Apply the 10% value rule to my product. My product saves users [X hours/week] at an effective rate of [$Y/hour], OR my product earns users [$Z/month] in incremental revenue. Recommend 3 monthly subscription price points and explain when to pick each. Then write the pricing page copy."*

## Your Turn

This week. Get a real number on the page.

1. **Calculate the value you provide.** In dollars per month, per user. Be specific. *"This saves the user 4 hours a week at $50/hour, so $800/month of value."*

2. **Apply the 10% rule.** Land on a starting price. Don't agonize. Pick the round number nearest your calculation.

3. **Pick your pricing model.** Flat monthly. Done. (Don't pick anything else unless you have a specific reason.)

4. **Write your pricing page** using the template above. Headline, price, 3–5 bullets, CTA, reassurance, FAQ. Less is more.

5. **Decide on your trial.** 7-day or 14-day. No credit card required. Email reminders at Day 5/7/12.

6. **Test it on three real users.** Show them the pricing page. Watch their reaction. Ask: "Does this feel about right? Cheap? Expensive? Why?" Their faces tell you more than their words.

7. **Don't change the price for at least 30 days post-launch.** You need a stable price to read the data correctly. Resist the urge to A/B test pricing on day 5; you don't have enough volume yet.

When your pricing page is live and at least one person has paid you, move to Chapter 9.

## FAQ

<details>
<summary><b>What if no one converts at my price?</b></summary>

The problem is almost never the price. It's usually one of: (a) the value isn't clear (revisit your landing page from Chapter 7), (b) the audience isn't right (revisit Chapter 1 — are you actually talking to your target user?), or (c) the product isn't done enough (revisit Chapter 3 — is the core flow obvious?). Pricing is the last thing to debug. Founders blame it first because it's the easiest to change, but it's almost never the bottleneck.

</details>

<details>
<summary><b>What if my competitors are all cheaper?</b></summary>

Probably fine. Cheap is a race to the bottom. Most successful SaaS in the last 5 years priced *higher* than the existing market, then justified it with better value. Linear didn't undercut Jira; it priced similarly and won on quality. Notion didn't undercut Confluence; it priced similarly and won on flexibility. Compete on value, not on price.

</details>

<details>
<summary><b>Should I offer annual pricing?</b></summary>

At MVP stage, optional. The standard is to offer annual at 20% off the monthly rate. It improves cash flow and reduces churn. But it's not necessary for launch. Add it after your monthly price has proven stable.

</details>

<details>
<summary><b>What if my user can't pay credit card (e.g. enterprise procurement)?</b></summary>

For MVP stage, you're probably not selling enterprise. If you are, you'll need to handle invoices, ACH, NET-30, and procurement. Add Stripe Invoicing or use a tool like Pylon. But don't optimize for this at Day 1 — most MVPs land on credit card customers, and adding enterprise infrastructure prematurely slows you down.

</details>

<details>
<summary><b>How do I know my price isn't too high?</b></summary>

Watch the conversion rate from your pricing page. If less than 1% of qualified pricing-page visitors convert, the price might be too high *or* the value isn't clear. Check both. The honest test is: when you talk to a user who didn't convert, ask why. They'll tell you. Most "too expensive" objections are actually "I didn't understand the value" objections in disguise.

</details>

---

## Ready to Launch Your SaaS?

At [Pexa Studio](https://pexastudio.com) we help founders set their first price during the build, not as an afterthought. Stripe integration is baked into Day 15 of the 21-day cycle, so you're shipping a paid product, not a free one with "monetization to figure out later."

→ **[Book a free 30-minute intro call](https://cal.com/shakirdmr/free-intro-call)**

*Trusted by founders in US & Europe · 21 days · $3k–$6k · 100% code ownership*

---

← [Chapter 7: Launching to First Users](../07-launching-to-first-users/) · **Next:** [Chapter 9 — Closing Your First Paying Customer →](../09-closing-your-first-customer/)
