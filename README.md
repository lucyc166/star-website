# Star Jesse Taylor — Website

Live site files: `index.html` (main site) + `ask.html` (Ask Me Anything page).

---

## Rebuild Prompt

Paste this into Claude Code to rebuild or modify the site:

```
Build me a personal website for Star Jesse Taylor, a mental fitness coach.

Likes turquoise. Dark background. Inspired by kylecease.com and tonyrobbins.com.

About him: helps people rewire their brain, end anxiety, build self-worth 
through practical tools (not therapy). Has a 129-page book, YouTube channel, 
online courses, and 1:1 coaching.

Offerings:
- Free YouTube content
- Intro course $197
- Self-Worth Workshop $497
- Discovery call $500 / 50 min
- Private coaching — 5wk, 10wk, 3mo packages

Real testimonials to use:
- "This book helped shift my mindset" — C.I.
- "Your book ultimately changed my perspective because of how simple you made it." — Arely
- "No need to spend years on therapy" — H.
- "Your teachings are God's work." — G.
- "I feel like a completely different person" — Kaye R.
- "8 sessions with Jesse — incredible experience. He was so kind and patient." — Kaye R.
- "My life now has never ever been so clear, and free." — Lara K.
- "My emotions no longer rule my life." — Lara K.
- "I gained immense freedom from being able to stop mid-thought." — Sophie

YouTube video IDs to embed: SALZHpK1AEg, -Erwj1uCDLU, RJ0z5-yghBg

Images I have: star-hero.jpg (headshot), book-cover.jpg

Sections: Nav → Hero → About → Programs → Videos → Book → 
Testimonials (scrolling marquee) → Coaching → Email CTA → Footer

Pure HTML + CSS + vanilla JS. No frameworks. Two files: index.html and ask.html 
(Ask Me Anything page in the same dark/teal design).
```

---

## How to Set This Up (no coding experience needed)

### The 3 things that make a website work

**1. The code — Claude Code writes this for you**
Your website is just two files: `index.html` and `ask.html`. Claude Code writes them. You describe what you want in plain English and it makes the changes — you never need to touch the actual code.

**2. Vercel — moves it from your computer to the internet**
Vercel publishes your files so anyone can visit. Free. Drag your folder in, it gives you a URL. Takes 2 minutes. Every time you update something, redeploy.

**3. Domain — your web address**
Buy `starjessetaylor.com` on Namecheap or GoDaddy (~$12/yr), then point it at Vercel in the settings. Vercel walks you through it step by step.

**If you later want bookings, payments, or user accounts — that's a database.**
A database (Supabase) stores everything: who signed up, who booked a call, purchase history. You don't need this on day one. Start with the static site, link out to your existing shop and Calendly. Add the database when you're ready to build something more custom.

---

## How to Use Claude Code

- Works in the browser at [claude.ai/code](https://claude.ai/code) or via the Chrome extension — no install needed
- Talk to it like a contractor: *"change the coaching section price to $600"* or *"make the hero image bigger on mobile"*
- Always say what NOT to touch: *"only edit the footer, don't change anything else"*
- One change at a time — don't ask it to redesign everything in one message
- If something breaks: *"undo that and go back to how it was"*

---

## Biggest Mistakes to Avoid

- **Trying to build everything at once** — site → database → payments → bookings. Ship the site first, add features one at a time.
- **Not saving a backup** — push your files to GitHub (this repo) so every version is stored forever.
- **Buying expensive tools before you need them** — a great site costs $12/yr (domain) + free Vercel.
- **Editing the wrong file** — always tell Claude which file and which section to change.

---

## Quickstart Checklist

- [ ] Buy domain on Namecheap or GoDaddy (~$12)
- [ ] Sign up for [Claude Code](https://claude.ai/code) ($20/mo) or use the Chrome extension
- [ ] Paste the rebuild prompt above → get `index.html` + `ask.html`
- [ ] Sign up for [Vercel](https://vercel.com) (free)
- [ ] Drag your folder into Vercel → site is live
- [ ] Connect your domain in Vercel settings
- [ ] Add Calendly links to the coaching buttons
- [ ] Push files to GitHub (this repo) as your backup
