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

---

# 1. What I'm Building & Who It's For

**One sentence:**

> A calculator that runs in my browser and does basic math with buttons or the keyboard.

**Project name:**

> `calculator`

**Why I'm building it:**

> I want one finished project I actually understand, that I can put on GitHub.

**Who, and where:**

> Anyone who needs a quick calculation, on a laptop or phone browser. No signup, no instructions needed.

---

# 2. Must-Haves

**What it has to do:**

> 1. Add, subtract, multiply, divide
> 2. Click buttons to enter numbers
> 3. Type on the keyboard to enter numbers
> 4. Show what I typed and the answer
> 5. Clear everything
> 6. Delete the last digit
> 7. Handle decimals

---

# 3. Not Building (Yet)

**Not in this version:**

> - No login or user accounts
> - No saving anything — close the tab, it's gone
> - No scientific functions (sin, cos, log)
> - No history of past calculations *(maybe later)*
> - No dark/light theme toggle *(maybe later)*
> - No back-end — this session is front-end-only

---

# 4. How It Behaves

**Behaviors:**

> - When I click `7`, then `7` shows in the display.
> - When I click `7 + 3 =`, then it shows `10`.
> - When I press `Enter`, then it acts like `=`.
> - When I press `Escape`, then it clears.
> - When I click `.` twice, then only one decimal point is accepted.
> - When an answer is showing and I type a number, then the new number replaces the answer.

---

# 5. What It Looks Like

**Sketch:**

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

**Colors and font:**

> Dark purple background, white text, purple `=` button. Clean sans-serif; monospace for the display so numbers don't jump around.

**How many screens:**

> One. No menus, no other pages.

---

# 6. Front-End Only, or Front-End + Back-End?

**Front-end** = what the user sees and clicks (HTML, CSS, JavaScript in the browser).

**Selection:**

- [Yes] **Front-end only** → fill in Section 7

> Front-end only. Nothing needs saving.

**How to tell:**

| If your app has to... | You need |
|---|---|
| Just calculate, display, or convert | **front-end only** |

> **Start front-end only if you can.** It's not a real complete app, rather its a demo, and i's far easier to get running. You can add a back-end later after the innovation hub presentation.

---

# 7. Front-End Basics

**Built with:**

> Plain HTML, CSS, and JavaScript. No frameworks, no libraries, nothing to install.

**What it has to remember while running:**

> The number I'm typing, the previous number, which operator I picked, and whether the display is showing an answer.

**Input methods:**

> Clicking/tapping the buttons, plus keyboard: digits, `+ - * /`, `Enter`, `Escape`, `Backspace`.

**Works on:**

> Chrome, Safari, Firefox, Edge. Must not break on a phone screen.

**Accessibility:**

> Every button reachable with the Tab key, with a visible outline. Buttons big enough to tap with a thumb.

---

# 8. Running It On My Computer

We're keeping this **local only** — it runs on your machine, at an address only you can open. That's a finished, working app. Putting it on the public internet is a later session.

**What's already installed on my machine:**

> VS Code, GitHub Desktop, Chrome.

**How I start it:**

> Double-click `index.html`.

**What "running it" looks like:**

| Your build | How you start it | Where you open it |
|---|---|---|
| Front-end only | double-click `index.html` | the file opens right in your browser |

**How I know it's working:**

> The calculator appears in the browser, buttons respond to clicks, and there are no red errors in the console (F12 → Console).

> **`127.0.0.1` and `localhost` mean the same thing: your own computer.** Nobody else on the internet can reach that address, which is exactly what you want while learning.

---

# 9. Rules and Edge Cases

**What happens when...**

> - **Divide by zero** → show `Cannot divide by zero`. Never show `Infinity` or `NaN`.
> - **Answer is really long** (`1 ÷ 3`) → round it so it fits the display.
> - **Extra zeros** → typing `0 0 5` shows `5`, not `005`.
> - **Starting with an operator** → ignore it, there's nothing to add to yet.
> - **`C` vs `DEL`** → `C` wipes everything; `DEL` removes one character.
> - **`0.1 + 0.2`** → must show `0.3`, not `0.30000000000000004`.

---

# 10. My Checklist — How I Know It's Done

**Test each:**

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

**My workflow:**

> 1. `main` always works. Broken code never sits on `main`.
> 2. Each new idea gets its own branch: `feature/layout`, `feature/operators`, `feature/edge-cases`.
> 3. I read the diff before every commit. If I don't understand a change, I ask AI to explain it before committing.
> 4. Commit messages say *why*: `Fix rounding on addition`.
> 5. If an attempt goes sideways, I delete the branch and start fresh from `main`.

> **Never commit passwords, API keys, or `.env` files.** Ask AI for a `.gitignore` **before** your first commit.

---

# 12. Prompts to Run, In Order

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
on screen after each one.
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

**What changed and why:**

> - `2026-08-08` — Wrote this at the Innovator Hub session, before any code.
> - `2026-08-25` — Confirmed the calculator spec as-written (Sections 1–10). Removed the VS Code Live Server option from Section 8 — this build is opened only by double-clicking `index.html`, nothing else. Scaffold (HTML/CSS) built; JavaScript behavior next.

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

---

*Hikma Foundation · Innovator Hub · Modern Development (AI-Assisted) · [www.HikmaCLT.org](https://www.HikmaCLT.org)*
