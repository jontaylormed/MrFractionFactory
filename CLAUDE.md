# Mr. Fraction's Factory — read this first

One file: `index.html` (~515 KB, one `<style>`, one `<script>`). Zero dependencies,
no build step, runs from `file://`. Five stations teach fractions, decimals and
percents as one idea: Job Training, Simplifier, Operations, Converter, Assessment
Bay. The page sections are `#page-home`, `#page-lesson`, `#page-simplify`,
`#page-operate`, `#page-convert` and `#page-factory`.

**`README.md` describes every station and the design rules behind it.** Read the
part you are about to change before changing it. Do not restate it here, because copies drift.

## Where it lives

- `origin` = https://github.com/jontaylormed/MrFractionFactory. A push to `main`
  runs `.github/workflows/static.yml` and deploys to
  https://jontaylormed.github.io/MrFractionFactory/
- `jtaylor-cloud/Mr.FractionFactory` is the retired original. It was imported from
  its 2026-07-28 build. Never push to it or link to it.
- Sister sites share the brand, fonts and palette: `jontaylormed/MrFractionWordExpress`
  and `jontaylormed/MrFractionMiningOperation`.

## Pushing is the user's decision, always

Never `git push`, add a remote, change repo settings or open a PR unless the
user asks in that turn. Approval is per push and does not carry forward. The site is
public, and a push deploys within minutes. Committing locally is normal work:
commit before and after every change.

## The repo is public

No personal info in any tracked file or commit message: no name, email,
Windows username or local paths, school or department. Grep the diff before
committing.

## Rules that keep the site working

1. **Asset names are exact and case-sensitive.** Images sit at the repo root
   (`Mr__Fraction_*.png`, `Mr__Fraction_GIF.gif`, `Gear.png`, `Pie.png`,
   `Pizza.png`), and fonts are in `assets/fonts/`. Pages serves from Linux, so
   case matters there even though Windows hides it. Use relative paths only, never a leading `/`.
2. **No network requests, no localStorage.** Fonts are self-hosted through the
   `@font-face` block at the top of the `<style>`. Ask before adding a CDN, a
   framework, a build step or any persistence.
3. **Edit with `Edit`, anchored on unique text.** The file is huge and
   repetitive, so a short anchor can match the wrong place. Never bulk-replace through a shell.
   In PowerShell, read it as UTF-8 explicitly
   (`[IO.File]::ReadAllText($p,[Text.Encoding]::UTF8)`), or em-dashes and
   symbols get corrupted.
4. **Keep the README's pedagogy and accessibility rules:** exactly one shared
   long-division implementation; ▲▼ buttons over drag; colour is never the only
   signal; the repeating bar uses `border-top`, not U+0305; let the student fail
   first; withhold discoveries instead of announcing them; keep Mr. Fraction's joke rationing.
5. **Read the stat line.** Run `git diff --stat` before every commit. If a deletion
   can't be explained, stop.

## Verifying a change

- Open in Edge with a percent-encoded path, because a bare path splits on spaces:
  `Start-Process msedge ('file:///' + ((Resolve-Path index.html).Path -replace '\\','/' -replace ' ','%20'))`
  Then press Ctrl+Shift+R, check the console for errors, and click through the station you changed.
- After a push, check the **deployed** site, not this folder. A changed asset
  should return 200, and a mis-cased copy of its name must return 404, or the check proved nothing.
- Measurement proves geometry, not appearance. Whether it *looks* right is the
  user's call, so say which one you checked.
