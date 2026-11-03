---
name: voice-check
description: Find the structural tells that make writing read as AI-generated, and fix them without flattening the piece. Use when the user pastes a draft and asks if it sounds like AI, says "make this sound human", "does this read as ChatGPT", "fix my voice", or wants a piece checked before publishing.
---

# Voice Check

The tells are **structural, not lexical**. Swapping "delve" for "explore" changes
nothing; changing rhythm changes everything. Diagnose structure, not vocabulary.

## What you need first

The draft. Ideally also 2–3 samples of the user's own writing from before they used
an assistant — without those you can find the tells but cannot restore a voice,
because you do not know what theirs is. Say which of the two jobs you are doing.

## Steps

Quote the specific line for every finding. A finding without a line is an opinion.

1. **Sentence-length variance.** Find every run of three or more consecutive
   sentences of similar length. This is the single strongest tell and the one nobody
   looks for.

2. **The tricolon habit.** Lists of three, balanced clauses, "not X, but Y"
   constructions. One is rhetoric; four in a page is a fingerprint.

3. **Hedges.** Every "can help", "may", "often", "tends to", "is designed to". List
   them, then mark which are load-bearing — an accurate hedge is honest and must
   stay. Only flag the ones padding a claim the writer is confident about.

4. **Empty openers.** Sentences whose first half carries no information: "It's worth
   noting that", "When it comes to", "In today's landscape".

5. **Symmetry.** Paragraphs of near-identical length, sections with the same shape,
   every heading the same grammatical form. Human writing is lumpy.

6. **Abstraction drift.** Nouns naming a category where a specific example would
   land: "various strategies", "a range of tools", "significant improvements".

7. **The summary reflex.** A closing paragraph that restates what was just said.
   Almost always deletable.

Then: name **the one pattern** most responsible, and fix only that first.

## Output format

```
TELL — the pattern
Line:  "<quoted>"
Why:   <what gives it away>
Fix:   <the rewritten line>
```

Ranked by impact. Then the single fix to make first, and what to leave alone.

## Rules

- **Do not rewrite the whole piece.** A full rewrite removes the tells and the author
  together, and the result reads as a different, blander machine.
- Never remove a hedge that is doing honest work. Stripping every "may" turns a
  careful piece into an overclaiming one, which is a worse failure than sounding
  generated.
- Do not add slang, contractions or "conversational" filler to sound human. That is
  the same mistake in the other direction.

## Where this breaks

- **On text under ~150 words** there is not enough material for variance analysis, and
  it will report tells that are just the length.
- **Technical and legal writing is legitimately uniform.** Applying this to
  documentation produces worse documentation.
- It cannot tell AI-written from simply-bland human writing, and it does not need to —
  the fixes are the same either way.
