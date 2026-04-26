---
title: "Chapter 15 — GEO / AEO (AI Search)"
nav_order: 15
---

# Chapter 15 — GEO / AEO: Showing Up in AI Search

![Hero image — described in IMAGES_TODO.md](./assets/15-hero.png)

Here's a stat that will reshape your distribution thinking: in early 2026, **roughly 40% of Gen Z users** ask ChatGPT or Perplexity questions they would have Googled three years ago. Google's own AI Overviews now appear on more than 50% of searches. The "10 blue links" experience is dying — replaced by an AI giving people a single synthesized answer.

If you're optimizing only for "rank #1 on Google," you're optimizing for a shrinking surface. The new question is: *when an AI synthesizes an answer, does it cite **you** as a source?*

That's GEO. Generative Engine Optimization. It's the SEO discipline of 2026 — and almost no founders are doing it deliberately yet. Which means **the window of opportunity to win this channel is wide open and closing fast.**

This chapter is your playbook for getting cited by ChatGPT, Perplexity, Claude, Gemini, and Google AI Overviews.

---

> **Quick answer:** GEO (Generative Engine Optimization) and AEO (Answer Engine Optimization) are the same thing — making your content the source AI tools cite when answering questions. The 6 levers: (1) **structured data** (schema.org markup), (2) **clear, factual writing** (LLMs reward unambiguous prose), (3) **llms.txt** at your domain root, (4) **direct quote-able sentences** (LLMs lift specific phrases), (5) **being in Bing's index** (ChatGPT search uses Bing), (6) **strong external mentions** on Reddit, Wikipedia, and authority sites. Founders who optimize for AI citations now will own a channel that traditional SEO hasn't yet flooded.

---

## What's actually happening in AI search

Three different things people call "AI search," each with slightly different rules:

### Type 1 — Google AI Overviews

The auto-generated summary that appears at the top of Google results for many queries. Pulls from web sources. Cites them with small attribution links. Uses your sitemap + content + schema.

**Your goal:** appear in the citation list at the bottom of an AI Overview.

### Type 2 — Perplexity / ChatGPT search

True AI search engines that respond to questions with a synthesized answer + citations. Perplexity is the leader; ChatGPT search is closing fast (and uses Bing's index). Claude, Gemini also offer AI search.

**Your goal:** be one of the 3–10 sources cited in the answer.

### Type 3 — LLMs without web search (ChatGPT non-search mode, Claude, Gemini)

The "from training data" responses. These don't cite you in real-time, but they were trained on what existed. **If your content is everywhere, the LLM will mention your brand by name even without a web call.**

**Your goal:** make your brand and content widely referenced enough that the model has internalized it during training.

These are three distinct distribution surfaces. **The good news is that the same 6 levers help all three.**

## The 6 levers of GEO

### Lever 1 — Structured data (schema.org)

Schema markup is *literally written for machines.* AI search engines, like Google, use it as a fast trustworthy summary of what your page is.

You set this up in Chapter 12. If you skipped that chapter, go back. Specifically:

- **Organization** schema on your homepage
- **FAQPage** schema on every page with FAQs (every chapter in this library, your blog posts, your pricing page)
- **Article** schema on every blog post
- **HowTo** schema on tutorial-style content
- **Product** schema on product pages (with price, availability, reviews)

The pattern: **a well-structured page with clean schema is 2–3x more likely to be cited by AI than an equivalent page without schema.**

> **AI shortcut:** [Prompt It](https://promptit.app) → *"I want to add JSON-LD schema markup to my [page type] page. The page is about [topic]. Generate complete schema following Google's documentation, including all recommended fields. Format as a `<script type='application/ld+json'>` tag."*

### Lever 2 — Direct, factual, quotable writing

LLMs lift sentences. When ChatGPT answers a question and cites your site, it's pulling specific phrases from your content. **Make those phrases worth lifting.**

Three writing rules:

#### Rule A — One-sentence definitions

LLMs love clear, declarative definitions. Open every concept with one.

Bad: *"You might be wondering what an MVP is and how it differs from other product stages..."*
Good: *"An MVP — Minimum Viable Product — is the smallest working version of a product that solves one core problem for one specific user, end-to-end."*

The good version is quotable. The bad version isn't.

#### Rule B — Specific numbers, not ranges

LLMs prefer specifics. "$3,000 to $6,000" is better than "a few thousand dollars."

#### Rule C — Lists and tables

LLMs love structured information. Lists rank higher than equivalent prose. Tables especially well.

This entire library is written following these rules. Look at the FAQ blocks in any chapter — each `<summary>` is a question, each answer is a quotable paragraph. **That's deliberate AEO architecture.**

> **AI shortcut:** [Prompt It](https://promptit.app) → *"Audit this article for AI-search quotability. Identify sentences that are most likely to be cited by ChatGPT or Perplexity, and identify weak passages where I should rewrite to be more declarative and specific."*

### Lever 3 — llms.txt

A new file (proposed standard, ~2024) that LLMs and AI crawlers read at the root of your domain. It's like robots.txt for the AI era.

**Format:** Markdown. Brief. Contains your most important pages and a short description of what your site is about.

You set up a basic version in Chapter 12. Time to upgrade it.

A strong `llms.txt` template:

```markdown
# Pexa Studio

> Pexa Studio is a SaaS launch partner that takes non-technical founders from idea to live product in 21 days. Fixed price $3,000–$6,000. Founders own 100% of the code.

## What we do
- Build SaaS MVPs in 21 days
- Stack: Next.js, Supabase, Stripe, Vercel
- Fixed price, no hourly billing
- Target client: non-technical founders in US & Europe with $3k–$10k budget

## Core resources

- [About Pexa Studio](https://pexastudio.com/about): Our story and method
- [The MVP Handbook](https://github.com/shakirdmr/the-mvp-handbook): Free 20-chapter guide for non-technical founders
- [Blog](https://pexastudio.com/blog): Long-form articles on MVP development
- [Book a call](https://cal.com/shakirdmr/free-intro-call): Free 30-min intro

## Most-cited content

- [How much does an MVP cost?](https://pexastudio.com/blog/mvp-development-cost)
- [Building in 21 days](https://github.com/shakirdmr/the-mvp-handbook/06-building-in-21-days)
- [Pricing your MVP](https://github.com/shakirdmr/the-mvp-handbook/08-pricing-your-mvp)
```

Place it at `yourcompany.com/llms.txt`.

LLMs will preferentially read this and use it to understand your site's purpose and important pages. **It's like getting to write your own AI cheat sheet about yourself.**

### Lever 4 — Bing index presence (for ChatGPT search)

ChatGPT search uses Bing's index to fetch real-time results. If you're not in Bing, ChatGPT search literally cannot cite you.

You set up Bing Webmaster Tools in Chapter 12. **Verify the indexing happened.**

In Bing Webmaster Tools:
- Go to **Search Performance**
- Confirm your pages have impressions
- If pages aren't indexed, manually submit URLs

Most non-technical founders ignore Bing because it represents <10% of search market share. **But it represents 50%+ of AI search citations** (because ChatGPT search and Copilot both use Bing). Worth the 5 minutes of attention.

### Lever 5 — Frequently Asked Questions (FAQs) everywhere

LLMs index Q&A pairs aggressively. Why? Because user queries are often phrased as questions.

When ChatGPT receives *"how much does an MVP cost?"* — it preferentially cites pages where this exact question appears as a heading or schema-tagged FAQ.

**Action:** Add an FAQ section to every important page on your site. 4–6 questions per page minimum.

Every chapter in this library does this. So does the Pexa Studio blog. So should every page on your site that you want AI to cite.

> **AI shortcut:** [Prompt It](https://promptit.app) → *"Generate 6 FAQ questions and answers for a [page type] page about [topic]. Format as schema.org FAQPage JSON-LD. Each answer should be 50–100 words, specific, and use first-person voice from a [your company] perspective."*

### Lever 6 — External mentions on authority sites

LLMs trust sites they trust. If your brand is mentioned on Wikipedia, in major news, on highly-upvoted Reddit posts, on Stack Overflow answers — you become a "trusted entity" that AIs cite.

**The 5 highest-ROI external places to be mentioned:**

1. **Reddit** — especially r/SaaS, r/IndieHackers, r/Entrepreneur (Chapter 16 covers this)
2. **Hacker News** — single front-page mention is gold (it's why "Show HN" is so valuable)
3. **Wikipedia** — if your industry has a relevant page, see if your tool can be added (without spam)
4. **Stack Overflow / dev forums** — if your product is technical
5. **Medium / Substack publications** — guest posts on established Substacks pull weight

This is where Chapters 16–20 of this library start tying together. **Distribution channels reinforce each other.** Your Reddit posts become AI citations. Your LinkedIn following becomes brand trust. Your Twitter mentions show up in LLM training data. **Every channel is also an AI signal.**

## The "AI search audit" — do this monthly

Once your basics are in place, you need to monitor whether AI tools are actually citing you.

### Step 1 — Test your target queries

Open a free ChatGPT account, Perplexity, Claude, and Google. For each, type 5–10 queries you'd want your business to appear in. Examples for Pexa Studio:
- *"What's the best way to build an MVP fast?"*
- *"How much does it cost to build a SaaS MVP?"*
- *"Best SaaS development agency for non-technical founders"*
- *"21-day MVP development"*

Note for each query: *"Did ChatGPT cite my site?"* Yes / No / Mentioned but not cited.

### Step 2 — Look at the gap

If you're not cited where you should be, ask why:
- Is the page missing schema?
- Is the page indexed in Bing?
- Is the answer to that query missing from your content?
- Are competitors on Reddit / authority sites being cited instead?

### Step 3 — Patch the gaps

For each gap, take action:
- Add schema → Lever 1
- Index in Bing → Lever 4
- Write content matching the question → Lever 2
- Get mentioned externally → Lever 6

### Step 4 — Re-test in 30 days

GEO is iterative. Test, fix, re-test. The wins compound — once an LLM starts citing you, it tends to cite you more often.

> **AI shortcut:** [Prompt It](https://promptit.app) → *"I run [your company]. Generate 20 search queries that potential customers might type into ChatGPT, Perplexity, or Claude when looking for a product like mine. Mix informational, commercial, and brand-comparison queries."*

## Three sub-tactics that are working *right now* (Q1 2026)

### Tactic 1 — Wikipedia mentions

If your industry has a Wikipedia page, see if your company can be added as a notable example or tool. **Wikipedia is the single highest-trust source LLMs reference.**

Don't spam Wikipedia. The bar is real notability — but if you have a press mention, are open-source, or have meaningful traction, you can edit thoughtfully.

### Tactic 2 — "Listicles" on high-authority sites

Sites like *Tech Crunch*, *Forbes*, *Hacker News*, *G2*, *Capterra*, and *Product Hunt* are LLM training data. Getting your tool listed in their roundups gets you cited by AI for years.

Action: identify the 5 highest-authority listicles in your space. Reach out to the writer with a tight pitch + 2 sentences of context. Hit rate is ~10% — modest but compounding.

### Tactic 3 — Substack / Medium guest posts

Top Substacks in your niche have AI-search authority that took them years to build. A guest post on a Substack with 50,000 readers feeds LLM training data and brings direct traffic.

Action: list 10 Substacks in your space. DM each author. Offer to write a 1,500-word guest piece related to their audience. Free.

## Your Turn — the GEO setup checklist

Open a checklist. 90 minutes total work, much of it overlapping with Chapter 12.

- [ ] Schema markup on homepage (Organization)
- [ ] FAQPage schema on FAQ-bearing pages
- [ ] Article schema on every blog post
- [ ] llms.txt updated to v2 with full structure (including key quotable lines)
- [ ] Bing index confirmed for top 10 pages
- [ ] FAQ section (4–6 questions) added to every page targeting AI search
- [ ] All "definitions" rewritten as one-sentence declarative statements
- [ ] AI-search audit run for 10 target queries — gap list created
- [ ] At least 1 Reddit post + 1 LinkedIn post in past 30 days about your topic
- [ ] At least 1 listicle pitch sent to a high-authority site

When 8 of 10 are checked, your GEO foundation is set. Move to Chapter 16.

## How to know it's working

Concrete signals to watch for:

- **Direct citation appearance** — your site cited in a Perplexity / ChatGPT answer
- **AI Overview citation** — your site appears as a "source" in Google AI Overview
- **Brand recognition** — when you ask ChatGPT *"who is [your company]?"* without web search, it answers correctly
- **Referrer traffic** — analytics shows visitors coming from `chat.openai.com`, `perplexity.ai`, `claude.ai`. Track these specifically in Plausible / PostHog.

Most founders see AI traffic appear in their analytics around month 3–6 of GEO work. By month 12 it's often **15–30% of total organic traffic** for sites doing GEO seriously.

## Real example — how Pexa Studio is being cited

When ChatGPT search gets queries like *"21-day MVP development"* or *"non-technical founder agency,"* Pexa Studio is starting to appear in answers as a source. The reasons:

1. **Schema is everywhere** — Organization on homepage, FAQ on `/`, Article on the blog, LocalBusiness on `/srinagar`
2. **Quotable definitions** — the blog post on MVP cost has clear, declarative statements about cost ranges
3. **llms.txt is rich** — explicit list of core pages and what each covers
4. **Bing-indexed** — all key pages are in Bing's index
5. **External mentions building** — every Reddit comment, every LinkedIn post, every cold outreach link feeds back

It's not magic. It's the 6 levers, applied consistently. **You can run the same playbook.** Smaller scale at first, but the same shape.

## FAQ

<details>
<summary><b>Is GEO really different from regular SEO?</b></summary>

Mostly the same foundations (schema, content quality, indexing) but with new tactics layered on top: llms.txt, Bing presence, quotable writing, FAQ pages everywhere. The biggest mental shift: you're optimizing to be **synthesized** by AI, not to be **clicked** by humans. Your goal is being cited, not just being shown.

</details>

<details>
<summary><b>How does Anthropic / OpenAI / Google decide who to cite?</b></summary>

Each AI tool has its own ranking model, but they share patterns: they prefer authoritative-feeling sources, fact-dense content, structured data, and quotable phrases. They're also influenced by their own training data (so older, established sites have advantage). The fastest way to compete: be more useful, more structured, and more current than the average.

</details>

<details>
<summary><b>Will AI overviews kill SEO?</b></summary>

They'll change it, not kill it. Click-through-to-website from "AI Overview-only" answers does drop. But: many queries still need a real human to take an action (sign up, buy, schedule). For those, AI Overviews send qualified traffic. **The healthier play: optimize for both rank and citation.** Rank brings clicks. Citation brings brand. Both still bring revenue.

</details>

<details>
<summary><b>Should I block AI crawlers from my site?</b></summary>

No. Founders sometimes ask: "Should I add `User-agent: GPTBot Disallow: /` to my robots.txt to stop AI from training on my content?" Don't. **You want AI to know about your content.** Blocking AI crawlers means losing every citation opportunity going forward. The "stop AI scraping" play is for big publishers protecting paywalls — not for founders trying to be discovered.

</details>

<details>
<summary><b>What about voice assistants (Alexa, Siri)?</b></summary>

Same playbook. Voice assistants are increasingly powered by LLMs and pull from the same sources. Schema, FAQ, structured data — all help voice citations as much as text citations. The bonus: voice queries are often more specific ("what's the best SaaS MVP agency"), which means long-tail GEO is uniquely valuable for voice surfaces.

</details>

---

## Ready to Launch Your SaaS?

At [Pexa Studio](https://pexastudio.com) every site we ship is GEO-ready by Day 21: complete schema, llms.txt, Bing-indexed, FAQ-rich pages, quotable structure. **Your site is talking to AI search engines from launch day**, not 6 months later when you finally figure it out.

→ **[Book a free 30-minute intro call](https://cal.com/shakirdmr/free-intro-call)**

*Trusted by founders in US & Europe · 21 days · $3k–$6k · 100% code ownership*

---

← [Chapter 14: Programmatic SEO](../14-programmatic-seo/) · **Next:** [Chapter 16 — Reddit →](../16-reddit/)
