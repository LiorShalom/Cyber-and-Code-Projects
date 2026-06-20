# JavaScript Homework — Functions & Loops

My first JavaScript project, written as coursework. It's an interactive command-line program that bundles two sets of exercises — **Functions** and **Loops** — into one menu-driven app.

## What it does

When you run it, you choose between two homework sections:

- **[F] Functions** — 9 exercises: finding the biggest/smallest number, checking even/odd, comparing numbers, mapping a number to a weekday, looking up month info, capitalizing names, and working with variable scope.
- **[L] Loops** — 10 exercises: printing number ranges, deleting array elements, counting odd/even, finding duplicates, reversing strings, summing arrays, and searching arrays.

Each exercise prompts you for input and prints the result. You pick which question to run from a menu.

## How to run

This program needs Node.js and the `readline-sync` package for keyboard input.

```bash
# 1. Make sure Node.js is installed (https://nodejs.org)
# 2. Install the one dependency:
npm install readline-sync

# 3. Run it:
node "Functions&Loops.js"
```

Then follow the on-screen menu: type `F` or `L` to pick a section, then a question number.

## Notes

- The file name contains an `&`, so wrap it in quotes when running (as shown above).
- This was an early learning project — the focus was on practicing core JavaScript: functions, nested functions, loops, arrays, and conditionals.
