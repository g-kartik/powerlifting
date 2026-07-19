# Post-SS ATG for Life — Progression Evidence Review

Companion to `tibialis_research.md`, extended to the rest of `post-ss-atg.md`. Goal: pick a progression model (`lp()` linear vs `dp()` double progression vs none) for each exercise based on how it's actually trained in the literature/practice, not a blanket default.

---

## Bucket 1 — Linear Progression (`lp`)

Exercises where the real-world protocol is "add small load once you clear the prescribed reps," with no meaningful rep-range component.

### Reverse Sled Drag

**Sources:**
1. Sled-pull load-velocity profiling research (young athletes) — PMC. Load prescription is traditionally %BM-based, progressed incrementally. **Credibility:** peer-reviewed, but population is sprint athletes, not accessory/rehab work at this scale. ([PMC6572326](https://pmc.ncbi.nlm.nih.gov/articles/PMC6572326/))
2. Mountain Tactical Institute case study — sled drag load progressed from 90kg to 380kg over 6 weeks in a tactical-fitness context. **Credibility:** practitioner case study, not RCT. ([mtntactical.com](https://mtntactical.com/knowledge/case-study-loaded-sled-drags-demonstrate-transferability-to-uphill-movement-under-load/))
3. RPE-anchored protocol: increase load only when RPE is below 8. **Credibility:** commonly cited coaching heuristic in the sled literature.

**Verdict:** Sled research is almost entirely sprint/speed-focused (%BW loading, velocity-decrement zones) and doesn't transfer cleanly to a 1x1 bodyweight-sled accessory set. No rep range to progress — this is a straightforward "add load when it's easy" case. Use `lp()`, but gate it on 2 successful pulls (not 1) since sled work has no rep ceiling to signal readiness the way a rep-range movement does.

### Neck Harness Flexion / Extension

**Sources:**
1. 14-week neck-strengthening protocol (novel device, self-generated centripetal force) — significantly improved isometric strength and RFD in cervical extension/lateral flexion. **Credibility:** peer-reviewed (PMC/ScienceDirect). ([PMC11624327](https://pmc.ncbi.nlm.nih.gov/articles/PMC11624327/))
2. Rugby U19 RCT — tailored neck program improved strength/fatigue markers over a season. **Credibility:** peer-reviewed RCT, but youth rugby population. ([PMC4427068](https://pmc.ncbi.nlm.nih.gov/articles/PMC4427068/))
3. Iron Neck / elite-program guidance — progression sequence is static → slow dynamic → fast dynamic → reactive, 2-3x/week, progressive overload. **Credibility:** vendor content, directionally consistent with the peer-reviewed sources above.

**Verdict:** All sources agree on progressive overload at 2-3x/week, but none suggest a rep-range/double-progression model — neck work in the literature is dosed by session count and load, not rep bands. Supports `lp()`. Given the neck is a small, slow-adapting joint with a real injury cost if rushed, use a 3-success-attempt gate (not the default 1) before adding load — more conservative than the other `lp()` exercises.

### Seated Good Morning

**Sources:**
1. EMG load-response study — hamstring and erector spinae activation increases proportionally with load (tested 50-90% 1RM). **Credibility:** peer-reviewed (PMC). ([PMC4304869](https://pmc.ncbi.nlm.nih.gov/articles/PMC4304869/))
2. General coaching consensus — beginners should master bodyweight/dowel hinge pattern before adding external load; train 1-2x/week, not after heavy squats.

**Verdict:** Load-activation relationship is linear and monotonic — more load simply drives more posterior-chain activation, no rep-range ceiling effect described. Supports `lp()`. Given the "master the hinge before loading" guidance and the exercise's lower-back involvement, gate on 2 successful sessions rather than 1.

---

## Bucket 2 — Double Progression (`dp`)

Exercises where the real-world protocol/practice is rep-range driven: work in a rep band, and only add load once the top of the band is hit for all sets. This is how these are actually trained in the sources below, so `dp()` fits the intent better than `lp()`.

### Poliquin Pulse / ATG Split Squat Pulse (partial-ROM pulses)

**Sources:**
1. SportRxiv preprint — lengthened partial reps produce muscle growth comparable to full-ROM reps in trained lifters. **Credibility:** preprint, not yet peer-reviewed, but methodologically sound. ([sportrxiv.org](https://sportrxiv.org/index.php/server/preprint/view/455))
2. Stronger by Science research spotlight — partials in the stretched position can match or exceed full-ROM growth (calf raise data specifically). **Credibility:** research-translation outlet, cites underlying peer-reviewed work.
3. ACSM position stand (via search synthesis) — muscular-endurance training uses 10-15 reps for novices, 15+ for advanced, at lighter relative loads.

**Verdict:** Nothing in the partial-rep literature implies a different progression *model* than any other accessory movement — these are just high-rep, light-load endurance work. Rep-range double progression is standard practice for this training mode. Narrow both exercises to a rep band and use `dp()`:
- Poliquin Pulse: 50-75 reps (was fixed at 75) → `dp(1.25kg, 50, 75)`
- ATG Split Squat Pulse: 30-50 reps (was fixed at 50) → `dp(2.5kg, 30, 50)`

### Reverse Squat (cable hip flexor raise)

**Sources:**
1. Practical coaching guidance (Motra, StrengthLog exercise guides) — once 10+ reps achievable with a controlled 2-3s eccentric, add small load (ankle weight/cable stack increment). **Credibility:** practitioner content, not peer-reviewed, but consistent across multiple independent sources and matches general cable-isolation practice.

**Verdict:** Sparse peer-reviewed literature specifically on cable hip-flexor progression exists — this is a case where the practical consensus (rep-cap-then-load) is the best available evidence. Textbook double progression. Narrow to 15-20 reps (was fixed at 20) → `dp(2.5kg, 15, 20)`.

### ATG Back Extension

**Sources:**
1. Biomechanical comparison, reverse hyper vs. back extension (PubMed, 20 subjects) — back extension produced greater erector spinae/glute/biceps femoris activation than reverse hyper. **Credibility:** peer-reviewed. ([PubMed 30946266](https://pubmed.ncbi.nlm.nih.gov/30946266/))
2. Coaching consensus (BarBend, Fitness Volt, TrainHeroic) — progression path is explicitly staged: reps first, then tempo, then load (ankle weights or DB between feet); rep ranges cited 12-25.

**Verdict:** The staged reps→tempo→load progression described across sources is double progression by definition, not linear. Narrow to 15-25 reps (was fixed at 20, giving room in both directions) → `dp(2.5kg, 15, 25)`.

### ATG Incline Press / ATG Incline Row (dumbbell)

**Sources:**
1. Double-progression method overviews (mesostrength, fitbudd, liftproof) — standard practice for dumbbell work specifically *because* DB weight jumps are coarse (2.5-5kg per side); a wider rep band absorbs the coarse jumps better than fixed reps + linear load. **Credibility:** practitioner/coaching content, consistent with the underlying logic of DB equipment constraints (not really a study-backed claim, more an equipment-driven necessity).
2. General hypertrophy rep-range research — 8-12 (novice-friendly, faster progression) to 10-15 is standard for compound dumbbell accessory work.

**Verdict:** This is less about specific research on these exact movements (no studies target "ATG incline press") and more about the well-established practice of pairing dumbbell equipment with double progression due to plate-jump granularity. Narrow both to 10-15 reps (was fixed at 15) → `dp(2.5kg, 10, 15)` each.

### Pulldown / Band Pushdown

**Sources:**
1. Lat pulldown reviewed as appropriate for novice progression/regression for upper-body pulling strength. **Credibility:** general exercise-science reference content.
2. Triceps hypertrophy research (Stronger by Science) — direct triceps work responds well to controlled tempo (paused reps, slow eccentric) in the 8-12 rep zone, trained 2x/week.

**Verdict:** Same logic as the DB press/row — standard cable-accessory practice is rep-range-capped then load-bumped. Narrow:
- Pulldown: 10-15 reps (was fixed at 15) → `dp(2.5kg, 10, 15)`
- Band Pushdown: 25-35 reps (was fixed at 35) → `dp(2.5kg, 25, 35)`

### Gripper

**Sources:**
1. Grip-training guidance (goldengrip.com, gripboard.com) — start at a resistance you can do 10-12 controlled reps with; once 15+ reps easy, move up in resistance (~5kg equivalent). **Credibility:** practitioner/community content, but consistent across independent sources and matches "Grease the Groove" (Pavel Tsatsouline) practice.
2. Systematic review/meta-analysis on hand-focused strength training — progression is typically dosed as %1RM or %MVC increases over time. **Credibility:** peer-reviewed (PMC). ([PMC12524766](https://pmc.ncbi.nlm.nih.gov/articles/PMC12524766/))

**Verdict:** The rep-cap-then-increase-resistance logic is identical to `dp()` — but hand grippers are sold as discrete fixed-resistance tools (not continuously plate-loadable), so a `dp(Xkg, ...)` weight increment doesn't correspond to anything purchasable. **No Liftoscript progression added.** Recommendation stays qualitative: once 20/20 reps across all 3 sets feels easy for 2+ sessions in a row, manually swap to the next-heavier gripper and reset the exercise weight in Liftosaur.

---

## Bucket 3 — No Weight Progression

### Standing Pancake

**Sources:**
1. Pancake-stretch progression guides (Journey to Mobility, Lattice Training, Emmet Louis) — explicit warning that "weight should only be used to pull you slightly deeper... don't overdo it," and that most of a stretch's ROM gain happens in the first 15-30s regardless of load. **Credibility:** practitioner/coaching content, consistent across multiple independent sources.

**Verdict:** This is a mobility drill, not a strength exercise — the literature actively discourages a load-progression mindset here. Progress via depth/ROM staging (supported tall sit → hinge → deeper fold), which isn't something `lp()`/`dp()` can track. **No change** — stays without a `progress:` line.

---

## Summary Table

| Exercise | Old scheme | New scheme | Rep range change |
|---|---|---|---|
| Reverse Sled Drag | `lp(2.5kg)` | `lp(2.5kg, 2)` | — |
| Neck Harness Flexion | `lp(1kg)` | `lp(1kg, 3)` | — |
| Neck Harness Extension | `lp(1kg)` | `lp(1kg, 3)` | — |
| Seated Good Morning | `lp(2.5kg)` | `lp(2.5kg, 2)` | — |
| Poliquin Pulse | `lp(1.25kg)` | `dp(1.25kg, 50, 75)` | 75 fixed → 50-75 |
| ATG Split Squat Pulse | `lp(2.5kg)` | `dp(2.5kg, 30, 50)` | 50 fixed → 30-50 |
| Reverse Squat | `lp(2.5kg)` | `dp(2.5kg, 15, 20)` | 20 fixed → 15-20 |
| ATG Back Extension | `lp(2.5kg)` | `dp(2.5kg, 15, 25)` | 20 fixed → 15-25 |
| ATG Incline Press | `lp(2.5kg)` | `dp(2.5kg, 10, 15)` | 15 fixed → 10-15 |
| ATG Incline Row | `lp(2.5kg)` | `dp(2.5kg, 10, 15)` | 15 fixed → 10-15 |
| Pulldown | `lp(2.5kg)` | `dp(2.5kg, 10, 15)` | 15 fixed → 10-15 |
| Band Pushdown | `lp(2.5kg)` | `dp(2.5kg, 25, 35)` | 35 fixed → 25-35 |
| Gripper | none | none (manual swap) | — |
| Standing Pancake | none | none | — |
| Tibialis Raise | `dp(2.5kg, 15, 20)` (unchanged, already evidence-based) | — | — |
| Pull Up | `lp(0kg, 2)` (unchanged, out of scope — flagged separately) | — | — |
