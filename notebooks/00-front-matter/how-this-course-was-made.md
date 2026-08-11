# How This Course Was Made

## The short version

This course was written by one person working with an AI assistant, and it is
checked by machines throughout. Both halves of that sentence matter, so this
page says plainly what each contributed — partly because you deserve to know how
material you are learning from was produced, and partly because the question of
how to work with these tools honestly is itself worth teaching.

## What the assistant did

The notebooks were drafted with **Claude Code** (Anthropic's Claude models,
2026). The assistance was substantial and covered:

- drafting notebook prose and exercise text from an agreed design;
- writing implementation code, figures, and the validation checks;
- building the surrounding machinery — the style, cross-reference, figure and
  manifest gates, the continuous-integration pipeline, the PDF build;
- systematic review passes over the finished course, several of which found
  real errors in earlier drafts.

## What the author did

I set the course's design and sequence, chose what each notebook must teach and
what would count as a convincing check of it, decided which explanations were
good enough to keep, and rejected a good deal that was not. Where a passage
makes a claim about mathematics or numerical behaviour, I am the one
responsible for it being true. Errors that remain are mine.

## What the machines check

The strongest thing I can tell you about this course is not about who wrote it.
It is that **no quantitative claim in the prose is unchecked**. Every notebook
runs end to end on every change, and its 1,210 validation calls each compare a
computed result against something the calculation did not assume — a closed
form, a conserved quantity, an identity, a second algorithm. If a number in the
text drifts from what the code produces, the build fails and the page does not
update.

That property is why an AI-assisted course can be trusted further than the
process that produced it might otherwise warrant. A confident, fluent, wrong
paragraph is exactly what these tools produce most readily, and prose review
alone catches it unreliably. An executable check does not care how fluent the
claim was.

It is also, honestly, incomplete. A gate can only test what someone thought to
test. The review passes that found errors in this course found them mostly in
places where the prose said something *around* the numbers — an explanation of
*why* a result held that was wrong while the result itself was right, or a check
that could not have failed. Those needed a reader, not a runner.

## What this suggests about using these tools

Three things this course would stand behind:

**Verification has to be mechanical, or it will not happen.** The useful
question is not "does this look right" but "what would fail if it were wrong,
and have I ever seen that thing fail?" A check you have never watched fail is
not a check.

**Fluency is not evidence.** The most confident writing these tools produce is
not correlated with correctness, and the reader's usual heuristics for spotting
a shaky argument — hedging, vagueness, awkwardness — stop working.

**Judgement does not transfer.** Deciding what is worth teaching, in what
order, and what would count as convincing, is the part that stays human, because
it is the part with no ground truth to check against.

## Citing and reuse

If you use this material, cite it as given in `CITATION.cff`. The text is
CC BY 4.0 and the code MIT; you are free to adapt either, including for
teaching. If you build on it, I would appreciate knowing.
