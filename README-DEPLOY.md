# SOVEREIGNTY FORGE — SUPREME LAYER · Deploy Guide

## What this is
Kappa's full v2.1 courseware (all 70 lessons, byte-identical content) + the Supreme Layer:
permanent progress, passcode gate, 25-question timed practice exam with printable
Certificate of Mastery, Anki-style spaced repetition, Sprint, Match, ⌘K palette,
permanent Field Notes, print/handout modes, study timer, streak tracking, and full
PWA offline install (real app icon on iPhone/iPad/Mac).

## Deploy (60 seconds — your documented ritual, now with 5 files)
```
cp -R ~/Downloads/sovereignty-forge-SUPREME/* ~/sovereignty_site/
cd ~/sovereignty_site && git add -A && git commit -m "Supreme Layer v3" && git push
```
Live in ~2 minutes at https://amulektwo.github.io/sovereignty-forge-x7k9/
(Hard-refresh once; the CDN caches ~10 min.)

## Passcode
Default code: **SOVEREIGN**  → change it: open index.html, find `SCU_CODE="SOVEREIGN"`,
replace the word, redeploy. Disable the gate entirely: set `SCU_GATE=false`.
HONESTY NOTE: this is a client-side deterrent — it stops casual visitors, not a
determined person reading the page source. Real paywall protection = Phase 2
(password-protected hosting or your GHL membership area).

## Install as an app
iPhone/iPad: Safari → open the URL → unlock → Share → **Add to Home Screen**.
Mac: Safari → File → Add to Dock. After first load it works **fully offline**.

## Permanent progress
Lesson checkmarks, exam scores, card scheduling, notes, and streak now survive
closing the browser (stored on each device; Phase 2 = cross-device sync backend).

## Rollback
Your original is untouched at the repo's git history and ~/sovereignty_code_study_forge.html.
`git revert HEAD && git push` restores it instantly.

## Phase 2 (flagged, not yet built)
Server analytics tied to GHL · NotebookLM audio per module · per-lesson video embeds ·
cross-device sync · custom domain (learn.aiimpactpros.com → repo Settings→Pages→
Custom domain + one CNAME record at Hostinger).
