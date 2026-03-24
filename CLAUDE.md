# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Purpose

This repo stores a [Starting Strength](https://startingstrength.com/) workout program encoded in [Liftosaur](https://www.liftosaur.com/) format.

- `liftosaur.md` — the workout program (paste into Liftosaur's "Program" editor)
- `Starting Strength Worksheet(3).xlsx` — the original source spreadsheet

## Liftosaur Program Format

`liftosaur.md` uses Liftosaur's plain-text DSL:

```
# Week N
## Workout A/B
<Exercise Name> / <sets>x<reps> <weight> / progress: lp(<increment>, <attempts>, <failures>, <deload%>, <deload_attempts>, <deload_failures>)
```

`lp(...)` = linear progression. Parameters: weight increment, success attempts needed, failure count, deload percentage, deload attempts, deload failures.

Workout A and B alternate each session (A, B, A, B, A...) following the Starting Strength novice linear progression model.
