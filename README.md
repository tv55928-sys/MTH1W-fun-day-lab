# Fun Day Code Lab

A no-login, browser-based coding page for Grade 9 math (Ontario MTH1W, strand C2: Coding). Students read, predict, run and change **EQAO-style pseudocode** that compares two linear relations and finds their point of intersection.

## Features

- Runs EQAO-style pseudocode: `output`, `if … = …`, `else if`, `else`, `repeat N times`, `store user input as`
- A symbol decoder at the top of the page
- Lesson programs preloaded: Warm-up, Task 1, Task 2A, Task 2B, going-further Tasks 3–5, and the EQAO 2025 Q9 perimeter item
- A "Run" button that unlocks only after students confirm their prediction is on the whiteboard
- A "Show in Python" view of the same program
- Works on Chromebooks; edits are saved in the browser

## How it works

The page translates pseudocode into Python and runs it in the browser with [Skulpt](https://skulpt.org/) (loaded from cdn.jsdelivr.net). There's no server and no account, and no student data leaves the device.

## Use it

Open `index.html` in a browser, or publish it with GitHub Pages (Settings → Pages → Deploy from branch → `main` / root).

If the page shows "The runner did not load", the school network is blocking cdn.jsdelivr.net. Ask IT to allow it.
