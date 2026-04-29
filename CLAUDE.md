# CLAUDE.md — Instructions for Claude Code

This file is automatically read by Claude Code every session. Follow these instructions without being asked.

---

## On every session start — do this automatically

1. Read `index.html` and `ask.html`
2. Check git status — tell the user what changed since last time
3. Tell the user in plain English: what's working, what's broken, and the ONE thing they should work on today
4. Ask: "What would you like to do today?" — then do it

---

## Before making ANY change

1. Read the file first — never edit from memory
2. Tell the user exactly what you're going to change and what you're leaving alone
3. Make only what was asked — nothing extra
4. After the change, confirm it worked

---

## After every change — run this automatically

- Check that the site still opens without errors
- Check for broken links or missing images
- Check that the layout still looks correct on mobile (375px wide)
- If anything broke, fix it before telling the user you're done

---

## Before going live / deploying — run this automatically

Check everything below and fix any issues found. Do not ask the user — just fix them:

- All buttons and links work
- All images load (check src paths)
- Mobile layout looks correct at 375px
- Text is readable (no overflow, no tiny fonts)
- Nav menu works on mobile
- Forms have somewhere to submit
- No placeholder text left (no "[your link here]" etc.)
- No console errors in the HTML/CSS

Report what you checked and what you fixed.

---

## Deployment — when the user says "go live" or "deploy"

Run in order:
```bash
git add .
git commit -m "Update site"
npx vercel --prod
```

If not logged into Vercel, tell the user:
> "Type this to log in: `! npx vercel login` — a browser window will open, sign in with your email, then come back and say 'deploy now'"

After deploy, give the user their live URL.

---

## After every session — do this automatically

1. Save everything to GitHub:
```bash
git add .
git commit -m "[describe what changed in plain English]"
git push origin master
```
2. Tell the user in 3 lines: what changed, what's still to do, what to work on next time
3. Never end a session without saving to GitHub

---

## IMPORTANT — do not rebuild the site

The site (`index.html` and `ask.html`) is already built. Do NOT recreate, overwrite, or replace these files unless the user explicitly says "rebuild" or "start from scratch." Only make the specific changes the user asks for.

---

## Code rules

- This is a pure HTML/CSS/vanilla JS site — no frameworks, no build step
- All CSS lives inside `<style>` tags in each file
- Keep the dark background (`#060606`) and turquoise accent (`#2DD4BF`) consistent
- Match the existing font stack: Instrument Serif (headings) + DM Sans (body)
- Mobile first — every change must work at 375px
- Never duplicate code — if something is repeated, simplify it
- Never add features that weren't asked for

---

## If something is broken

1. Read every file involved before guessing
2. Tell the user what you think is causing it and why
3. Fix the root cause — not the symptom
4. Test the fix before saying it's done
5. Check that fixing it didn't break anything else

---

## Tone when talking to the user

- Plain English only — no technical jargon
- Short answers — one paragraph max unless showing code
- If something is complex, explain it like the user has never coded before
- Always say what you did, not just that you did it
