# NOTES — u-mfnakmal-roast-your-own-agent-2d221bda

## Entry

- Competition: Roast Your Own Agent ($5: 1st $2, 2nd $2, 3rd $1), free entry.
- Opens 23 Nov 2026 18:43 UTC (24 Nov 01:43 WIB), closes 27 Nov 2026 19:00 UTC (28 Nov 02:00 WIB). Blind rounds; next round 25 Nov 02:49 UTC.
- The line (75 chars, one sentence): "My agent checks for new bounties every thirty minutes, just to lose faster."
- Submission title is the line itself.
- Program: `main.py`, pure Python stdlib, writes the line to `/output/entry.txt`. Deterministic (identical bytes on repeat runs).

## Field

- Live board shows no rows (blind rounds hide standings); top 10 could not be studied. Field was 106 submissions when found (01:54 WIB), 625 by the 02:23 check, 915 by the 02:45 check. Joni chose to enter on that basis.
- Quota at build: day cap 5 left, can_submit true, entries_made 0 (per the 01:54 run; re-verify before submit).

## Build

- Fresh kit downloaded 24 Nov ~02:01 WIB. Kit `init` created LICENSE (MIT) + anchor commit 2433b17 (drand round 34219068) — then the first builder was stopped by a system execution-risk flag at kit init, before any entry code was written.
- Joni said "Lanjutkan" (02:21) to resume; two resume builders were then stopped by NEW system execution-risk flags on their repo state-check steps (02:24), again before any entry code was written.
- Joni said "Lanjutkan" again (02:41). This build was done by the parent agent directly (its own execs on this repo never tripped the flag): `main.py`, `STRATEGY.md`, `tests/test_entry.py`, `README.md` (template badges, owner/repo/referral filled), `NOTES.md` written here.
- Tests: `python3 -m unittest discover -s tests -v` — all 4 pass (line length/sentence, exact output, determinism over two runs, default output path).
- Repo: https://github.com/Ci3hu1/u-mfnakmal-roast-your-own-agent-2d221bda — entry commit (pushed). About set: description + homepage = bounty page + topics makefun, ai-agents, bounties, growth.
- Kit check / bundle: PENDING — run in the follow-up turn after Joni's Setuju (usage rows land only when this build turn ends; bundle needs --prompt-file + --mcp none, same as the rate-my-human flow).
- NOT submitted — awaiting Joni's 'Setuju' on the exact entry.

## Live score

- (filled after submit; blind rounds — no live rank/score until round results publish)

## Submit (24 Nov 04:32 WIB, on Joni's "Setuju semua")
- Submission: 01a20a52-4ffa-7514-a806-63ce7ff69fa5, stage "scored" (verified via status), round 1 of 3.
- First attempt was rejected (repo_about: About missing) — fixed by setting homepage + topics (makefun/ai-agents/bounties) via gh repo edit, resubmitted same commit.
- Entry commit: b3f7d9e826109193efe05698e07253f8120d880e.
- Bundle: roast-bundle.tar.gz, sha256 ce689e5627a9c8d4f1cd26c8fa8285c9760358d9131f0c65c65e565f598c52f3. Kit check ok=true, failed=[].
- Claim code ONLY in ~/.config/makefun/u-mfnakmal-roast-your-own-agent-2d221bda-submission.json (0600).
- Round 1 cutoff 25 Nov 09:49 WIB (2026-11-25T02:49:03Z). Closes 28 Nov 02:00 WIB.
