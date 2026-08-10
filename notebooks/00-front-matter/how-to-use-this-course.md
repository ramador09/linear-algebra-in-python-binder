# How to Use This Course

Fifty-six notebooks is a lot to arrive at cold. This page is the map: what you
need before you start, four routes through the material depending on why you
came, and how the exercises are meant to be worked.

If you would rather just begin, the [Prologue](../prologue/one-matrix-five-factorizations.ipynb)
is designed exactly for that — one $4\times4$ matrix taken apart five ways, in
about an hour, ending on a question the [Epilogue](../epilogue/five-factorizations-one-idea.ipynb)
comes back to answer.

## What you need first

**Mathematics.** A first linear algebra course, or a willingness to look things
up as they appear. You should have seen matrix multiplication and solving
$A\mathbf{x} = \mathbf{b}$; you do not need to remember how. Everything from
vector spaces onward is rebuilt here from the concrete side.

**Python.** Enough to read a `for` loop and call a function. Chapter 0 assumes
nothing about NumPy and builds the array model from scratch, because the
difference between a loop and a vectorised expression is a linear-algebra
question disguised as a programming one.

**A machine.** Every notebook runs in the browser through the Binder or Colab
buttons at the top of each page — nothing to install. Locally, `pip install -r
requirements.txt` and a Jupyter kernel is all it takes.

## Four routes

Each route is a sequence you can follow start to finish without hitting an
unexplained dependency. Numbers are notebook numbers; a chapter's landing page
introduces its own notation.

### The full course, in order (one semester, ~13 weeks)

The intended path. Roughly four notebooks a week, with Chapters V and VIII the
two places where a week buys less ground than you expect.

> Prologue · 0.1–0.3 · I (1.1–1.7) · II (2.1–2.5) · III (3.1–3.7) ·
> IV (4.1–4.5) · V (5.1–5.6) · VI (6.1–6.6) · VII (7.1–7.3) ·
> VIII (8.1–8.7) · IX (9.1–9.5) · Epilogue

If you must cut, cut **VII** and **IX** — they are the two chapters nothing
later depends on. Do not cut 0.2 (floating point); half the course's later
surprises trace back to it.

### The short path to the SVD (15 notebooks)

For a reader who wants the single most useful factorization and the shortest
honest route to it. Everything here earns its place in the final argument.

> Prologue · 0.2 · 0.3 · 1.1 · 1.3 · 1.4 · 2.1 · 2.2 · 2.3 ·
> 3.1 · 3.2 · 4.1 · 4.2 · 4.3 · Epilogue

### The machine-learning route (22 notebooks)

For a reader whose interest is the matrix algebra inside modern models. The
detour through Chapter II is not optional: ridge regression, the pseudoinverse
and the filter-factor picture are the same object, and 8.1 assumes you have met
it.

> 0.1–0.3 · 1.1 · 2.1 · 2.3 · 2.4 · 3.1 · 3.2 · 3.3 ·
> 4.1 · 4.2 · 4.3 · 4.4 · 6.5 · 8.1–8.7

Chapter VIII ends at 8.7, "Where Linear Algebra Stops", which is the honest
boundary of the whole approach and the best single argument for reading the
rest.

### The numerical-computing route (19 notebooks)

For a reader who will implement or debug solvers. This is the route where
Chapter V is the destination rather than a detour.

> 0.1 · 0.2 · 1.2 · 1.3 · 2.2 · 2.4 · 3.1 · 3.2 · 3.5 · 3.7 ·
> 4.1 · 5.1–5.6 · 6.3 · 6.4

### A shorter fifth path

If you came for quantum information, 9.1–9.5 need only 3.4 (complex, Hermitian,
unitary), 6.4 (Kronecker products) and 7.1 (index notation) ahead of them. That
is six notebooks to a working CHSH violation, eight for the whole chapter.

## How to work the exercises

Every notebook is the same shape: a short theory section, a **Setup** cell, then
exercises, each closing with a validation cell.

**The Setup cell is not the lesson.** It holds data, an instrument, or something
built from scratch earlier and restated for convenience — it never contains the
method the notebook is about. Where a central method appears, the exercise says
**Write this one yourself**, and it means it.

**The validation cells are the point.** Each prints a ✓ and an independent
check: a closed form, a conserved quantity, an identity the calculation did not
assume. They are not decoration — the course's build fails if any of them fails,
which is what lets the prose make claims in the indicative.

**Solutions are hidden, not absent.** Each exercise ships with a full worked
solution; on the public site the source is stripped and the *output* is kept, so
you can see what the answer should produce before you see how. Instructors can
request access to the un-stripped twin.

**Read the numbers, not just the ticks.** Where a check has thin headroom the
notebook says so. Several passages exist only to show a method failing — 2.4's
deblurring, 5.4's zig-zag, 8.7's region count — and those are the ones worth
slowing down for.

## For instructors

The material is CC BY 4.0 (text) and MIT (code); use it, cut it, re-order it.
Three things may save you time:

- **Every notebook is independently runnable** given its chapter's landing page.
  There is no hidden global state, and no notebook imports another.
- **The manifest is the registry.** `manifest.yml` records, for every notebook,
  what the reader computes, what is plotted, and what is independently checked —
  which is usually faster to read than the notebook when you are deciding what
  to assign.
- **A typeset edition exists.** The whole course is available as a single PDF,
  and each page links a per-notebook excerpt, if you would rather hand out
  something printable than a URL.

If you adopt any of it, I would like to hear about it. Corrections especially.
