---
title: "Chapter 5 — Designing for Clarity"
nav_order: 5
---

# Chapter 5 — Designing for Clarity, Not Beauty

![Hero image — described in IMAGES_TODO.md](./assets/05-hero.png)

Founders new to product-building have a recurring pathology around design: they think pretty equals professional, and ugly equals unfinished. So they spend two weeks of a 21-day build cycle picking gradients, choosing fonts, and arguing about button shadows.

That entire two weeks is wasted.

Your MVP doesn't need to be pretty. It needs to be **obvious.** Users don't churn on a v1 because the navigation isn't beautiful — they churn because they couldn't figure out what to do in the first 30 seconds. Beauty is a luxury you earn after 100 paying users tell you the product solves their problem. Clarity is non-negotiable from day one.

This chapter is about how to design an MVP that gets out of the user's way, so they can have the experience that makes them love the product.

---

> **Quick answer:** An MVP's job, design-wise, is to **make the next action obvious.** Not to be beautiful, not to be on-trend, not to demonstrate your taste. Use a clean default style, follow conventions users already know, and remove every element that doesn't push someone closer to the core action. The right level of design is "boring but obvious." If your screen makes a user pause for 3 seconds to figure out what to do, you've failed at design — even if it looks like Stripe's homepage.

---

## The Kevin Hale framework

Kevin Hale, partner at YC, gave Stanford CS183B Lecture #7 — *"How to Build Products Users Love."* Buried in a great talk is a framework most founders ignore:

**Users love products that are reliable, usable, pleasurable — in that order.**

- **Reliable:** It works. Every time. No bugs in the core flow. No 500 errors. No "wait did I lose my data?" moments.
- **Usable:** They can figure out what to do without asking for help.
- **Pleasurable:** It feels nice. The fonts are pleasant, the animations are subtle, the colors are tasteful.

The hierarchy matters. **Reliable beats usable beats pleasurable.** A pleasurable product that's unreliable is worse than a reliable product that's plain. Users will tolerate ugly far longer than they'll tolerate broken.

For an MVP, you should be at "reliable + usable" and skip "pleasurable" entirely. Pleasurable comes in v2, after you have enough users to know what they actually like.

## Why "ugly works" — Craigslist economics

The most-used classifieds site in the United States, for two decades running, has looked like this since 1996: blue links, white background, no images, no design. **Craigslist prints money.**

There are roughly two reasons:

1. The site is **fast.** No animations, no 3MB hero videos, no React hydration delays. Pages load instantly. On bad internet (which is most internet, globally), Craigslist works.
2. The site is **obvious.** You arrive, you see categories, you click. There's no design hiding the function.

Modern startups would call this "a UX nightmare." Craigslist would call it "still profitable in 2026 with a six-person team."

The lesson isn't *"never design anything."* The lesson is that beautiful design is a feature, not a foundation. **The foundation is making the next action obvious.** Craigslist does that perfectly. Your MVP needs to do the same — even if it ends up looking nicer than Craigslist (it should).

## The three rules of MVP design

These are the only design rules that matter pre-PMF. Memorize them.

### Rule 1 — One primary action per screen

Every screen has *one thing* the user is supposed to do. That thing should be the most visually prominent element on the screen. A bold button, a clear link, a single input — whatever the action is, it's the loudest thing.

If you have two buttons of equal weight on a screen, you've already failed. The user is now choosing between two things, which means their brain is consuming cognitive load that should be spent on the actual task.

**Test:** Show your screen to someone who's never seen the app. Ask them: *"What would you click first?"* If they hesitate or get it wrong, redesign the screen.

### Rule 2 — Steal conventions, don't invent them

Every common interaction pattern has a default. Sign-up forms go on the right side. Navigation goes on the top or left. Settings have a gear icon. Logout is in the top right. Search has a magnifying glass.

Founders sometimes feel that following conventions makes them "uncreative." It doesn't. It makes them clear. Users don't want to learn your app's special way of doing things — they want to do their job and leave.

**Steal liberally from products your users already use.** If your users live in Notion, your sidebar should look like Notion's sidebar. If your users live in Stripe, your dashboard should look like Stripe's dashboard. Familiarity isn't theft; it's UX.

### Rule 3 — Remove until it hurts, then add back one thing

The default state of any screen, page, or component should be **the absolute minimum.** Then, only add elements when you can justify why they're there.

A typical founder builds a sign-up screen and adds: a logo, a tagline, a hero image, a feature list, three social-login options, an email input, a password input, a "remember me" checkbox, a "forgot password?" link, a sign-up button, a "by signing up you agree to..." line, footer links, a chat widget, and a cookie banner.

A good founder builds the same screen with: a tiny logo, an email input, a password input, a sign-up button. Sign-in goes on a separate page. Forgot password is reachable from sign-in.

The user knows what to do in 0.5 seconds. That's the whole goal.

## What "good enough" looks like

Founders panic about design because they don't have a target. They assume they need to be Linear or Stripe-quality. They don't. Here's what "good enough" actually means at MVP stage:

✅ **Layout is grid-based.** Things line up. No random margins.
✅ **One typeface, two weights.** Inter or Geist or whatever — pick one. Use 400 (regular) and 600 (semi-bold). Done.
✅ **A small color palette.** One brand color, one neutral (grayscale), one alert color (red or amber). That's it.
✅ **Whitespace.** Pad your elements. Cramped layouts read as amateur. Generous whitespace reads as intentional, even with no other design.
✅ **No two competing styles.** Don't mix sharp corners with rounded corners. Don't mix flat with shadowed. Pick one and commit.

That's the whole bar. If your MVP hits these five things, you're at "good enough" design — and **good enough is the right place to be at v1.**

## Where to find your starting design

You're not designing from scratch. You don't have time, and you probably don't have the skill. Here are your options, fastest to slowest:

### Tailwind UI templates

If you're on Next.js + Tailwind, Tailwind UI ($300 one-time) gives you 500+ pre-designed components — sign-up forms, dashboards, marketing pages, settings panels. Drop them in, change colors, ship. Saves you ~20 hours.

### Shadcn/UI

Free. Pre-built React components with sensible defaults. Beautiful out of the box. Used by half the modern indie SaaS in 2026. If you're using Next.js, you almost certainly want this.

### Free Figma community files

Search Figma Community for your product type ("dashboard," "saas landing page," "onboarding flow"). Hundreds of free, pixel-perfect templates that you can reference for layout and steal patterns from.

### Hire a junior designer for a week

If you have $500–$2,000, a junior designer on Upwork can take your scoped MVP and deliver a clean Figma file in 5–7 days. They're not going to ship a Stripe-quality product, but they'll save you from your own design instincts.

### Use Pexa Studio's defaults

If you're working with us, design comes baked into the 21-day build. We use a tested, unflashy design system that converts well, and we customize it to your brand without inventing fragility. You don't need to make any design decisions yourself.

## The "five-second test"

Once your MVP design is built, run this test before launch:

1. Open your app on a fresh browser (or a friend's screen).
2. Show the screen for **five seconds**, then close it.
3. Ask: *"What do you think this app does? What were you supposed to do on that screen?"*

If they can answer both questions correctly, your design is doing its job. If they can't — even if the screen is beautiful — you have a clarity problem.

Run this test on your three most-important screens: the landing page, the first screen after sign-up (onboarding), and the screen where the core action happens.

You'll probably fail the first time. Iterate. Most clarity problems are solved by **removing things**, not adding things.

## Design mistakes that cost MVPs their launches

Things we see kill MVPs over and over:

- **Carousel hero on the landing page.** Users don't engage with carousels. Pick one message, make it loud.
- **Modal popups for newsletter signup before the user has even read your home page.** Annoying. Aggressive. Skip.
- **Custom fonts that take 4 seconds to load.** Use system fonts or one Google Font. Done.
- **Dark mode on day one.** Real, but: you're now designing two products. v2 problem.
- **Multi-column dashboards with 40 metrics.** A v1 dashboard should have 2–3 metrics, max. Add the rest after users tell you they want them.
- **A hamburger menu on desktop.** No. Show your nav. Hidden navigation is the leading cause of "I didn't know that feature existed."
- **Animations on every interaction.** Animation should be reserved for moments where it provides feedback or guides attention. Animating everything is the visual equivalent of a friend who won't stop talking.

If you find yourself debating any of these, default to the *less* version. Less animation. Less popup. Less carousel. Less custom-font. **Less is the right answer at MVP.**

## Real example — Notion's first 6 months

Notion launched in 2016 with what was, by 2026 standards, an extremely plain interface. White background. Slate gray text. One brand color (a very subtle pale yellow, mostly used for highlights). No animations. No flourishes.

What Notion got right wasn't visual flourish. It was **clarity of action.** Every page had one thing you could do: type. Every block was a building block, and the system for inserting blocks was the same everywhere. The brilliance was in the consistency, not the aesthetic.

Six years later, Notion's design has barely changed. They still use the same plain palette. The same sober typography. The product is now used by tens of millions of people, and Notion's design philosophy — *clarity, consistency, restraint* — has become an industry reference.

The takeaway: their design wasn't unfinished. It was finished in the most important way. Pretty, but not at the cost of clear. **You don't have to choose ugly to be clear** — but if forced to choose between *pretty-but-confusing* and *plain-but-obvious*, always choose plain-but-obvious.

> **AI shortcut:** [Prompt It](https://promptit.app) → *"Audit my UI mockup for the 'next action' rule. For each screen, identify: (1) what is the primary user action, (2) is it the visually loudest element, (3) what should I remove to make it more obvious? Be ruthless about cutting decoration."* Paste your screenshot or describe each screen.

## Your Turn

This week. Before you finalize any UI.

1. **Write your "next action" for each screen.** Open a doc. List every screen in your MVP. For each, write one sentence: *"On this screen, the user is supposed to [do X]."* If you can't articulate the action in one sentence, the screen isn't ready.

2. **Audit your designs for that one action.** Open your wireframes (or your half-built UI). For each screen, ask: *"Is the next action the visually loudest thing here?"* If not, redesign until it is.

3. **Pick your design system.** Tailwind UI, Shadcn/UI, a Figma template, or a designer. Don't hand-roll. Decide today which tool/template/source you're starting from.

4. **Run the five-second test.** On three screens. With three different friends. Don't argue with their feedback — when three strangers all say "I'm not sure what to do," you have a problem worth fixing.

5. **Ship the simpler version.** Whatever your current design has, remove three things. Replace nothing. The simpler version is almost always closer to the right one.

When your designs pass the five-second test, you're ready for Chapter 6.

## FAQ

<details>
<summary><b>What if I'm a designer myself?</b></summary>

Then you have an unusual advantage and an unusual risk. The advantage: you can craft a beautiful product. The risk: you'll over-design. Designer-founders are notorious for shipping pixel-perfect MVPs that took 2 months when a "good enough" version would have shipped in 3 weeks. Set yourself a hard time limit on design (3 days max, ideally). Iterate visually post-launch.

</details>

<details>
<summary><b>Should I hire a designer for my MVP?</b></summary>

For most MVPs, no. A clean design system + 5 hours of your own arrangement gets you a clear, professional-feeling product. Hire a designer when (a) your differentiation is design itself, (b) you've already validated the product, or (c) you have budget to spare and want a small head start on visual polish. Don't hire one for v1 because you "feel like you should."

</details>

<details>
<summary><b>Does design even matter for B2B / enterprise products?</b></summary>

Less than for consumer, but yes. Enterprise users have switched in the last 5 years from "I'll tolerate ugly because the company forces me to" to "I will quietly ask my manager to switch us off this if it's painful to use." The bar is lower than consumer-grade beauty, but the bar for *clarity* is the same.

</details>

<details>
<summary><b>What about animations and microinteractions?</b></summary>

Use them sparingly, and only where they communicate something. Loading state? Yes. Successful action? Sure, a tiny check animation is fine. Page transition? Maybe. Decorative animation on the homepage that takes 3 seconds to complete? No. Animation should serve the user's understanding, not the founder's pride.

</details>

<details>
<summary><b>How do I choose colors?</b></summary>

Pick one brand color you like. Use it sparingly — maybe 5% of any screen, on the most important action. Use grayscale for everything else (whites, blacks, two or three grays). Add red or amber for warnings/errors. That's it. **Three to four colors total, used consistently, beats fifteen colors used inconsistently every single time.**

</details>

---

## Ready to Launch Your SaaS?

At [Pexa Studio](https://pexastudio.com) we take non-technical founders from idea to live SaaS in **21 days**. Fixed price **$3k–$6k**. You own 100% of the code.

Design comes baked in. We use a clean, tested system that converts — adapted to your brand without inventing fragile patterns. You don't have to debate fonts.

→ **[Book a free 30-minute intro call](https://cal.com/shakirdmr/free-intro-call)**

*Trusted by founders in US & Europe · 21 days · $3k–$6k · 100% code ownership*

---

← [Chapter 4: Choosing Your Stack](../04-choosing-your-stack/) · **Next:** [Chapter 6 — Building in 21 Days →](../06-building-in-21-days/)
