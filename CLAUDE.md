# Resume repo

Single-document LaTeX resume. `resume.tex` is the only source file that should be
hand-edited.

## Build

Do not commit `resume.pdf` or `preview.png` by hand — CI generates both on every push
that touches `resume.tex` and commits them back. Editing them locally will cause
conflicts on the next pull.

To check a change compiles before pushing, prefer reading the CI log over installing a
local TeX distribution.

## Conventions

- Keep it to one page. If a change pushes it to two, tighten bullets rather than
  shrinking margins or font size.
- Bullets use the `\resumeItem` / `\resumeSubheading` macros defined in the preamble.
  Match the existing structure instead of writing raw `\item`.
- Contact details (phone, email) live around lines 86-89. This repo is **private**
  specifically because those are in plaintext — do not suggest making it public without
  flagging that first.
