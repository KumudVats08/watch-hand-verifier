# Watch Accuracy Verifier

A deliberately over-engineered web app for answering one simple question: **is your wristwatch showing the correct time?**

Instead of checking a phone, the Watch Accuracy Verifier makes users manually recreate their watch reading with an antique-style spinning clock, select AM or PM, solve a mental arithmetic problem, and wait through an unnecessarily formal verification process.

## Features

- Interactive hour and minute hands controlled with pointer or touch dragging.
- One full hour-hand rotation equals one hour.
- One full minute-hand rotation equals one minute.
- AM/PM selection and procedural confirmation.
- Long addition and subtraction exercises with simple multiplication.
- Incorrect answers trigger a rejected inspection stamp and reset the procedure.
- Live bureaucracy score tracking unnecessary user effort.
- Playful warning messages and an evasive “check my phone” button.
- Antique-inspired clock face with Roman numerals, aged dial coloring, brass and wood trim, and ornate hands.
- Formal verification result with a generated case number and issue time.
- Opening rules declaration inspired by intentionally frustrating form experiences.
- Responsive layout and reduced-motion support.
- No build process or external JavaScript dependencies.

## Run Locally

Because the app is a self-contained HTML file, it can be opened directly in a browser:

1. Open `index.html` in a modern browser.
2. Accept the temporal rules.
3. Rotate both clock hands, choose AM or PM, and acknowledge the procedure.
4. Confirm the declared time.
5. Solve the arithmetic challenge.
6. Review the official result.

A local server is optional. For example, with Python installed:

```bash
python -m http.server 8000
```

Then open <http://localhost:8000>.

## Design Direction

The visual language combines a satirical government form with an antique measuring instrument. Warm paper tones, Roman numerals, layered brass trim, formal labels, and stamped outcomes make the app feel authoritative while the deliberately unnecessary workflow undercuts that authority.

The interaction design adds playful friction without making the app unusable: users receive official-sounding warnings, accumulate a bureaucracy score, and encounter harmless resistance when attempting to take a shortcut.

## Technical Notes

- HTML, CSS, and JavaScript are all contained in `index.html`.
- The current system time is read with JavaScript’s `Date` object.
- Pointer events support mouse and touch interaction.
- The arithmetic answer is calculated with standard multiplication precedence.
- Google Fonts are used optionally for the Fraunces and DM Sans typefaces.
