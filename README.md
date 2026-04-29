# Star Jesse Taylor — Website Setup

## Step 0 — Get Claude Code (do this first)

Two ways — pick one:

**Option A: Chrome extension (easiest, no install)**
1. Open Chrome and go to: [claude.ai/code](https://claude.ai/code)
2. Sign up or log in ($20/mo)
3. Install the Chrome extension when it prompts you — this lets Claude see your browser and open links for you

**Option B: Desktop app**
1. Download at: [claude.ai/download](https://claude.ai/download)
2. Sign up or log in

---

## Step 1 — Run this in Claude Code

Open Claude Code and paste exactly this:

```
Read this README and set up my website: https://github.com/lucyc166/star-website

Clone the repo, open index.html so I can preview it, then ask me what I want to change before we go live.
```

Claude will handle everything from here. Just follow what it tells you.

---

## Step 2 — Preview and edit

Claude will give you a local link like `http://localhost:8080` — open it in Chrome to see your site.

Then tell Claude anything you want to change:
```
Change the discovery call price to $600
Add my Calendly link to both Apply Now buttons: [paste your Calendly URL]
Replace the hero headline with: [your new headline]
```

---

## Step 3 — Create a Vercel account (free hosting)

1. Open a new tab and go to: [vercel.com/signup](https://vercel.com/signup)
2. Sign up with your email (free)
3. Come back to Claude and say:
```
Deploy my site to Vercel
```
Claude will run the deploy command. When it says "Paste this in your terminal" or asks you to log in, type this into Claude:
```
! npx vercel login
```
A browser window will open — log in with your Vercel email. Then tell Claude:
```
Now deploy it
```
Claude will give you a live URL ending in `.vercel.app` — your site is on the internet.

---

## Step 4 — Buy and connect your domain (~$12/yr)

1. Go to: [namecheap.com](https://namecheap.com)
2. Search for `starjessetaylor.com` and buy it (~$12/yr)
3. Go to: [vercel.com/dashboard](https://vercel.com/dashboard) → click your project → Settings → Domains
4. Type in your domain and click Add
5. Vercel will show you two DNS records to copy
6. Go back to Namecheap → Dashboard → click Manage next to your domain → Advanced DNS
7. Paste the two records Vercel gave you
8. Wait 10–30 min — your site will be live at your domain

---

## Step 5 — Save your work to GitHub

After any changes, tell Claude:
```
Save all my changes to GitHub
```
This backs up every version forever. If anything breaks, you can always go back.

---

## That's it — you're live.

For any future edits, open Claude Code and just say what you want:
- *"Add a new testimonial from [name]: [quote]"*
- *"Change the workshop price to $597"*
- *"Add a new section for my podcast"*
- *"Make the site look better on mobile"*

---

## Power workflows

See **[WORKFLOWS.md](WORKFLOWS.md)** for 10 copy-paste prompts covering:
- What to work on next
- Bug checks before you ship
- Mobile testing
- Architecture review
- How to add features without breaking things
- End-of-session save + summary

---

## Claude Code tips

- Say which section to change: *"only update the coaching section prices"*
- Say what NOT to touch: *"don't change anything except the footer"*
- One thing at a time
- If something breaks: *"undo that and go back to how it was"*
- Save after every session: *"commit and push to GitHub"*

---

## For Claude — setup instructions

> *Read this and execute in order when the user runs the setup prompt.*

1. `git clone https://github.com/lucyc166/star-website.git && cd star-website`
2. Open `index.html` with `open index.html` so the user can preview it in their browser
3. Say: *"Your site is open in Chrome. What would you like to change before we go live?"*
4. Make edits to `index.html` and/or `ask.html` based on user input
5. When user is ready to deploy, run: `npx vercel --prod`
   - If not logged in, prompt: *"Type this in the chat to log in: `! npx vercel login`"*
   - After login, re-run: `npx vercel --prod`
6. Give the user their live `.vercel.app` URL
7. Walk them through Step 4 (domain) and Step 5 (GitHub save) above
8. After domain is connected and changes saved, say: *"You're live at [domain]. To make any future changes, just open Claude Code and tell me what you want."*

**To rebuild from scratch:**
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

Real testimonials:
- "This book helped shift my mindset" — C.I.
- "Your book ultimately changed my perspective because of how simple you made it." — Arely
- "No need to spend years on therapy" — H.
- "Your teachings are God's work." — G.
- "I feel like a completely different person" — Kaye R.
- "8 sessions with Jesse — incredible experience. He was so kind and patient." — Kaye R.
- "My life now has never ever been so clear, and free." — Lara K.
- "My emotions no longer rule my life." — Lara K.
- "I gained immense freedom from being able to stop mid-thought." — Sophie

YouTube video IDs: SALZHpK1AEg, -Erwj1uCDLU, RJ0z5-yghBg
Images: star-hero.jpg (headshot), book-cover.jpg

Sections: Nav → Hero → About → Programs → Videos → Book → 
Testimonials (scrolling marquee) → Coaching → Email CTA → Footer

Pure HTML + CSS + vanilla JS. No frameworks. Two files: index.html and ask.html.
```
