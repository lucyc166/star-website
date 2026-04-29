# Claude Code Power Workflows

These are the highest-leverage prompts to use with Claude Code. Copy and paste any of them at any time.

---

## 1. "What should I do next?"

Use this when you're not sure what to work on. Claude will scan what you've built, what's broken, and what matters most, then give you one prioritized recommendation.

```
Read my project files and tell me the single highest-leverage thing I should work on right now. Check for: broken things first, then missing features, then improvements. Give me one recommendation and explain why.
```

---

## 2. Check for bugs before you ship

Use this before you share the site with anyone or go live. Claude will scan your code for common mistakes.

```
Before I share this site, do a full bug check. Look for:
- Links that go nowhere
- Buttons that don't work
- Anything that breaks on mobile
- Images that won't load
- Forms that don't submit
- Any typos in the HTML or CSS that would cause display issues

List every issue you find, then fix them all.
```

---

## 3. Mobile check

Use this after any change to make sure your site still looks good on a phone.

```
Check how this site looks on mobile (375px wide screen). Look for:
- Text that's too big or too small
- Buttons that are hard to tap
- Anything that overflows or gets cut off
- Images that are the wrong size
- The navigation menu on small screens

Fix anything that looks wrong on mobile. Don't touch the desktop layout.
```

---

## 4. Architecture review — "is this built well?"

Use this when you want a second opinion on how the site is structured before adding more features.

```
Review the structure of my website files. Tell me:
- Is this organized well for someone who wants to keep adding to it?
- Are there any patterns that will cause problems later?
- Is there anything duplicated that should be in one place?
- What's the simplest way to add [feature] without breaking what's there?

Don't make any changes yet — just give me your assessment.
```

---

## 5. "Explain what you're going to do before you do it"

Use this any time you want to understand Claude's plan before it touches your code. Prevents surprises.

```
Before you make any changes, tell me:
- What you're going to change and why
- What you're NOT going to touch
- What it will look like when it's done
- Any risks or things that could go wrong

Wait for me to say "go ahead" before making any edits.
```

---

## 6. Find and fix one specific bug

Use this when something is broken and you know what it is.

```
[Describe the bug exactly — what you see, what you expected, when it happens]

Before you fix it:
1. Read every file that could be related
2. Tell me what you think is causing it
3. Explain the fix you're going to make
4. Then fix it and confirm it's working
```

---

## 7. Quality review — "is this code clean?"

Use this after adding a new section or feature to make sure it didn't add unnecessary bloat.

```
Review the changes I just made. Look for:
- Anything repeated that could be simplified
- CSS that conflicts with existing styles
- Anything that's more complicated than it needs to be
- Dead code or styles that aren't used

Clean it up. Keep everything working — just make it simpler.
```

---

## 8. Add a feature the right way

Use this when you want to add something new without breaking what's there.

```
I want to add [describe the feature]. 

Before you build it:
1. Read the existing code so you match the style exactly
2. Tell me the simplest version of this feature
3. Tell me what files you'll touch and what you'll leave alone
4. Build it, then check it on mobile

Only build what I asked for — nothing extra.
```

---

## 9. Before/after check — "did anything break?"

Use this after any change to verify nothing was accidentally broken.

```
I just made changes to [section/file]. Run a quick check:
- Does the site still open without errors?
- Do all links still work?
- Does the layout still look correct on desktop and mobile?
- Did anything shift or disappear that shouldn't have?

Tell me what you checked and whether everything passed.
```

---

## 10. End of session — save and summarize

Use this at the end of every working session.

```
We're done for today. Please:
1. Save all changes to GitHub with a clear commit message describing what we did
2. Tell me what we changed in plain English
3. Tell me what's still not done or could be improved
4. Tell me the one thing I should work on next time

Keep it short — just the facts.
```

---

## Quick reference

| When you want to... | Paste workflow # |
|---|---|
| Know what to work on | 1 |
| Check for bugs | 2 |
| Test on mobile | 3 |
| Sanity-check the structure | 4 |
| See Claude's plan before it acts | 5 |
| Fix a specific bug | 6 |
| Clean up messy code | 7 |
| Add something new safely | 8 |
| Verify nothing broke | 9 |
| Wrap up a session | 10 |
