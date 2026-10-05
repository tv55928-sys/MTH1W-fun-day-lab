# Fun Day Code Lab

A browser-based coding page for Grade 9 math (Ontario MTH1W, strand C2: Coding). Students don't need to log in. They read, predict, run and change **EQAO-style pseudocode** that compares two linear relations and finds their point of intersection.

## What's on the page

- **Start here:** five short lessons for students who have never coded. They cover output, storing a number, doing math with variables, updating a variable, and making a decision. Each lesson checks the student's work and unlocks the next one.
- **Lesson programs:** the Warm-up, Task 1, Task 2A, Task 2B, going-further Tasks 3–5, and the EQAO 2025 Q9 perimeter item.
- **Supports for IEP accommodations:**
  - A colour-coded editor with a colour key that can be switched off.
  - "Bigger text" and "Read aloud" buttons.
  - Steps shown one at a time.
  - Hints that appear one at a time.
  - Numbered page regions: 1 Read the task, 2 Read the code, 3 Predict, 4 Run and compare.
  - A sentence frame after each run.
  - "Step through", which shows memory boxes updating line by line.
- The Run button unlocks only after students confirm that their prediction is on the whiteboard.
- **Try similar questions (optional):** after each task, students can try three similar questions in the EQAO style. They get immediate feedback, including a specific tip for common wrong answers. They can use "See it run" to check a question with the computer, or move on to the next task at any time.
- **EQAO-style practice:** a linear systems set of eight questions about two linear relations and where they meet.
- A symbol decoder, and a "Show in Python" view.

## How it works

The page translates the pseudocode into Python. It then runs the Python in the browser with [Skulpt](https://skulpt.org/) 1.2.0 (MIT licence). Skulpt is built into `index.html` (its licence is in a comment just before the Skulpt code), so the page is a single file and doesn't depend on an outside code server. There's no server and no account, and no student data leaves the device.

## Safety

- **Locked-down runner.** Students write pseudocode only. The page turns off:
  - imports
  - JavaScript access (`jseval`)
  - file and network modules
  - `input()` pop-ups
  - names that start with `__`
  - special strings (f-strings and similar)
  - several other built-in functions
  
  If a student types any of these, the page explains why in plain language instead of running the code.
- **Limits.** Programs stop after 4 seconds, 500 lines of output, or 300 lines of code.
- **Inputs are cleaned.** Typed inputs are limited to 20 values of 40 characters each.
- **Output can't run.** Everything a program outputs is shown as plain text, never as HTML.
- **No outside connections.** A Content Security Policy blocks the page from connecting to other sites. The only outside item it loads is Google Fonts.
- **Work is cleared on shared Chromebooks.** Saved work is erased after 12 hours, and students can press "Clear my work" (tap twice).

## Use it

1. In your GitHub repository, choose **Add file → Upload files**.
2. Drag in `index.html` and `README.md`, then choose **Commit changes**.
3. Turn on GitHub Pages: **Settings → Pages → Deploy from branch → `main` / root**.

You can also open `index.html` directly in a browser.

A GitHub Pages site is public. Anyone with the link can open it, but they can't change it.
