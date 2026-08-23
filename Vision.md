# vision.md

### Hikma Innovator Hub · AI-Assited DEVELPMENT

**Fill this out before you write any code.** Then hand it to your AI assistant — Claude, Copilot, or ChatGPT — and let it build what you described.

---

## Why bother?

AI will build almost anything you ask for. That's the problem. *"Make me a calculator"* gets you **a** calculator — maybe not yours.

Ten minutes here saves an hour of *"no, not like that."*

**This is the Discovery & Planning step** from the session. Blueprints before building.

---

## How to use it

1. Copy this file into your project folder. Name it `vision.md`.
2. Fill in every 🔲. Delete the calculator examples as you go.
3. Open the folder in VS Code and start your AI assistant.
4. First prompt: **"Read vision.md and tell me what you're about to build. Don't write code yet."**
5. Then: **"Looks right — build it."**
6. Something wrong? **Fix `vision.md` first**, then say *"I updated vision.md, re-read it."*

| Marker | Meaning |
|---|---|
| 🔲 | You fill this in |
| 📐 | Example answer (calculator app) — delete it |
| ⏭️ | Skip if it doesn't apply to you |

---

# 1. What I'm Building & Who It's For

🔲 **One sentence:**

> 📐 A calculator that runs in my browser and does basic math with buttons or the keyboard.

🔲 **Project name** (this becomes the folder and repo name):

> 📐 `simple-calculator`

🔲 **Why I'm building it:**

> 📐 I want one finished project I actually understand, that I can put on GitHub.

🔲 **Who, and where:**

> 📐 Anyone who needs a quick calculation, on a laptop or phone browser. No signup, no instructions needed.

---

# 2. Must-Haves

Keep this list short. Everything here is code that can break.

🔲 **What it has to do:**

> 📐
> 1. Add, subtract, multiply, divide
> 2. Click buttons to enter numbers
> 3. Type on the keyboard to enter numbers
> 4. Show what I typed and the answer
> 5. Clear everything
> 6. Delete the last digit
> 7. Handle decimals

---

# 3. Not Building (Yet)

**Don't skip this one.** AI fills silence with assumptions. If you don't say "no login," you might get one.

🔲 **Not in this version:**

> 📐
> - No login or user accounts
> - No saving anything — close the tab, it's gone
> - No scientific functions (sin, cos, log)
> - No history of past calculations *(maybe later)*
> - No dark/light theme toggle *(maybe later)*
> - No back-end — this session is front-end-only

---

# 4. How It Behaves

Write these as "when I ___, then ___." This is what AI turns into code.

🔲 **Behaviors:**

> 📐
> - When I click `7`, then `7` shows in the display.
> - When I click `7 + 3 =`, then it shows `10`.
> - When I press `Enter`, then it acts like `=`.
> - When I press `Escape`, then it clears.
> - When I click `.` twice, then only one decimal point is accepted.
> - When an answer is showing and I type a number, then the new number replaces the answer.

---

# 5. What It Looks Like

A rough sketch beats a paragraph. Text boxes are fine.

🔲 **Sketch:**

> 📐
> ```
> ┌─────────────────────┐
> │               1,234 │  ← the display
> ├─────┬─────┬─────┬───┤
> │  C  │ DEL │  .  │ ÷ │
> ├─────┼─────┼─────┼───┤
> │  7  │  8  │  9  │ × │
> ├─────┼─────┼─────┼───┤
> │  4  │  5  │  6  │ − │
> ├─────┼─────┼─────┼───┤
> │  1  │  2  │  3  │ + │
> ├─────┴─────┼─────┼───┤
> │     0     │  =  │ + │
> └───────────┴─────┴───┘
> ```

🔲 **Colors and font:**

> 📐 Dark purple background, white text, purple `=` button. Clean sans-serif; monospace for the display so numbers don't jump around.

🔲 **How many screens:**

> 📐 One. No menus, no other pages.

---

# 6. Front-End Only, or Front-End + Back-End?

This is the biggest decision in the file. It decides how much gets built and how hard it is to run.

**Front-end** = what the user sees and clicks (HTML, CSS, JavaScript in the browser).
**Back-end** = a program running behind the scenes that stores data or keeps secrets.

🔲 **Pick one:**

- [Yes] **Front-end only** → fill in Section 7

> Back-end builds aren't covered in this template — that's a later session.

> 📐 Front-end only. Nothing needs saving.

**How to tell:**

| If your app has to... | You need |
|---|---|
| Remember something after the browser closes | a back-end |
| Let two different people see the same data | a back-end |
| Hide a password or API key | a back-end |
| Just calculate, display, or convert | **front-end only** |

> **Start front-end only if you can.** It's a real, complete app, and it's far easier to get running. You can add a back-end later.

---

# 7. Front-End Basics

🔲 **Built with:**

> 📐 Plain HTML, CSS, and JavaScript. No frameworks, no libraries, nothing to install.

🔲 **What it has to remember while running:**

> 📐 The number I'm typing, the previous number, which operator I picked, and whether the display is showing an answer.

🔲 **Input methods:**

> 📐 Clicking/tapping the buttons, plus keyboard: digits, `+ - * /`, `Enter`, `Escape`, `Backspace`.

🔲 **Works on:**

> 📐 Chrome, Safari, Firefox, Edge. Must not break on a phone screen.

🔲 **Accessibility:**

> 📐 Every button reachable with the Tab key, with a visible outline. Buttons big enough to tap with a thumb.

---

# 8. Running It On My Computer

We're keeping this **local only** — it runs on your machine, at an address only you can open. That's a finished, working app. Putting it on the public internet is a later session.

🔲 **What's already installed on my machine:**

> 📐 VS Code, GitHub Desktop, Chrome. No Python yet.

🔲 **How I start it:**

> 📐 Double-click `index.html`, or right-click it in VS Code and choose "Open with Live Server."

**What "running it" looks like, by project type:**

| Your build | How you start it | Where you open it |
|---|---|---|
| Front-end only | double-click `index.html` | the file opens right in your browser |
| Front-end only, nicer | VS Code "Live Server" extension | `http://127.0.0.1:5500` — auto-refreshes when you save |

🔲 **How I know it's working:**

> 📐 The calculator appears in the browser, buttons respond to clicks, and there are no red errors in the console (F12 → Console).

> **`127.0.0.1` and `localhost` mean the same thing: your own computer.** Nobody else on the internet can reach that address, which is exactly what you want while learning.

---

# 9. Rules and Edge Cases

This is what separates a demo from something that works. Ask AI *"what edge cases am I missing?"* and add its answers here.

🔲 **What happens when...**

> 📐
> - **Divide by zero** → show `Cannot divide by zero`. Never show `Infinity` or `NaN`.
> - **Answer is really long** (`1 ÷ 3`) → round it so it fits the display.
> - **Extra zeros** → typing `0 0 5` shows `5`, not `005`.
> - **Starting with an operator** → ignore it, there's nothing to add to yet.
> - **`C` vs `DEL`** → `C` wipes everything; `DEL` removes one character.
> - **`0.1 + 0.2`** → must show `0.3`, not `0.30000000000000004`.

---

# 10. My Checklist — How I Know It's Done

Click through these by hand. You can also hand this list back to AI and ask it to check each one.

🔲 **Test each:**

> 📐
> - [ ] `7 + 3 =` shows `10`
> - [ ] `9 − 12 =` shows `-3`
> - [ ] `10 ÷ 4 =` shows `2.5`
> - [ ] `5 ÷ 0 =` shows an error, not `Infinity`
> - [ ] `0.1 + 0.2 =` shows `0.3`
> - [ ] Typing `1 2` then `Enter` works like clicking
> - [ ] `Escape` clears the display
> - [ ] `.` twice gives only one decimal point
> - [ ] Tab moves through every button visibly
> - [ ] Nothing overflows on a phone-width window
> - [ ] No errors in the browser console
> - [ ] I can explain every function in my code out loud

---

# 11. My Git Habits for This Build

From the *Vibe Coding* slide: **a branch per attempt.** If an idea fails, you delete a branch instead of repairing your project.

🔲 **My workflow:**

> 📐
> 1. `main` always works. Broken code never sits on `main`.
> 2. Each new idea gets its own branch: `feature/layout`, `feature/operators`, `feature/edge-cases`.
> 3. I read the diff before every commit. If I don't understand a change, I ask AI to explain it before committing.
> 4. Commit messages say *why*: `Fix rounding on addition`.
> 5. If an attempt goes sideways, I delete the branch and start fresh from `main`.

> **Never commit passwords, API keys, or `.env` files.** Ask AI for a `.gitignore` **before** your first commit.

---

# 12. Prompts to Run, In Order

**Ask for one step at a time.** "Build the whole thing" gives you code you didn't watch get written — and can't fix.

**On GitHub Copilot Free:** chat is capped at 50 messages/month (code completions
get 2,000/month — effectively unlimited for a project this size). The 6 prompts
below cost 6 of your 50 per build, leaving roughly 44 for debugging. Stretch it
further: batch several questions or edge cases into one message instead of
one-per-message, let inline completions (not chat) handle small one-line edits,
and stay in one chat thread per project instead of starting new ones.

**1. Plan**
```
Read vision.md in this folder. Tell me in your own words what you're about
to build, list any assumptions you're making, confirm front-end-only is
right for this (Sections 1-6), and ask me anything unclear. Don't write
code yet.
```

**2. Scaffold + structure**
```
Based on Section 7 of vision.md, create the files this project needs plus
a .gitignore, and explain what each file does. Follow the Standing Rule:
Structured File Layout below when laying out folders. Then, using the
sketch in Section 5, write the HTML and CSS only — no JavaScript yet. I
want to see and click the buttons before anything works.
```

**3. Behavior**
```
Now add the JavaScript for the behaviors in Section 4 of vision.md,
starting with typing numbers and showing them, then operators and the =
button. Also handle every edge case in Section 9 (divide by zero, long
decimals, leading zeros, floating-point rounding, etc.) as you go. Explain
how you're keeping track of what I typed.
```

**4. Run it**
```
Give me the exact steps to run this on my computer right now, starting
from "I just opened this folder in VS Code," based on what's listed in
Section 8 of vision.md. Number every step and tell me what I should see
on screen after each one. Also list everything that needs to be installed,
with a command to check if I already have it.
```

**5. Verify**
```
Go through my checklist in Section 10 of vision.md one item at a time.
Say pass or fail and why for each, then fix anything that fails.
```

**6. Wrap up**
```
Explain the main function in my code line by line as if I've never
written JavaScript, then ask me three questions to check I understood.
Finally, write a README.md based on vision.md: what this is, how to run
it, and what I learned building it.
```

> **When something's broken, be specific.** Not *"it doesn't work"* but:
> *"When I click 5, then ÷, then 0, then =, I expected an error but got Infinity. Which part of the code handles that, and why didn't it catch it?"*
>
> Specific in, specific out.

---

# 13. Notes

🔲 **What changed and why:**

> 📐 `2026-08-08` — Wrote this at the Innovator Hub session, before any code.

---

## Standing Rule: No Back-End

> No matter what I ask for later in this project, do not add a back-end,
> server, database, or API. If a request implies one — login, saved data,
> multi-user state, hidden keys — say so, explain why it needs a back-end,
> and point back to Section 3 instead of building it. Don't ask me to
> confirm; just decline and explain.

## Standing Rule: Structured File Layout

> Organize output into folders, don't dump files in the root. Typical
> layout: `frontend/` (or `src/`) for HTML/CSS/JS, `assets/` for images
> and fonts, `backend/` only if Section 6 calls for one. Keep
> `index.html`, `README.md`, and config files (`.gitignore`,
> `package.json`) at the project root.

## Using this for your next project

Only the examples are calculator-specific — the same sections work for a to-do list, budget tracker, or personal site. Swap the examples, keep the structure. The sections that matter most: **3** (Not Building), **6** (Front-end or back-end), **10** (Checklist).

---

*Hikma Foundation · Innovator Hub · Modern Development (AI-Assisted) · [www.HikmaCLT.com](https://www.HikmaCLT.com)*
