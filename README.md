# Mr. Fraction's Factory

An interactive, dyslexia-friendly tool for teaching fractions, decimals, and percentages to middle school students. Everything lives in a single self-contained HTML file styled as a factory that *produces fractions*, with Mr. Fraction guiding students through every step.

🔗 **Live site:** [jontaylormed.github.io/MrFractionFactory](https://jontaylormed.github.io/MrFractionFactory/)

[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

---

## What it does

Students enter through a loading screen (Mr. Fraction dancing), land on the factory home page, and pick a station. Each station teaches the same numbers from a different angle — fraction, decimal, and percent — so students stop seeing them as separate topics.

| Station | Name | What students do |
|--------|------|------------------|
| 01 | **Job Training** | Two bays and a workshop. **Bay A — What Fractions Are** (10 steps): what a fraction is, what each number controls, equivalence, the number line, negatives, and why some decimals never end. **Bay B — Working With Fractions** (7 steps): mixed numbers, the GCF, adding and subtracting, percents, multiplying, and dividing. **Division Workshop** (4 steps, optional): place value as an exchange, dealing out into groups, and what "bring down a zero" really means. Students pick a door and can switch at any time. |
| 02 | **Simplifier** | Reduce fractions to lowest terms with a full Euclidean-algorithm engine, animated step reveals, and canvas pie charts. |
| 03 | **Operations** | Build two fractions by shading pieces, then add, subtract, multiply, or divide. Every operation walks through its steps before the answer. Adding and subtracting: compare → re-cut → combine. Multiplying, on an area model: start with B → take A of it → count the pieces. Dividing, with division-bracket arrows: compare → re-cut → count how many B fit in A. Each fraction has a "Negative" box at its top, and anything negative is added or subtracted on a number line. |
| 04 | **Converter** | Change any value — fraction, decimal, or percent — and watch the others follow, with pie charts, number lines and percent bars side by side. Includes **The Remainder Belt**, a working long-division machine. |
| 05 | **Assessment Bay** | Nine randomized, gamified challenges across four difficulty tiers. Ships only on 100% correctness, with "Try Again" on every challenge and a Certificate of Completion at the end. |

Mr. Fraction appears at the bottom of every station page.

Two buttons at the top right of every page:

- **🎓 For Teachers** opens a guide page: what the site is, the learning targets for every station, suggested routes for different students, and the supports built in.
- **Reading & Access** opens the settings panel described [below](#reading--access). <kbd>Alt</kbd> + <kbd>A</kbd> also opens it.

## Learning targets

The For Teachers page lists these as student "I can" statements, each tagged with the closest Common Core standard:

| Station | Targets | Standards |
|---|---|---|
| Job Training · Bay A | Explain what the numerator and denominator tell me; tell proper fractions, improper fractions and whole numbers apart; make and justify equivalent fractions; place and compare fractions, including negatives, on a number line; predict whether a decimal stops or repeats | 3.NF.1 · 4.NF.3 · 4.NF.1 · 3.NF.2 · 6.NS.6c · 6.NS.7 · 7.NS.2d |
| Job Training · Bay B | Switch between improper fractions and mixed numbers; find a GCF; add and subtract with unlike denominators; write a fraction as a percent; multiply with an area model; divide as "how many fit" | 4.NF.3b · 6.NS.4 · 5.NF.1 · 6.RP.3c · 5.NF.4 · 6.NS.1 |
| Division Workshop | Explain long division as dealing out and exchanging leftovers for smaller place values | 5.NBT.1 · 6.NS.2 · 6.NS.3 |
| Simplifier | Simplify to lowest terms with the GCF, and explain why the amount doesn't change | 6.NS.4 · 4.NF.1 |
| Operations | Add, subtract, multiply and divide fractions and explain each step; find the LCD; add and subtract negatives on a number line; use the sign rules | 5.NF.1 · 5.NF.4 · 6.NS.1 · 7.NS.1 · 7.NS.2a–b |
| Converter | Convert between fractions, decimals and percents; explain repeating decimals with long division | 6.RP.3c · 7.NS.2d |
| Factory Floor | Show all of the above independently, across nine challenges in four tiers | — |

## Inside Job Training

**Bay A — What Fractions Are**

1. What is a Fraction? — eat a drawn pizza slice by slice; eaten and remaining fractions move together
2. The Two Numbers — a live model where the denominator re-cuts the whole and the numerator only fills it
3. Types of Fractions
4. Equivalent Fractions
5. Fractions on a Number Line
6. **Below Zero** — negative fractions as mirror images, including the ordering trap (−3/4 < −1/2)
7. **The Dividing Machine** — predict "clean cut or endless loop", then watch real long division settle it
8. **The Sevenths Wheel** — discover that all six sevenths are the same six digits, rotated
9. Fractions in Real Life

**Bay B — Working With Fractions**

1. **The Repackaging Line** — improper ↔ mixed numbers; the leftover pieces *are* the remainder
2. Finding the GCF — the Euclidean machine
3. **The Mixing Line** — adding and subtracting. Combining fails first, which is how the common denominator earns its existence
4. **The Hundred Mould** — percent as a denominator, not an operation
5. Multiplying Fractions — read the grid
6. **The Measuring Line** — division as measurement ("how many of these fit inside that?"), then why you flip

**Division Workshop** *(optional, reachable from any machine that needs it)*

1. **The Exchange Counter** — place value as an exchange. Break one whole into ten tenths, a tenth into ten hundredths, and watch the total value refuse to move
2. **Dealing Out** — deal items round-robin into groups, one round at a time. The number of complete rounds *is* the quotient; whatever cannot make one more round is the remainder
3. **Exchange the Leftovers** — the leftovers sit in the Ones column, get exchanged for tenths, and get dealt again

Deliberately outside both bays. A confident student never opens it; a struggling one reaches it from a **🔧 Shaky on division?** button inside the Dividing Machine, the Repackaging Line, the Measuring Line, or Station 04's Remainder Belt. It remembers which bay and step they came from — or which station — and hands them back there when they finish.

The workshop never says "multiply the remainder by ten". That framing is why the step does not land. It is an **exchange** — the same amount in finer pieces, one column to the right — and the phrase "bring down a zero" is introduced last, as the name for what the student has just done.

## One rule, three forms

The site's spine is that a fraction, its decimal, and its percent are one number, and that a single rule governs all three.

- **A fraction is a division.** The bar means divide. Run it and you get the decimal.
- **A percent is a denominator.** "Per cent" means *per hundred*, so a percent is the same fraction re-cut into a mould of 100 — not a calculation.
- **The same rule decides both.** A denominator built only from **2s and 5s** gives a decimal that stops, because 10 = 2 × 5. And **100 = 2 × 2 × 5 × 5**, so that identical rule decides whether the percent is clean. A fraction with a repeating decimal has a repeating percent for exactly the same reason — verified across every fraction with a denominator below 100.

Repeating decimals then run through the whole site rather than sitting in one lesson:

- **Correct notation everywhere.** A repeating decimal renders with a proper vinculum, and the bar covers only the digits that actually repeat.
- **Station 01** teaches *that* it happens and the 2s-and-5s rule that predicts it.
- **Station 04's Remainder Belt** teaches *why* it is unavoidable. A crate carries each remainder to a stamper; if the remainder is not zero, a return chute sends it back. On a repeating decimal the machine physically cannot stop — the student has to shut it down. It prints the real long division as it goes.
- **Challenge 9 (Stamp the Bar)** assesses the skill students actually fail: placing the bar over exactly one period, starting where the repeat truly starts.

## What Mr. Fraction does

The speech bubble is not decoration. It carries three jobs the screen cannot.

**It walks through simplifications the screen performs silently.** Station 03 shows an answer as counted and then in simplest form, so a student who works out `6/8` also sees `3/4`. The bubble gives the route between them:

> You worked out **12/18**, and its simplest form is **2/3**. Here is the route: 12/18 ÷ 2 → **6/9**, then 6/9 ÷ 3 → **2/3**. Or in one go — both divide by **6**.

Composite factors are staged, because a student who cannot spot 6 can usually spot 2. Top-heavy results get the mixed number as well. Already-simple answers produce no dialogue at all. This fires on all four operations, in the Simplifier, and on a wrong lowest-terms answer in Challenge 4.

**It adapts to whether the student has done the Division Workshop.** Before: *"This one is really a division question underneath — the workshop is three short steps."* After: the workshop's own language everywhere, so the Remainder Belt becomes *"every line in that log is one workshop round: deal what you can, exchange the leftover for ten, go again."* Two wrong answers on anything division-shaped from someone who has never opened it, and he offers it with a working button.

**It occasionally makes a joke.** Fifteen of them, rationed by three rules: never while the student is on a wrong streak, never in the middle of an explanation, and never within four exchanges of the last one. A joke landing on someone who is stuck reads as being laughed at.

> *"I asked a repeating decimal when it would be finished. Still waiting."*

## Classroom testing

The site has been tried with a few students and a teacher. Their responses were positive, and the site generated general interest. Their feedback led directly to the Station 03 rebuild below, the pizza fix in Bay A, and the Reading & Access panel.

## Station 03, rebuilt after classroom feedback

A teacher and their students found the first version of Operations hard to read. Each change below answers something they reported:

- **No "Whole Numbers" control.** It only set how many empty bars were drawn, but everyone read it as the whole part of a mixed number. Students now pick the piece size (▲▼) and shade pieces, and a new empty whole appears once the last one is full. So 7/4 grows into a second bar, and the readout says *"that's 1 and 3/4"*.
- **No sliders.** ▲▼ steppers and typed boxes replace them, in line with the ▲▼-over-drag rule below.
- **Re-cut keeps the amount.** Changing a denominator used to wipe out the fraction that was there, so it wasn't clear whether to build equivalents from the given fractions. "Cut every piece into 2/3/4/5" multiplies the top and bottom together, and the starting fraction stays on screen.
- **Solve always works.** With different denominators it used to switch itself off. Now it walks through each step: compare the pieces, predict a size both can be cut into, re-cut, combine, and simplify. Multiplying and dividing use the same step-by-step format. In × the student predicts how many pieces one whole is cut into (rows × columns), which is why the tops multiply and the bottoms multiply. In ÷ both fractions are re-cut to one size and the student counts how many B fit inside A, with flip-and-multiply shown as a check, not as the method.
- **Operation signs can't be confused with fraction signs.** The operation buttons are neutral ink and carry their names (add, subtract, multiply, divide). The colours that belong to Fraction A and Fraction B are never used for an operation. The problem is written out as `A (op) B = ?`, with negatives in parentheses: `2/5 − (−3/5)`.
- **One "Negative" box per fraction, and a number line.** The old sign control was a +/− pair that looked just like the operation buttons. A station-wide "use negatives" switch was tried and dropped as redundant. Now each fraction has a single box at its top. The old bars drew negative fractions using their absolute values, so −13/5 + 2/5 showed 13 shaded pieces. A bar can't show a negative amount, so adding and subtracting with negatives is drawn as a move along a number line.
- **The LCD message is no longer canned.** It used to fire on every slider tick, and it asked "why not 4×3?" even when the LCD *was* 4×3. Now it speaks once things settle, and it explains differently depending on whether the denominators share a factor.

## Design priorities

- **Dyslexia-friendly first.** [Atkinson Hyperlegible](https://fonts.google.com/specimen/Atkinson+Hyperlegible) throughout, generous spacing, high contrast, left-aligned body text, and plain-language explanations.
- **Let it fail first.** The Mixing Line refuses to add 1/4 and 1/6 and shows the mismatched pieces, so the common denominator is discovered as a solution to a problem the student just hit. The Dividing Machine makes you call it before it runs.
- **Discovery is withheld, not announced.** The Sevenths Wheel will not tell you the pattern until you have checked all six.
- **Dialogue does real work.** Mr. Fraction runs on a small learner model built only from what a student actually does — which fractions they explore, how many terminating versus repeating cases they meet, their prediction accuracy, whether they have been through the workshop. Probes are computed from their own history. After repeated wrong answers he narrows the question, then states the rule outright rather than asking a fifth riddle.
- **Pedagogical accuracy is non-negotiable.** The multiplication area model uses a dynamic multi-unit grid so improper fractions are handled correctly. There is exactly one long-division implementation in the file, shared by every machine that needs it.

## Reading & Access

A panel opened from the top right of every page, or with <kbd>Alt</kbd> + <kbd>A</kbd>. Every option works on every page:

- **Read aloud.** Students can have the whole page read, just what Mr. Fraction is saying, or any text they highlight. There's a Stop button and three speeds, and an option to read Mr. Fraction aloud automatically every time he speaks. It uses the browser's built-in speech, so no audio files are involved. Text is read in short chunks, because some browsers cut off long passages partway.
- **Typeface:** Standard (Atkinson Hyperlegible), Rounded, or Dyslexia-friendly. The last one uses OpenDyslexic when the device has it installed, and a similar font otherwise.
- **Text size:** 100%, 125% or 150%.
- **Page tint:** cream, peach, blue, green or grey. The tint replaces the page colour instead of laying a film over it.
- **Line spacing:** normal or extra.
- **High contrast:** darker text and stronger borders.
- **Reduce motion:** stops the spinning gears, bobbing and sliding. It is off until a student chooses it. The site deliberately does **not** follow the computer's own "animation effects" setting, which is often switched off on school machines. Following it once meant a whole class lost the Factory Floor's box-closing reward without anyone choosing that.
- **Reading ruler:** dims everything except a band that follows the pointer, or the ↑ and ↓ keys.
- **Reset all.**

Settings last for the whole visit and reset on reload. The site stores nothing on the device.

## Accessibility notes

- The repeating-decimal bar is drawn with a CSS `border-top`, **not** the Unicode combining overline (U+0305), which renders inconsistently across fonts and is mangled by screen readers. The visual form is `aria-hidden`, with a spoken form supplied alongside.
- Interactive controls prefer **▲▼ buttons over drag-and-drop** for touch and Chromebook reliability. Challenge 1 still offers drag, implemented with pointer events so it works with mouse and touch alike.
- Colour is never the only signal: fills and cut lines differ in lightness as well as hue.

## Mobile

- Station 03's builders stack below 700px, and the operation buttons become a single row between them.
- Every numeric field opens the right keypad: `inputmode="numeric"` for whole numbers, `inputmode="decimal"` for the decimal and percent boxes.
- Station 03 has ▲▼ steppers and typed boxes for the piece size and the pieces shaded, so nobody has to tap a 5px cell. On touch screens, its steppers and Re-cut buttons are at least 44px.
- Page gutters tighten below 600px, and `@media (pointer: coarse)` puts a 40px minimum on small controls.

## Tech

- **Single self-contained HTML file** — no build tools, no frameworks, no dependencies to install. One `<style>` block, one `<script>` block, zero external JavaScript.
- Plain HTML / CSS / JavaScript.
- Fonts are **self-hosted** in `assets/fonts/` (about 84 KB of woff2): Atkinson Hyperlegible, plus Black Han Sans and Libre Baskerville for display and certificate text. They are the same files the sister sites use, all under the SIL Open Font License. The page makes **no network requests**, so it works offline on a locked-down school machine.
- Deployed via GitHub Pages, using `.github/workflows/static.yml`, on every push to `main`.

## Running it

Just open `index.html` in a browser — or visit the live site above. No server or setup required.

### Image assets

All images are referenced by their exact filenames and must live in the repo root alongside `index.html`:

```
Mr__Fraction_Front.png
Mr__Fraction_Back.png
Mr__Fraction_Left_Side.png
Mr__Fraction_Right_Side.png
Mr__Fraction_Ladder.png
Mr__Fraction_Factory.png
Mr__Fraction_GIF.gif
Gear.png
Pie.png
Pizza.png
```

Don't rename these or change their extensions — the file references them directly, and there are no fallbacks.

### Updating the site

Commit the change and `git push` to `main`. The Pages workflow deploys it within a minute or two. Avoid GitHub's drag-and-drop uploader, which silently flattens folders and would break `assets/fonts/`. GitHub Pages caches aggressively at this file size, so hard-refresh (Ctrl/Cmd + Shift + R) before deciding something is broken.

## Credits

Site created by Claude and Jon Taylor.

Mr. Fraction's Factory was designed and coded by Claude, Anthropic's AI model, across many working sessions, including the Station 03 rebuild, the For Teachers page and the Reading & Access panel.

## License

[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/).

You're free to share and adapt this for non-commercial use, with attribution, as long as you license your version the same way.

[![CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

---

*Built with ❤️ for middle schoolers who just need to see the fraction.*
