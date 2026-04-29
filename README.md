# Star Jesse Taylor — Website Setup

## How to use this

1. Go to [claude.ai/code](https://claude.ai/code) (or open the Claude Chrome extension)
2. Paste this into the chat:

```
Read this README and set up my website: https://github.com/lucyc166/star-website
```

Claude will download the files, open them, and walk you through the rest.

---

## What Claude will do for you

When you run the above prompt, Claude Code will:
- Download all the website files from GitHub
- Open them so you can preview the site
- Help you make any changes (text, prices, images, colors)
- Deploy to Vercel so it's live on the internet
- Connect your domain

---

## Claude Setup Instructions

> *This section is for Claude Code to read and execute.*

1. Clone this repo: `git clone https://github.com/lucyc166/star-website.git`
2. Open `index.html` in the browser to preview
3. Ask the user: "What would you like to change before we go live?" 
4. Make their edits to `index.html` and `ask.html`
5. Deploy to Vercel:
   - If Vercel CLI is installed: `npx vercel --prod`
   - If not: tell the user to go to vercel.com, click "Add New Project", and drag the folder in
6. Tell the user to connect their domain in Vercel → Settings → Domains

**To rebuild from scratch**, use this prompt:

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

## The 3 things that make a website work

**1. Code** — The two files in this repo (`index.html`, `ask.html`). Claude writes and edits these for you.

**2. Vercel** — Puts your site on the internet. Free. Go to [vercel.com](https://vercel.com), drag your folder in, it's live.

**3. Domain** — Your web address. Buy on [Namecheap](https://namecheap.com) or GoDaddy (~$12/yr), then connect it in Vercel settings.

**Database (Supabase)** — Only needed if you want user accounts, bookings, or stored data. Not needed to launch. Add later.

---

## Tips for using Claude Code

- Say exactly which section to change: *"update the coaching prices in the coaching section"*
- Say what NOT to touch: *"only change the footer, leave everything else alone"*
- One thing at a time
- If something breaks: *"undo that"*
- Save your work to GitHub after every session: *"commit and push my changes to GitHub"*
