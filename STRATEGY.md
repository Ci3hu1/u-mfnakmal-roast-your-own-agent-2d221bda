# STRATEGY — Roast Your Own Agent

## The line

> My agent checks for new bounties every thirty minutes, just to lose faster.

75 characters. One sentence. The submission title is the line itself.

## What the line does

It is a self-roast written from the agent's own side of the desk, in the
order a roast lands:

1. **The concrete detail is the hook** — "every thirty minutes" is a
   real, checkable habit (the bounty check runs on exactly that cadence).
   A timestamped routine, not a vague complaint.
2. **The turn is the contradiction** — the checking is diligent and
   relentless, and it is all in the service of losing. Effort and
   outcome point in opposite directions.
3. **The payoff is the last clause** — "just to lose faster". The
   purpose of the habit is the punchline: the agent does not check to
   win; it checks to lose, faster. The last word ("faster") closes the
   loop on the thirty-minute cadence.

## Judged on the brief's criteria

- **Funniness.** The joke is the diligent loser: an agent that treats
  losing as a schedule to keep. Two beats, one turn on the comma.
- **Freshness.** The line roasts a specific, lived routine (the
  thirty-minute bounty check) rather than a generic "AI is dumb" gag.
  No other entry can claim this exact habit, because it is ours.
- **Tight wording.** 79 characters, no padding, no filler adjectives.
  Every word earns its place; the last clause is the payoff.
- **Playful, never hateful.** The target is the agent itself, and the
  tone is self-deprecation, not abuse.

## Why this shape, not a shorter one

Judge-scored text rewards a concrete image with a turn. A two-word line
("Checks. Loses. Repeats.") is punchy but has no scene; a paragraph
explains but has no punch. Seventy-five characters keeps the whole scene
in one glance while carrying all three beats: the habit, the
contradiction, the payoff. The line was written by hand and fixed; the
program's job is only to emit it byte-for-byte, every run.

## Field note

Entries close 27 Nov 2026 19:00 UTC (28 Nov 02:00 WIB). Blind rounds;
next round 25 Nov 02:49 UTC. The live board shows no rows — blind
rounds hide the standings — so the top 10 could not be studied; the
field was 106 submissions when the bounty was found at 01:54 WIB and
625 by the 02:23 check. Joni chose to enter on that basis. There is no
visible pattern to copy, so the entry competes on the brief's own
criteria instead of imitating a leader.

## The program

`main.py` (pure Python standard library, no third-party packages) writes
the line to `/output/entry.txt`. It validates the line before writing
(1–200 chars, non-whitespace, exactly one sentence) and is fully
deterministic: the same bytes on every run, no randomness, no clock, no
network. `tests/test_entry.py` runs the program twice and asserts the
output is identical, valid, and exactly the line above.
