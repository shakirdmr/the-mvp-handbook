---
title: "Chapter 3 — Scoping Your MVP"
nav_order: 3
---

# Chapter 3 — Scoping Your MVP

![Hero image — described in IMAGES_TODO.md](./assets/03-hero.png)

If Chapter 1 was about picking the right problem, and Chapter 2 was about confirming the problem is real, this chapter is about the brutal arithmetic of what to actually build.

It's the chapter most founders ignore. They spend two weeks validating, get excited, then immediately scope a product with 19 features because *"users said they wanted X, Y, and Z, so we should include all three."* Three months later they haven't shipped anything, and the original window of opportunity is gone.

This is the single most important chapter in the entire library. **Scope is the only real lever a founder has.** Get it right and you're shipping in 21 days. Get it wrong and you're shipping in 9 months — by which point you'll have spent 3x your budget, your co-founder will be exhausted, and the market will have moved on.

---

> **Quick answer:** Your MVP should have **3–4 features, max.** It should solve **one specific problem** for **one specific user**, in a way they can use end-to-end on day one. Anything else is scope creep, and scope creep is the leading cause of dead startups. The right MVP makes you slightly embarrassed when you launch it. If you're not embarrassed, you waited too long.

---

## What an MVP actually is (and isn't)

The term "MVP" gets misused so badly it's almost lost meaning. Let's reset.

**An MVP is the smallest version of a product that solves one core problem for one specific user, end-to-end.**

Read that twice. Three things in there matter:

1. **One core problem.** Not "many problems." The single most painful one your validation revealed.
2. **One specific user.** Not "everyone." The narrowest profile of the person you talked to in Chapter 2.
3. **End-to-end.** They can use it from start to finish without you holding their hand.

What an MVP is *not:*

- A prototype (prototype = something to look at, MVP = something to use)
- A landing page (that's a marketing test, not a product)
- A "version 1" that has all the features you eventually want, but uglier
- "Everything I imagined, minus the AI integration we'll add later"

Sam Altman opened Stanford CS183B Lecture #1 with a line that cuts through all this: *"It's better to make a small number of users love you than a large number of users like you."* You can't make anyone love anything that does six things half-well. You can make someone love something that does **one thing exceptionally**.

## Why founders overbuild (and why it kills them)

Three failure modes drive 90% of MVP scope creep:

### Failure mode 1 — "But what if a user wants X?"

You've watched a single demo from a competitor, or talked to one user who mentioned an edge case, and now feature X feels essential. It isn't. Users don't churn over missing edge-case features. They churn over a confusing core experience.

**Fix:** Maintain a "v2" doc. Every feature you cut goes there, not into the trash. You're not killing the feature; you're scheduling it for after revenue exists.

### Failure mode 2 — "We need to look professional."

Founders spend two weeks making a settings page beautiful before anyone has even signed up. Or they build a pricing page with three tiers when they don't have one paying user. Polish is a way of avoiding the harder work of getting users.

**Fix:** Anything that doesn't move a user from "stranger" to "uses the core feature" can be cut. If your settings page can be a dropdown with three options, do that. Polish is post-PMF.

### Failure mode 3 — "If we're going to bother building it, we should build it right."

This is the most seductive trap because it sounds responsible. *"Let's set up SSO from day one. Let's add team accounts now since we'll need them eventually. Let's use a proper queue system because what if it scales?"*

You're not going to scale before you have users. You're going to spend three weeks setting up infrastructure for a problem you don't have.

**Fix:** Build for tomorrow. Not for the future. Solve the problem you have now, with the simplest tool that works. You can always add complexity. You can rarely *remove* it.

## The 3–4 feature rule (and how to find yours)

Here's the test: at the end of validation, your users described **a workflow that goes wrong.** Map that workflow. Identify the exact step (or two steps) where it breaks down. Build features that fix only those steps.

**Example.** Let's say your validation revealed that small bookkeepers waste 4 hours a week reconciling invoices across QuickBooks, email, and Slack. Their workflow looks like this:

1. Get invoice via email
2. Forward to client for approval
3. Wait for approval
4. Manually enter into QuickBooks
5. Mark as approved in Slack
6. Follow up if approval is delayed

Where does it break? Steps 3 and 6. Approval and follow-up are killing them.

**Your MVP, then, is:**
- Forward invoice → auto-creates a one-click approval link for the client (Feature 1)
- Auto-reminder email after 48 hours of no response (Feature 2)
- Approval triggers auto-creation in QuickBooks (Feature 3)

That's it. Three features. The bookkeeper saves 4 hours a week. They will pay you. **You did not need a dashboard. You did not need analytics. You did not need user roles. You did not need dark mode.** All those things are post-MVP.

## The Loom example — single-feature beat full-product

Loom started in 2015 as a Chrome extension that did exactly one thing: record your screen and your face at the same time, then give you a shareable link. That's it. No editing tools. No teams. No analytics. No commenting. **One feature.**

The reason it took off wasn't because Loom built more than competitors — it was because Loom built **less, but in the exact spot users felt pain.** Existing screen recorders were either bloated (heavy desktop apps) or too primitive (no link sharing). Loom solved the workflow gap with one focused feature, then earned the right to add the rest *after* people were already using it.

By the time Loom added comments, teams, and editing — they had millions of users telling them exactly what to build. **They didn't have to guess on v2 because v1 had earned them a real audience.**

That's the whole game. Ship the one feature that makes someone love you. Earn the data to ship v2. Ship v2 confidently. Repeat.

## How to scope: the 3-pass cut

Here's the exercise. It works. Do it tonight.

### Pass 1 — Brainstorm everything

Write down every feature you've ever imagined for this product. No filtering. Sketches, half-thoughts, "wouldn't it be cool if" — all of it. You'll typically end up with 15–30 items.

### Pass 2 — Cut to 7

For each feature, ask: *"Does this directly fix the painful workflow step my users described in validation?"* If the answer is no, move it to your v2 list. If the answer is "kind of" or "indirectly," also v2.

You'll be left with about 7 features. Be ruthless. The list always wants to be longer than it should be.

### Pass 3 — Cut to 3 or 4

Now do the harder cut. From your 7, ask: *"Could a user accomplish their core goal without this feature?"* If yes, v2.

What survives is your MVP. Three or four features. End-to-end. One user, one workflow, one painful problem solved.

If you have five features and can't get to four, the problem is usually that two of them are actually one feature in disguise. Combine them.

If you have eight and can't get below seven, **you are not yet at MVP scope**. Go back to validation. You probably don't have a clear enough picture of which workflow step is the most painful. You're trying to solve the whole workflow.

## The "embarrassment test"

Reid Hoffman's famous line: *"If you are not embarrassed by the first version of your product, you've launched too late."*

This isn't a slogan. It's a calibration tool. When you imagine launching your scoped MVP, do you cringe slightly? Do you think *"oh god, what if a user notices it doesn't have [X]?"* — that's the right amount of embarrassment.

If you imagine launching and feel *proud* of the product, you've over-scoped. You've polished things that didn't need polishing. You've added features for credibility, not for users. Cut more.

The only correct emotional state at launch is mild dread, immediately followed by relief that it's out the door.

## What to put on your "v2 list"

Everything you cut goes here. Be generous to it — most of these features will eventually matter. Just not now.

A typical v2 list at the scoping stage:
- Settings page beyond the basics
- Team accounts and roles
- Analytics dashboard
- Email notifications beyond the critical one
- Onboarding tour / product walkthrough
- Public API
- Integrations beyond the one most-requested
- Multiple pricing tiers
- Mobile app
- Dark mode
- White-labeling

If you build any of these in your MVP, you're stealing time from the 3 features that actually move someone from stranger to fan. Don't.

## How this maps to a 21-day build

Three to four features is the exact scope a focused MVP team can ship in 21 days. Here's roughly how the math works:

- **3 days** — design and architecture (what does the user see, what's behind it)
- **2 days** — auth, account creation, the basic skeleton
- **3–4 days per core feature × 3** — the actual feature work
- **2–3 days** — polish, payments, deployment, the launch checklist

It adds up. If you scope to 6 features, the math becomes 30+ days, plus the inevitable 30% slip every project has. Now you're shipping in week 6 instead of week 3. Now you're paying double. Now you're losing motivation.

This is, incidentally, what we do every day at [Pexa Studio](https://pexastudio.com). The reason we can promise 21 days is not magic — it's that we've been ruthless about scope on the founder's behalf. **Most founders aren't great at cutting their own ideas.** A specialist partner will tell you, in the first call, which 3 features actually matter. That conversation alone saves most founders 3 months and $20,000.

> **AI shortcut:** [Prompt It](https://promptit.app) → *"I have a list of 20 features I want in my MVP: [paste]. Help me ruthlessly cut to 3–4. For each one I should keep, explain why. For each one I should cut, explain which user goal it doesn't directly serve. Be brutal — assume scope creep is the default failure."*

## Your Turn

This week. Before you write a line of code or hire anyone.

1. **Write the workflow.** In one paragraph, describe how your target user currently deals with the problem you're solving. What do they do today? What breaks? Where's the worst friction?

2. **Identify the 1–2 broken steps.** Highlight the moments in their workflow where things go wrong. These are the only places your product needs to insert itself.

3. **Brainstorm every feature you've imagined.** No filter. Get to 20+ items.

4. **Do the 3-pass cut.** Trim to 7. Then to 3–4. Move everything else to a `v2.md` file. Don't delete it — schedule it.

5. **Name your MVP.** In one sentence, complete this: *"A [tool/app/service] that lets [specific user] do [one thing] without [the friction]."* Example: *"A Chrome extension that lets bookkeepers send one-click invoice approvals without copy-pasting into QuickBooks."*

6. **Run the embarrassment test.** Imagine launching this. Do you feel mild dread? Good. Do you feel proud? Cut another feature.

When you have your scoped MVP, move to Chapter 4.

## FAQ

<details>
<summary><b>What if my market really does need 5+ features to launch?</b></summary>

It doesn't. Every founder thinks this. The market doesn't need 5 features — *you* think it does because you're imagining the full product. Look at the most successful SaaS launches in the last 10 years and find one that launched with more than 4 core features. You won't. Linear launched with one (issue tracking). Notion launched as a glorified note-taker. Stripe launched with 7 lines of code.

</details>

<details>
<summary><b>What if a user demands a feature I've cut?</b></summary>

Add it to v2 immediately and tell them. *"That's a great suggestion — we're tracking it for v2 and you'll be the first to know when it ships."* Most users are fine with this. The ones who aren't probably wouldn't have stuck around anyway. Don't promise to add features in v1 to win one user — you'll burn the launch trying to keep that promise.

</details>

<details>
<summary><b>What about the table-stakes features (login, settings, etc.)?</b></summary>

Those aren't features. Those are infrastructure. Login, basic account settings, password reset — these don't count toward your "3–4 features." They count toward your scaffolding. Use a template, copy from a starter kit, or use a SaaS like Clerk or Supabase Auth that gives you all of them in 30 minutes.

</details>

<details>
<summary><b>How do I handle requests for "team accounts" or "enterprise features"?</b></summary>

Politely defer. Single-user MVPs validate problems faster than team-based MVPs. Team features add a 30%+ complexity tax. If your buyer is a manager who needs team accounts to even consider buying, you have a B2B problem and should reread Chapter 2 with that in mind. Otherwise, single-user first, always.

</details>

<details>
<summary><b>I've already built more than 4 features. What now?</b></summary>

You have two options. Option 1: keep building, ship the bloated version, and accept that you've spent 2x as long as you needed to. Option 2: rip the extra features out, hide them behind a feature flag or a separate route, and launch the leaner version. Option 2 is almost always the right move — the extra features don't disappear, but they don't slow your launch either.

</details>

---

## Ready to Launch Your SaaS?

At [Pexa Studio](https://pexastudio.com) we take non-technical founders from idea to live SaaS in **21 days**. Fixed price **$3k–$6k**. You own 100% of the code.

The reason we can promise 21 days is exactly because of this chapter. Most of our intro calls are spent helping founders cut their feature list from 12 down to 3. That's the conversation that saves people three months and $20,000.

→ **[Book a free 30-minute intro call](https://cal.com/shakirdmr/free-intro-call)**

*Trusted by founders in US & Europe · 21 days · $3k–$6k · 100% code ownership*

---

← [Chapter 2: Validating Before You Build](../02-validating-before-building/) · **Next:** [Chapter 4 — Choosing Your Stack →](../04-choosing-your-stack/)
