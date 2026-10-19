# The clinic carnet: what students have to learn, and how the week teaches it

> **Decisions taken (owner, 2026-10-14):**
> - **Scope:** full redesign of `carnet.html`. The game and the calculators are kept.
> - **Thinking structure:** causal maps that students build. Monday gives a worked-example core;
>   Tuesday's loops are built by the students themselves.
> - **Tuesday:** the owner's design. Each team builds a loop to improve one focal variable. A
>   boundary debrief follows, then a merge into one large loop showing delays, limits and tipping
>   points. Run as a **jigsaw**: one focal variable per team, then mixed groups merge.
> - **Focal variables:** the game's four viewpoints. Monday builds the money loop; Tuesday's teams
>   take access to care, team climate and carbon footprint.
> - **Method:** a named reasoning cycle, shown to students.
> - **Sources:** objectives derived from what exists (the owner's aim, the current carnet, the game
>   model, Friday's proposal). There are no separate course sources for the clinic.
> - **Objectives O1–O6 confirmed** (§3).
> - **Three teams, always.** Each team takes one Tuesday focal variable. The jigsaw groups each
>   have one member from every team.
> - **The surgery case moves to Wednesday.** It is the margin-per-hour question, which is
>   Wednesday's topic. Tuesday's numbers block becomes one short break-even calculation.
> - **Monday's free play stays short** (10 min).
> - **Clock:** every session is planned for **9:00–11:30**. **12:00** is a hard maximum, kept as a
>   buffer and never planned into.
> - **Load comes first** (§7a). Students need time to understand a concept, then to see it happen
>   in the game. The carnet asks for few written outputs so that time goes to thinking and
>   trying, not to filling in forms.
> - **The work is not graded.** Grading weights and levels leave the carnet. The criteria stay as
>   "ce qui rend une proposition défendable", a self-check.
> - **Facilitator notes** go in a separate file, `notes-animateur.html`, which is not linked from
>   the carnet.

Written for the owner. Nothing in `carnet.html` has changed yet.

---

## 1. What the carnet should teach

Four things, in the owner's words:

1. **A way to organise thinking about a clinic.**
2. **Economics as a tool for that thinking.** It is not a separate subject.
3. **Applying it to one particular case**, to make propositions that are objective. Here
   objective means traceable, compared with doing nothing, and conditional.
4. **Placing it in context** with the thinking structure: causal maps, their boundary, and the
   viewpoint adopted.

The end point is the same as before. On Friday a team answers Dr Neri's proposal with figures they
produced, and they know the limits of those figures. What changes is *how* the week gets them there.

## 2. What the current carnet gets wrong

| # | Problem | Evidence |
|---|---|---|
| 1 | **Organised by tools, not by thinking.** The week table's third column is "Ce que vous apprenez à calculer". Each day adds two or three calculators. | Accueil §04 |
| 2 | **The thinking structure arrives late and finished.** The loop appears only on Tuesday, as a fixed five-variable SVG; students only tick S/O. It is absent on Monday, Wednesday and Thursday, and it returns once on Friday. | Mardi §03–04 |
| 3 | **Economics and the map never meet.** The loop has no price, no costs and no margin, which is where every calculator works. Nothing tells students that the break-even point answers a question about the Cas traités → Résultat arrow. | Mardi §04–05 |
| 4 | **The method is implicit until Friday.** Each day's situation is a separate puzzle. The four-part answer (affirmation, éléments, condition, risque) is met once, on the day it is assessed. | Vendredi §03 |
| 5 | **Context is a separate day.** Boundary and viewpoint ("vu d'où ?") appear only on Thursday, not as a step of every proposition. | Jeudi §03 |
| 6 | **Instructions are prose.** Blocks mix explanation, steps and questions. Nothing states what "done" looks like, so students cannot check themselves. | all days |
| 7 | **Monday: before/after taken for with/without.** The year-on-year change in the game mixes the decision with the 60 % first-year ramp-up, staff climate and client growth. (With exact forecasts, the setting used, demand does not vary: the realised year equals the plan. Checked in `app.js:1008`, 2026-10-16.) | `app.js:1007`, `:13`, `:682` |
| 8 | **Monday: no completed year at the start.** Year 1 shows a forecast only (exact by default). | `app.js:155` |
| 9 | **Terms used before they are defined.** Monday asks for observation, then defines demandes, coûts variables, etc. afterwards. | Lundi §01–02 |
| 10 | **Dr Neri's letter comes too late.** It is printed only on Friday, but Wednesday asks for "le premier jet" of the reply. | Mercredi §06, Vendredi §02 |
| 11 | **Years do not add up.** Accueil says six years, the clinic's targets say year 4, and the default target year is 4. | `carnet.html:252`, Référence, `app.js:193` |

**What works and stays:**
- the calculators and their wording;
- the with/without comparison (*analyse différentielle*) and the Référence / Planifié columns;
- the practitioner's two-column notes on Thursday;
- the Friday three-year table and the 100 / 80 / 60 table;
- the grading criteria;
- the rule that every figure comes with its calculation and its screen;
- the figure checks in `outils/verifier-chiffres.js`.

## 3. Proposed objectives (yours to confirm)

Each objective names what a student must be able to produce, so it can be seen in the dossier.

| | Objective | Observable in the dossier |
|---|---|---|
| **O1** | **Read a clinic.** Describe it in figures: stock vs flow, demand / capacity / cases served, fixed vs variable costs. Each figure comes with its screen and its year. | The indicator table; each node of the map carries a figure |
| **O2** | **Build, bound and merge causal maps.** Mark S or O on each arrow. Show delays, ceilings and tipping points. Say what is included and what is left out. Join loops into one system. | Maps v1 → v4; a list of what is inside and outside the boundary |
| **O3** | **Choose the tool the map calls for.** Pin each economic tool to the arrow whose question it answers, apply it, and call it by its professional name. | Each calculation is labelled with its arrow |
| **O4** | **Compare with and without, under uncertainty.** Judge a decision against "no change" over several years, and say how much error it tolerates. | Decision record (Référence / Planifié / réalisé); the 100 / 80 / 60 table; margin of safety |
| **O5** | **Frame.** Name the viewpoint, the model's boundary, and the relevant, sunk and opportunity costs. | One sentence on the viewpoint in each proposition |
| **O6** | **Propose and revise.** Claim, figures, a checkable condition, a risk. Revise when new data arrives. | One four-part proposition per day; Friday's is the fifth |

## 4. Instructional design

### The backbone: 4C/ID

The week ends in one complex whole task: the reply to Dr Neri. The *Four-Component Instructional
Design* model (van Merriënboer & Kirschner, *Ten Steps to Complex Learning*) is built for exactly
this.

| Component | In the carnet |
|---|---|
| **Learning tasks**: whole tasks, simple to complex, support fading | One case per day, each taken through the whole cycle. **Mon:** the partner's +20 % price rise, as a worked example. **Tue:** the team's own clinic, mapped and taken to break-even, each step prompted. **Wed:** "plus de chirurgie" and their own clinic, done alone. **Fri:** Dr Neri, unaided. |
| **Supportive information**: mental models and strategies | The maps and the cycle. They are given *after* students have tried, then reused every day. |
| **Procedural information**: just in time | Calculator cards and "Où lire" lines. Each appears at the step that needs it, never as a block at the start. |
| **Part-task practice** | Short drills where automaticity matters: S or O on an arrow, stock or flow, fixed or variable. |

### Each day follows Merrill's First Principles

1. **Activation.** Reopen yesterday's map and diagnosis.
2. **Demonstration.** One worked example. If a behaviour did not occur in a team's game, the carnet
   gives a short example computed from the model, then asks "est-ce que cela explique quelque chose
   chez vous ?". Tuesday's synthesis no longer depends on luck.
3. **Application.** The day's case, with that day's level of support.
4. **Integration.** Revise the dossier and write the day's four-part proposition.

### Where students invent first, and where they are shown first

- **Maps: invent, then name** (Schwartz & Bransford, *A time for telling*, 1998; Kapur, productive
  failure). Students try to build a loop before the vocabulary of delay, ceiling and tipping point
  is given. The words then name what they ran into. This keeps the original Monday intent ("ce que
  vous aurez remarqué vous-même est ce que nous nommerons ensuite") but moves it to where
  construction happens.
- **Cycle and calculations: worked examples, then fading** (Renkl; Sweller, cognitive load). The
  method has many steps and errors cost a lot, so it is shown whole first, then its support is
  removed one day at a time.
- **Jigsaw** (Aronson) for Tuesday's merge. Each person carries one loop into a mixed group, so the
  merge cannot happen without every person explaining their arrows.

### Instructions students can follow alone

Every activity block uses one template. A verifier rule will check that every field is present.

> **Objectif** — one sentence
> **Durée** — minutes
> **Étapes** — numbered, one action each
> **Où lire** — screen › card, exactly as the game labels it
> **Vous avez fini quand…** — an output the student can check
> **Si vous bloquez** — one hint

Two further rules:
- **One new term per step**, defined where it appears. Hover tooltips are not used.
- **No forward reference** that a student cannot act on yet.

### Records they can return to

The shared document becomes **one dossier with five parts**, revised every day instead of having a
section added:

1. **Carte** — v1 to v4.
2. **Tableau** — indicators, with screen and year.
3. **Journal des décisions** — for each year:
   - before passing it: décision, effet attendu, Référence, Planifié;
   - after passing it: réalisé, ce qui reste à expliquer.
4. **Diagnostic** — observation kept separate from explanation; what would test the explanation.
5. **Proposition** — the four parts, rewritten each day.

Every later step is built on these records, Friday's presentation included.

## 5. The named cycle

**Décrire → Situer → Expliquer → Chiffrer → Comparer → Cadrer → Proposer** — then *Réviser*.

| Step | What students do | Dossier part |
|---|---|---|
| **Décrire** | Figures from their clinic, each with its screen and year | Tableau |
| **Situer** | Place the problem or decision on a node or arrow of the map | Carte |
| **Expliquer** | A causal explanation, kept separate from the observation, and what would test it | Diagnostic |
| **Chiffrer** | The tool pinned to that arrow, called by its name | Diagnostic |
| **Comparer** | Planifié − Référence sans action is the effect; réalisé − Planifié is the uncertainty | Journal |
| **Cadrer** | Viewpoint, boundary, costs that count | Proposition |
| **Proposer** | Affirmation · éléments · condition · risque | Proposition |

Cadrer is introduced lightly on Tuesday, through the boundary debrief, and fully on Thursday.

## 6. The maps, day by day

Every arrow, sign, threshold and delay below exists in the model. A verifier rule will assert each
one: it changes the cause in `simulateYear` and checks the direction of the effect.

| Model feature | Where | On the map |
|---|---|---|
| Price reduces demand (elasticity per service) | `data.js` services, `app.js:801` | Prix → Demandes (O) |
| Client trust raises demand | `app.js:824` | Confiance → Demandes (S) |
| First-year ramp-up: 60 % of demand | `app.js:13` | **delay** on Capacité → Cas traités |
| Overtime paid ×1.25, capped at 130 % | `app.js:9–10` | Heures sup. → Coûts (S) |
| Overtime lowers climate; last year's overtime adds this year's absence | `app.js:1135`, `:686` | Heures sup. → Climat (O); **delay** to Absence |
| Climate < 50 raises absence | `app.js:682` | Climat → Absence (O) |
| Climate < 30: a resignation at year end | glossary; verify in code | **tipping point** |
| Requests for services not offered | `app.js:2264` | **ceiling**: a finite market |
| Carbon per case target (−15 %, keeping 80 % of volume) | `app.js:1307` | Cas traités → Carbone (S); per-case levers |

**Monday — the money loop (worked example).** Demandes → Cas traités → Recettes and Coûts
variables → Résultat net → Trésorerie; Capacité → Cas traités; Coûts fixes → Résultat net (O);
Prix → Recettes (S) and Prix → Demandes (O). Students place their year-1 figures on the nodes and
mark each node as a stock or a flow.

**Tuesday — the owner's design, as a jigsaw.**

The clock-time version of this design is in §7a.

**Wednesday — alone.** The Capacité node opens into vet hours, support hours, rooms, equipment and
skills. The constraint is the smallest of these. Students cost the three situations they met (a full
room, overtime, ramp-up) and rank services by margin per hour of the scarce resource. They predict
the constraint before passing a year. Cycle pass #3 ends in a first draft of the reply to Dr Neri.

**Thursday — boundary, second pass.** The practitioner's words are sorted against the merged map:
what is inside, what is outside, what no viewpoint reaches. The game's "Mieux ou moins bien — vu
d'où ?" is read as four loops the students built, not as four scores. Relevant, sunk and opportunity
costs are introduced, and **Cadrer** is applied to Wednesday's draft.

**Friday — unaided.** Students save the clinic, then test each option from that same point: buy or
lease, train or hire. They compare three years with and without the project and fill the
100 / 80 / 60 table. They place the proposal on the map (which arrow, what delay, what stops it) and
state the viewpoint and the condition.

## 7a. Time and load: the rules every day follows

1. **Understand → see it → use it.** Each new idea gets three moments: a short explanation, a
   step where students *watch it happen in the game*, then one use on their own clinic. The middle
   step costs time and is never cut.
2. **No more than four new terms in a session block.** Anything beyond that waits for the next
   block or the next day.
3. **Few outputs, revised rather than multiplied.** A day asks for at most four short things in
   the dossier. A map drawn on paper and photographed counts; nothing needs retyping.
4. **One decision per year** when playing. It keeps the with/without reading simple.
5. **Every block says when it is finished**, so nobody keeps filling in.
6. **Planned to 11:30, never to 12:00.** The last 30 minutes absorb slow starts, game hiccups and
   discussion.
7. **One 10-minute break** around 10:00–10:45, at a natural seam.

### Monday, 9:00–11:30: "Lire une clinique"

| Time | Block | Students do | Output |
|---|---|---|---|
| 9:00 | Ouverture (10) | Hear Dr Neri's letter; see the cycle; set roles | — |
| 9:10 | Premier regard (10) | Free look, one question, **do not pass the year** | — |
| 9:20 | La carte de l'argent (30) | Copy the map; find each figure on its screen; box the stocks | Map v1 with 9 figures |
| 9:50 | La proposition de l'associé (40) | The cycle, step by step, as a worked example | 4-line reply |
| 10:30 | Pause (10) | | |
| 10:40 | Deux années (35) | One decision per year; Référence / Planifié before, réalisé after | 2 journal rows |
| 11:15 | Premier diagnostic (15) | Observation · explanation · what would test it · a question | 4 sentences |
| 11:30 | *end — buffer to 12:00* | | |

### Tuesday, 9:00–11:30: "Voir le système"

| Time | Block | Students do | Output |
|---|---|---|---|
| 9:00 | Reprise (10) | Each team reads its question from Monday | — |
| 9:10 | Votre variable (35) | Home team builds a loop around its focal variable; tests one arrow in the game | Loop on paper |
| 9:45 | Ce que vous avez laissé dehors (15) | What did we include, what did we leave out? → périmètre | 3 lines |
| 10:00 | Pause (10) | | |
| 10:10 | Assembler (30) | Jigsaw groups join the three loops and Monday's money map | One merged sheet |
| 10:40 | Ce que la grande boucle montre (20) | Teacher synthesis: délai, plafond, seuil de basculement, contrainte; each one shown in the game | — |
| 11:00 | Combien faut-il ? (25) | Break-even and margin of safety on their own clinic, written next to Cas traités | 2 figures on the map |
| 11:25 | Retour (5) | Home team: photograph the merged map; one sentence revising the diagnosis | 1 sentence |
| 11:30 | *end — buffer to 12:00* | | |

### Tuesday revised: the case is back (owner, 2026-10-14)

Tuesday now has its case: **« Augmentons tout le monde de 10 % »**, taken through the seven steps with a prompt at each, and with break-even and margin of safety inside it. Timings: Reprise 10 · Votre variable 30 · Dehors 10 · pause 10 · Assembler 25 · Grande boucle 20 · Le cas 40 · Retour 5.

Checked in the model: on the starting clinic, a 10 % rise adds 10 370 € of fixed costs. Break-even moves from 3 462 to 3 710 cases. Cases served stay the same. Climate moves from 49 to 53, crossing the absence threshold at 50. The explanation "l'équipe est usée" is wrong at the start: the team is under-used (37 %), and a workload below 45 % also lowers the climate. The viewpoints disagree.

### Wednesday, at home, 150 min

Reprise 10 · « Faisons plus de chirurgie » 40 (margin, margin per hour) · Ce qui limite votre clinique 30 (constraint analysis) · Prévoir, puis vérifier 20 (pass year 4) · Premier jet pour la Dre Neri 40 (indifference point → payback period) · Une question pour jeudi 10.

### Thursday, 9:00–11:30: the practitioner is retired and does not know the clinic

Avant qu'il commence 5 · La rencontre 90 · pause 10 · Ce que la carte compte 25 (second pass on the boundary) · Cadrer votre premier jet 20 (relevant, sunk and opportunity costs; viewpoint). Each team brings **one general question from Wednesday**, asking for a story: time, opening a service, the team, a money decision. No questions about the simulation.

### Friday, 9:00–11:30

Ouverture 5 · Tester sur trois ans 50 (from a saved clinic: without, then with) · Si la demande n'arrive pas 15 · Finir la réponse 20 · pause 10 · Présentations 45 (3 × 10 + questions) · Fin 5.

### Two things found while building Friday

- **The 80 % / 60 % test could not be played.** The game has no demand setting, yet the carnet and the calculator said "refaites l'année à 80 %". It is now **computed**: gap at 80 % = gap − 20 % of the project's cases × margin per case. The project's fixed costs stay whole.
- **Dr Neri's project needs four counted actions in the same year.** The default limit is 3. The facilitator sets **action limit = 4** in Game setup.

## 7. Day plans

| Day | Question | Activation | Demonstration | Application (support) | Tools pinned to the map |
|---|---|---|---|---|---|
| **Lun** 9:00–11:30 | Que fait cette clinique, et pourquoi perd-elle de l'argent ? | 15' free exploration, one question | The money loop; the +20 % price case worked through the whole cycle | 2 years with the decision record (full template) | Structure des coûts → cost nodes · Capacité inutilisée → Capacité · Analyse différentielle → two versions of the map |
| **Mar** 9:00–11:30 | Que se passe-t-il quand on pousse, et combien faut-il ? | Monday's question | Synthesis of the large loop | Jigsaw maps; break-even on their clinic (each step prompted) | Marge → Cas → Recettes − CV · Seuil, marge de sécurité → Cas → Résultat |
| **Mer** home | Qu'est-ce qui limite ? | Map v2; the year just played | One drill per situation | Surgery case; own clinic, alone; first Neri draft | Contrainte, marge par heure → Capacité → Cas · Point d'indifférence → cost shape of a capacity choice |
| **Jeu** 9:00–11:30 | Que laisse la carte dehors, et vu d'où ? | The Neri draft | The practitioner | Sorting against the map; Cadrer on the draft | Coûts pertinents / irrécupérables / d'opportunité |
| **Ven** 9:00–11:30 | Que répondez-vous ? | The full dossier | — | Neri, unaided | All of the above; délai de récupération |

Monday's and Tuesday's clock tables are in §7a.

## 8. Year budget

| When | Years passed | Clinic at the end |
|---|---|---|
| Monday | 2 | start of year 3 |
| Before Wednesday | 1 | start of year 4 |
| Wednesday | 1 (constraint prediction) | start of year 5 |
| Friday | 3, tested from a saved clinic | year 8 |

The facilitator sets **target year = 8** in Game setup. The game allows up to 12.

## 9. Open questions for the owner (answered 2026-10-14, see the decisions at the top)

1. **Facilitator notes.** The jigsaw groups, the order for assigning focal variables, the synthesis
   script and the target-year setting must stay out of the carnet. `guide-animateur.html` is no
   longer in this folder. Where should they live?
2. **Number of teams.** The rotation needs a multiple of three for clean jigsaw triads. If there are
   not enough teams, what is the fallback?
3. **Tuesday is full.** It fills exactly 180 min. Should the surgery case shrink, or move to
   Wednesday?
4. **Monday's free exploration.** It is kept at 15 min, with one question. Do you want it longer,
   or removed?
5. **Grading weights.** The dossier now has five parts revised every day, not five day-sections.
   Should the weights (10 / 15 / 20 / 15 / 25 / 15) move to the dossier parts, or stay by day?

## 10. Build order

1. **This document.** Confirm §3 and answer §9. ← *we are here*
2. **Accueil, the map component, the cycle, Référence, Lundi, Mardi.** Owner review in the browser.
3. **Mercredi to Vendredi**, answer keys, facilitator notes, verifier rules:
   - arrow signs and thresholds from the model;
   - term before first use;
   - activity template present;
   - every cycle step each day;
   - Neri letter before Wednesday;
   - year budget within the target year.

   Then falsify each rule once.


## Revision of 2026-10-19: two years a day, "exploit before you expand", the map put to use

The owner replayed Monday as most groups played it (vaccination in year 1, preventive care in year 2). Measured in the model (`outils/semaine-type.js`):
- At the start of year 3 the consultation room is the constraint and 85 % of requests are served.
- The clinic makes a profit, and climate is 52 and rising.
- Allocating staff above 100 % gives 0 overtime while the room is full.
- The pay-rise case did not fit this clinic.

**Decisions:**

**Two years per day.**

| Day | Years |
|---|---|
| Monday | 1–2 |
| Tuesday | 3–4 |
| Wednesday | 5–6 |
| Thursday | none |
| Friday | 7–9, twice, from a saved clinic |

The target year is 10.

**Ladder, written in the carnet and enforced by the facilitator.** The bank refuses any expansion before Friday.

| Day | Newly allowed |
|---|---|
| Monday | Prices, services the team can already run, allocations up to 100 % |
| Tuesday | Opening hours, overtime, salaries, HR, staff meeting, communication, pace, sustainability |
| Wednesday | Training |
| Friday | Everything, for the Neri project only |

The aim is to exploit the constraint before paying to enlarge it. The Neri project is the first time the clinic can expand.

**Tuesday's case is « La salle est pleine ».** Four proposals, each touching a different loop: later hours, faster consultations, a higher price, and the municipality's low-carbon plan.

**The map is put to use: "predict with the map, check in the game".** Students write ↑/↓ before planning, then ✓/✗ after. Every ✗ is discussed, and **the perimeter is worked on Tuesday**, from those ✗. Three limits of the model come out of it:
- rushed visits cost almost no trust;
- a higher price can raise trust;
- a vet working beyond 100 % is hidden by the team average.

Thursday keeps only a 15-minute « Hors du périmètre » block.

**Break-even of a decision.** For a clinic that already makes a profit, the useful question is how many cases a decision must bring in to cover its added fixed cost. The fixed cost is read in « Ce que cette décision coûte ».

**Margin per hour of the scarce resource.** On Wednesday this is per hour of room when the room is full. The new `Temps de salle par cas` line on the service sheet makes it readable. Ranking for the canonical clinic: vaccination 133 €/h, preventive care 80 €/h, consultation 77 €/h.

The test result: raising the consultation's price or shortening it pays. Giving all of Maya's time to vaccination fails, because preventive care loses her hours.

**Generated, not typed.** `outils/semaine-type.js` produces the figures and `outils/corriges-semaine.py` writes the Tuesday and Wednesday answers. `verifier-chiffres.js` checks:
- the ladder;
- the « Permis » boxes;
- the predict/check routine;
- Friday starting at year 7;
- the facilitator's demonstration figures.


## Revision of 2026-10-19 (b): trust, rushed visits and price that students can see and act on

**The problem, measured.**
- Trust barely mattered: trust 40 against 60 made about 400 € a year of difference, with no threshold.
- Rushed visits cost almost nothing, because their trust loss was cancelled out by serving more.
- Price ignored the type of client as far as students could see, and a higher price even *raised* trust.

**What was added.** Every parameter is in `data.js`: `servicePaces.fast` and `trustModel`.

- **Rushed visits**
  - 10 % come back as unpaid return visits. They use room and staff time and supplies, and they add carbon.
  - Trust −6 per year, weighted by the share of cases rushed.
  - Climate −1 per year for each rushed service.
- **Trust**
  - It moves the price clients accept: ±0.4 % per point away from 50.
  - It has thresholds on clients:

    | Trust | Effect on clients per year |
    |---|---|
    | below 45 | −3 % |
    | below 35 | −8 % |
    | above 65 | +3 % |
- **An unfair price**
  - A price above the accepted price costs trust each year, weighted by the type of client's price sensitivity (×20, capped at −6 per year).
  - The type of client becomes a Tuesday lever (« Marché cible »).

**Visible on screen**
- `Impact du plan` has two new rows: `Confiance des clients` and `Climat de l’équipe`.
- The price screen shows the type of client, each service's `Prix accepté par vos clients`, and a warning when the price is above it.
- The trust card says what moved trust and where the threshold is.
- The service sheet shows `Retours de visites pressées`.
- The year's results have two new lines: `Prix jugés trop élevés` and `Rythme pressé`.

**Safety protocol**
- `outils/instantane-modele.js` records 15 paths.
- With every new parameter at 0, the snapshot comes back **identical**: the code adds nothing by itself.
- Switched on one at a time, each mechanism only moves the paths that use it.
- Balanced year 1, the `CHIFFRES` block (Monday) and Friday's correction are unchanged.
- **Known, accepted consequence:** the rescue scenario starts with price-sensitive families and prices above what they accept. Left alone, its trust spirals down (43 → 7 over six years) and clients leave. The owner chose to keep this. Rescue's starting trust was raised to 46. The course uses balanced.

**What the Tuesday case looks like now**, on the canonical clinic:
- **Fast consultation:** +7 500 € instead of +14 400 €. About 200 unpaid returns, trust 55 → 53 → 51, climate −1 per year.
- **58 € consultation:** trust −1.2 per year with the local mix. Much worse with price-sensitive families (−5 to −6 per year). No penalty with advanced-care owners.

The real limits left for the boundary work: individual overload hidden by the team average, animal welfare, and what a refused client tells others.


## Revision of 2026-10-19 (c): no number without a role

**Audit.** Measured on the course clinic:
- **Soutien des référents** changed nothing until an advanced service existed (the result was identical to the euro at 30, 50 or 70), and slid down on its own.
- **Pression d’accès** never passed 50, so it never acted. Its sense was odd: refusing clients created *more* requests.
- **Réputation** and **clients** drove demand but appeared nowhere on screen.
- **Carbon** had no consequence back in the clinic.
- **The goals** are information only.

**Decisions (owner)**
- Give référents and pression a real role.
- Show clients, and fold reputation into trust.
- Add a carbon feedback.

**What changed** (`data.js` `socialModel`; the same protocol as before: zero-parameter snapshot identical, then one mechanism at a time)

| Indicator | Before | Now |
|---|---|---|
| Référents | +0.3 % advanced requests per point | +1 % per point; moves the ultrasound's demand on Friday |
| Pression d’accès | added requests above 50 | each year moves halfway toward 40 + 1.5 × the % of requests refused, and costs 0.1 trust per point above 50; no longer adds requests |
| Réputation | grew clients | no longer grows clients; trust carries it (growth weight 1/300). Removed from the PDF; kept, inert, in the JSON |
| Carbon per case | no effect | lower than last year raises trust, higher lowers it, ±2 a year at most |

On the course clinic, the full room's refusals now catch up: pressure goes from 46 to 80 by year 7, trust falls from 59 toward 52, and clients slow down.

**Visible**
- A `Clients` card on the overview, with next year's count and the reason.
- The relations panel (« Agir sur le climat et la confiance ») says, for each indicator, what moves it and what it changes.
- The trust card names the refusals and the footprint per case.

**Exports**
- **JSON:** `acceptedPrice` per service, and `clientMovement`.
- **PDF:** a « Relations autour de la clinique » table each year (start → end and why it moved), plus accepted-price and return-visit columns.

**Found on the way**
- A new service treats no cases until it is given hours. Friday's carnet step now says so, and the facilitator notes ask the facilitator to check it.
- My snapshot tool had run Dr Neri's project with the default limit of 3 actions, so the ultrasound was never opened. It now runs with 4, and it fails loudly if the ultrasound serves nothing.

## Revision of 2026-10-19 (d): goals become promises, and the game must not settle

Owner's requests:
- make the goals matter;
- explain why there are 1 200 clients but 1 906 cases served;
- replace the long texts about climate and trust with something that can be read at a glance;
- make choices affect other areas, return with a delay, and force trade-offs that students discover by playing.

**Model.** Each goal is now a promise to someone who reacts the following year. The parameters are in `commitmentModel` in data.js; the figures below come from the model.

| Who | Goals | Kept | Missed |
|---|---|---|---|
| The bank | net, cash, margin | loans at 6 % | one year: 9 %; two years in a row: a new loan is refused |
| The clients | served | — | already acts through access pressure, then trust; no new mechanism, to avoid counting it twice |
| The team | staff, climate | — | already acts through workload, then climate |
| Referring vets | services, advanced | referral support +2 | −1 |
| The municipality | carbon | a €2 000 grant the next year, only if the clinic invests in a sustainability measure | no grant |

**Screen.**
- One strip, Foyers clients → Demandes → Cas traités, with « ≈ x par foyer et par an » and the share served.
- Four gauges: trust, climate, access pressure and referral support. Each shows its thresholds, the planned value, the past years and at most three cause chips; each chip opens the screen where one acts on that cause. The explanation sits behind an « i ».
- The Engagements panel shows a ✓ ✗ track per stakeholder and the consequence « l’an prochain ».
- The plan panel adds trust and climate « dans 2 ans ».
- JSON and PDF carry the promises.

**Measured** (`node outils/boucles.js`: the course clinic over 8 years, under seven simple policies):
- No policy keeps every promise every year from year 3 on.
- Serving everyone keeps the clients until year 4. The climate then falls under 50 in year 6 and 45 in year 7, and the clients promise breaks again: an oscillation.
- Consultations raccourcies earn more for three years. Trust then falls from 57 to 41 and households fall from year 7: a delayed cost.
- Going green earns the grant from year 4, but refusals pile up: pressure reaches 87 and trust falls back.
- **Finding:** after year 3, the bank and referring-vet promises are never at stake in the course clinic, whatever the policy. The bank's loan rate will matter only for a team that lost money two years running. This is reported to the owner rather than tuned away.

**Checks.**
- Headless tests cover:
  - the loan rate at 9 % and the loan refused;
  - referral support +2;
  - the grant only with investment;
  - the flow strip, the gauges and the hidden explanations;
  - the pressure chip opening the rooms;
  - the two-year rows;
  - the commitments in JSON and PDF;
  - `boucles.js` passing.
- Each test was falsified once.
- verifier-chiffres rule 19 holds the carnet's Engagements table and trust thresholds to the model.

**Carnet.**
- The Référence's « où le trouver » column points to the strip and the gauges.
- The goals block became « Les engagements de la clinique ».
- New glossary rows: Foyers clients, Jauge, Engagement.
- The journal has a column « Quelle promesse a bougé, et quand ».
- Friday asks which promise the Neri project puts at risk, and in which year, and has students read the loan rate in Gestion → Financement.

## Revision of 2026-10-19 (e): mechanics, not display

**Owner:** the gauges, warning lines, sparklines, cause chips, « i » panels and « dans 2 ans » rows added things to decode without helping anyone understand. The job is for the mechanics to work: social and client effects with real repercussions, the results showing the signals, and students re-diagnosing each year from the last. **All of that display is removed.** The overview keeps:
- plain cards (net result, workload, carbon, climate, trust);
- the one-line strip households → requests → cases;
- a plain promises list.

**Measured before the change.** Shocks were applied at the start of year 3 of the canonical clinic (consultation room full, 83 % served):

| Shock | Effect |
|---|---|
| trust −15 | −470 € |
| climate −15 | **+822 € and +27 cases**: absences shifted room time to vaccination |
| pressure +25 | 0 the same year |
| households −10 % | −1 058 € |

Households kept growing until about 70 % of requests were served. The full room absorbed every client-side and team-side signal.

**Two mechanisms** (`socialModel`, under the snapshot protocol: neutral = identical, then each switched on):
- `refusedLeave: .06`: six households in a hundred refused requests go elsewhere for good. A clinic that does nothing now levels off at the promised share served (about 82 %) instead of growing while refusing.
- `slowBelow: 50, slowPerPoint: .004`: below 50, each climate point lost adds 0.4 % to every case's staff and room time. Climate −15 now costs about 5 700 € and 160 cases, even with the room full.

The Monday figures are unchanged.

**Results page.** « Signaux de l’année » sits under the year's figures: one plain line per signal (cause → effect next year), each with an « Agir › » link to the screen where it is acted on:
- refusals → households lost;
- climate → time per case, or a resignation;
- overtime → absences;
- return visits;
- a price above what clients accept;
- trust → prices and households;
- pressure → trust;
- each missed promise → its consequence.

The same lines are in the PDF and the JSON (`signals` per year). A test checks that screen, PDF and JSON match.

**Tests:**
- refused requests cost households;
- no year below 80 % served grows households;
- a tired team serves fewer cases with the room full;
- no worse state improves the year;
- the signal lines and their links;
- no gauges, chips or two-year rows on the overview.

Each test was falsified once. verifier-chiffres now checks the carnet's two new repères (« Familles refusées », « Équipe fatiguée ») and the notes' demonstration sentence against the model.

**What the loops now show** (`boucles.js`):
- The clinic balances on its capacity.
- Rushed consultations earn every year while trust slides.
- The Neri project takes vet hours from the consultation, so refusals rise and the clinic loses households in the years after: the clients promise is what it puts at risk.
- The bank, team and referring-vet promises are rarely at stake in the course clinic after year 3.

## Revision of 2026-10-19 (f): the team screen points, it does not explain

**Owner:** the game is not built for the carnet. The screen should point things out through visual structure, not write the conclusion.

**The case that started it.** Maya was assigned 117 % of her hours, yet the screen showed 0 € of overtime. Her card said « 17 % d’heures supplémentaires »; the drawer said 0 h. The model was right: only worked hours are paid, and the full consultation room stopped about 360 of her assigned hours from being worked. The screen hid this.

**Changes (app.js, styles.css; the model is unchanged):**
- **One hours bar** per person, on the card and in the drawer:
  - worked hours;
  - overtime;
  - hours lost, each with its cause (room full, service closed, missing skill, no demand), and the cause links to its screen;
  - unassigned hours;
  - a mark at the hours available.
- **The bar replaces** the four-cell grid, the assignment meter and the « Heures utilisées » line.
- **Constraint badge** at the top of the team screen.
- **Cause tags** on the team warnings and the service rows (« Salle de consultation pleine »).
- **The draft's effect beside the control:** « Cas traités −19 · Résultat net −339 € ».
- **Removed:**
  - the false overtime claim on the card;
  - the red tone when no overtime is worked;
  - the « surplus » sentences;
  - the « manque » sentence when a full facility is the limit.
- **Collapsed:** the « cas portés » paragraph.
- **New results signal:** « N h affectées à X, non travaillées → cause ».

**Tests:**
- the bar adds up to the larger of available and assigned hours;
- worked hours never exceed available hours;
- the headline never announces overtime the bar doesn't show;
- an assignment above 100 % behind a full room is not called overtime;
- hours behind closed services or a missing skill show as lost.

**Found, not changed:** assigning Maya more hours behind the full room *lowers* cases (−19) and the result (−339 €). The room is shared in proportion to staff pools, so room time moves to preventive care, which takes longer per case. This is a question for the owner: should staff hours decide which service gets the room?

## Revision of 2026-10-19 (g): one refusal count, screens that point

**Refusals.** Each service now records `lostBy`: requests lost to staff hours, then to a full room or equipment item, then to stock-outs. These add up to demand − honoured, and a test checks the sum on four paths. The model's figures are unchanged (snapshot identical).

The overview strip shows the total with a striped split by cause. On the course clinic in year 5: 727 = salle 415 + heures vétérinaires 158 + ruptures 154. The stock-outs explain why the room reads 97 % while « saturée ».

The same split appears in four places:
- the care page's service rows (cause tags with counts);
- the care page's room panel (« N demandes refusées ici »);
- « Points d'attention »;
- the results page.

A test checks the figures agree across screens.

**Pointing, not prescribing.**
- « Points d'attention » states the fact and links to the screen. Removed: « Ajoutez de la capacité, étendez les horaires… », « Ajouter une salle », « Affecter X », « Déplacez des heures… ».
- The constraint badge is now on the care page too.

**Results page.**
- The six cards show their change over the year instead of « Amélioration ou objectif atteint ».
- The subtitle no longer asks students to « consigner les apprentissages ».
- The causes lose their descriptive sentences, and the service lines lose their repeated constraint.

**Durabilité.**
- The per-case footprint is signed against its target (« −42 % par rapport au départ · objectif −15 % »).
- The card « Promesse à la commune » marks each condition: per case, volume kept, a sustainability measure. Its ✓/✗ is the one the overview's promises show.
- The target now comes from the goal itself rather than a second hard-coded table.
- The commune consequence is shortened to « pas de prime ».

## Revision of 2026-10-19 (h): fewer cards, one word per idea

**The owner's decision.** When a room is full, staff hours decide which services get its time. Giving a person more hours on a service behind a full room can therefore lower the year. This stays as a lesson to discover.

**Care page.**
- The « Salles 1 » and « Équipement clinique 0 » cards are removed, along with the two-button « Salles / Équipement » block.
- « Gérer les salles › » and « Gérer l’équipement › » now sit in the room-use panel's heading, and that panel moves above the service list (where the controls must be, by an existing test).

**Vocabulary:**
- **Charge** means hours worked ÷ hours available, everywhere. The percentage on each person's card is labelled « charge ».
- The staff goal now reads « Garder la charge de l’équipe entre 45 % et 94 % » instead of « l’utilisation du personnel ».
- **Hours:** « disponibles », « travaillées » and « non travaillées ».
  - The team card is renamed « Heures payées non travaillées ».
  - The PDF and hours-by-service columns say « Travaillées » and « Non travaillées ».
- **A full room or machine** reads « {nom} pleine » / « {nom} saturé » on every screen: plan panel, badge, tags and signals. The label is changed at its source in i18n.js.

**Phone plan bar:** « Trésorerie finale 286 786 € (0 €) » instead of « 0 € », the difference shown alone.

**Tests:**
- the phone bar shows the treasury itself;
- the « charge » label is present;
- « staff use » appears nowhere on screen;
- the care page has no room or equipment count cards.

## Revision of 2026-10-19 (i): the drawers, and a fix that wore out nothing

**Bug.** Choosing the neighbourhood the clinic is already in was a real move: 20 000 € and 5 % of demand, and it removed the parking. It is now a no-op in the model.

The choice in force is shown as « Actuel », without a preview or a button, in four drawers: Implantation, Marché cible, Stock and RH.

**Diminishing returns** (`socialModel.repeatDecay: .5`, under the snapshot protocol: neutral is identical, and switched on the course paths are unchanged too). When the same trust or climate action is taken in consecutive years, its effect is halved each year (+8, +4, +2) and comes back in full after a year off. The preview beside the button shows the reduced effect.

**Option cards:**
- The repeated sentence « Pas encore d’effet sur les cas : … » is gone.
- What a purchase still needs is shown as ✗ tags per service (« Chirurgie courante ✗ Poste d’anesthésie ✗ service ouvert »).
- The room count is a badge (« 1 en service », « aucune ») instead of running into the price.
- « Explorer les services » uses « Salle de consultation pleine » instead of « Saturé ».

**Tests** (each falsified once):
- one current card per drawer, with no button;
- the same neighbourhood costs nothing;
- the decay goes ×1, ×.5, ×.25 and back to full after a year off;
- the room previews use tags, not sentences.

## Revision of 2026-10-19 (j): Gestion as a structure, comparisons as tables

**Gestion.** One bar from the model shows where the year's money goes, on one ruler:
- variable costs (with « ≈ x € par cas traité »);
- fixed costs (with the overtime they include);
- tax;
- the net result, or the loss running past the « Recettes » mark.

The legend gives « Marge sur coûts variables » and « Coûts totaux ». This replaces the Recettes, Coûts totaux and Coûts variables cards; Résultat net and Trésorerie keep theirs. A test checks that the bar adds up to the revenue, for both a profit and a loss.

The fixed costs are now shown rather than left to calculate. The carnet's Monday « où lire » and the glossary point to the bar, and keep « Coûts totaux − Coûts variables » as a check.

**Comparisons.**
- **Équipement:** each item compares Acheter / Louer on one table (one-off cost, recurring cost, net result, treasury, cases), with each condition still missing shown once as tags.
- **Financement:** the three loan cards are now one table with three columns (30 000, 50 000, 100 000 €).
- **Prix des services:** a scale marks the clinic's price against the price clients accept. The zone above the accepted price is shaded, and the « au-dessus : … » sentence is gone.
- **Collapsed or shortened prose:** the threshold rules in Stratégie RH, the « Qui peut faire quoi » explanation, the price-sensitivity note, and the drop-off description (now a list of facts, without « Utile quand une salle est saturée »).

**Marketing, diagnosed (not yet changed).** Measured on the course clinic with the three « Stratégies de marché » (net in the first year; 3-year total in brackets):

| | Year 1, room free | Year 3, room full |
|---|---|---|
| none | −64 969 (−184 963) | 35 075 (105 665) |
| communication, regular follow-up / targeted | −66 256 / −68 624 | 33 094 / 29 770 |
| competitor monitoring, internal / external | −64 175 / −69 339 | 35 403 / 30 811 |
| local market study, internal / external | −62 587 / −68 206 | 35 612 / 29 864 |
| social action « Améliorer la communication » | −64 348 | 34 685 (107 700) |

Findings:
- Paid marketing never pays in the course clinic, whether the room is free or full.
- The free « internal » options gain a few hundred euros, because they use idle support hours.
- Once the room is full, every demand-raising option adds refusals (821 → 1 096), and so lost households.
- Competitor monitoring acts on a « concurrence » that no screen shows. Monitoring and the local market study are both just « +x % demand » under different names.
- « Communication » exists twice. The marketing version is yearly, with demand and accepted price. The social action is one-off, at 800 €, and gives more trust.
- The owner's decision is pending.

## Revision of 2026-10-19 (k): marketing that teaches, and a money bar that reads

**The owner's decisions:** merge communication; remove competitor monitoring; give the market study an information role; show what raising demand costs.

**Model** (under the snapshot protocol: course paths identical):
- **Communication exists once**, as a ladder (de base / suivi régulier / ciblée) in « Communication et étude de marché ». The one-off social action « Améliorer la communication » is removed. The ladder's trust gain wears in like any repeated fix (+5, +2.5, +1.25 for each year kept at the same level); its demand and accepted-price effects stay.
- **Veille concurrentielle is removed.** It acted on a competition factor that no screen showed. The `relief` term is gone, and `competition` is the location's own.
- **The local market study buys information, not demand.** Its `precision`:
  - without a study, the accepted price is known only as a range of about ±20 %;
  - a study by the team (60 support hours) narrows it to ±8 %;
  - a consultancy (8 000 €/year) gives the exact figure.

  The range is never centred on the true value. The model itself always uses the true value; only what is shown changes. The price screen, the signals, the PDF and the JSON (`acceptedPriceShown`) all show the range the clinic knew that year.

**Screens:**
- **Option previews:** every decision's preview now shows « Demandes refusées » and « Foyers l’an prochain » when they move. Marketing a full clinic visibly adds refusals: suivi régulier takes them from 708 to 813 on the owner's clinic in year 5.
- **Prix des services:** the price scale draws the uncertainty band.
- **The relations drawer** links to the communication ladder.

**Gestion bar, rebuilt** after the owner could not read the first version (grey and orange with a lone « Recettes » line):
- two bars on one scale: « Recettes » on top, « Où elle va » underneath (coûts variables, coûts fixes, impôt, résultat net), each labelled on the bar;
- a bracket marking the « Marge sur coûts variables »;
- a loss drawn as the cost bar running past the revenue bar.

**Tests:**
- no veille, and no second communication;
- the study adds no demand;
- the ladder wears in;
- the refusals show in the preview;
- the range contains the true value without being centred on it;
- the same range appears on screen, in the PDF and in the JSON;
- the bar adds up, with its structure and the loss case.

verifier-chiffres now holds the carnet's « Étude du marché local » repère (±20 %, ±8 %, exact) to the model.

## Revision of 2026-10-19 (l): the constraint is diagnosed, previews show only change, the overview tells the truth

**Constraint.** It is the students' to diagnose, so no screen names it before the year is passed:
- the badges are gone from Équipe and Soins;
- the plan panel's « Contrainte principale » row is gone;
- it appears in Résultats (Origine du résultat) once the year is played.

Before the year, the forecast still shows the refusals by cause (overview bar, Points d’attention, service tags): facts, not a verdict.

Finding: at the start of year 3 on the course path, the constraint of the year just passed is stock-outs (134 refusals). The room fills only during year 3 (forecast: room 419, support hours 164, stock-outs 148, vet hours 90). Tuesday's « la salle est pleine » now comes from the overview's refusal split.

The carnet, the notes and the Tuesday answer key were reworded accordingly: « ce qui refuse le plus de demandes » before the year, « Résultats → Contrainte principale » after it.

**Previews.** Each decision shows only what it changes, signed (« Ce que ce choix change »):
- cost lines, with the second year when it differs;
- cases, refusals (with the cause that grew, e.g. vaccination's « Ruptures de stock »), net result, treasury, households next year, workload, carbon, climate, trust, referral support, access pressure — each only if it moves.

The before → after list is gone, because the plan panel holds the full picture. The Équipement and Financement comparison tables stay.

The owner's question, why opening vaccination adds refusals: on the starting clinic they are stock-outs (52 of 864), from the default « Basique » stock strategy, not capacity. They now carry that cause in the preview.

**Overview:**
- « Les clients ✓ — les refus retombent » was false between about 82 % and 93 % served. It now states the access pressure the year leaves and the trust it costs.
- Carbon is shown per case against its target, not as a total.
- This year comes first. Under « L’an prochain »: households (now → next, and how many leave after a refusal) and the promises, in their figures (« ≥ 82 % des demandes servies », « charge 45 %–94 % »…).
- « + N non proposées » is replaced by the requests of services the clinic could open now.
- « Heures de soutien » is used everywhere.
- The filler carbon signal and the instruction subtitles are gone.

The page went from about 330 words to 260.

## Revision of 2026-10-19 (m): measurements before the year, causes after; cards show only their direct effect

**The owner's diagnosis, confirmed.**
- The refusal-split bar on the overview still named the constraint: its largest segment is what Résultats calls « Contrainte principale ». It filled the page width whatever the count, and had no title.
- The same attribution was given before the year in five other places: Points d’attention, the care service tags and room panel, the team hours bar and warnings, the Explorer chip, and the previews.

**The rule** (owner, 2026-10-19):
- Before the year, the screens give the count and the measurements: room hours used against capacity, hours worked, requests and refusals.
- After the year, Résultats gives the attribution: « Contrainte principale », and the refusals split by cause, now under « Origine du résultat ».
- **Exception: stock-outs** are always named (« 708 refusées · dont 154 ruptures de stock », « 94 ruptures de stock » on a service, « Ruptures de stock » in a preview). They belong to the stock strategy, not to a constraint, and naming them keeps a first opening understandable.

**What changed on screen:**
- **Points d’attention:** the busiest room or machine as a measurement (« Salle de consultation 2 180 / 2 256 h · 97 % »), and the service refusing the most (« Soins préventifs 948 / 1 286 traités · 338 refusées »).
- **Care page:** rooms are coloured by measured use (above 95 %); « Pleine » and « refusées ici » are gone.
- **Team screen:** unworked hours show as « non travaillées ». A closed service and a missing skill are still named, because they are the person's own set-up.
- **The carnet, the notes and the Tuesday key** ask students to find what is closest to its capacity, and to check it in Résultats.

**Option cards show only what the choice changes directly:**
- its costs, line by line;
- what it does to activity: requests, cases, refusals, households next year;
- an indicator only when the choice acts on it directly (`directIndicators`: measures and location → carbon; meeting, pay, HR, hours → climate; communication and price → trust; pace → both).

Net result, treasury and workload are no longer repeated on every card; they are in « Impact du plan ». A market-focus card went from ten figures to five.

**Durabilité:** the « Promesse à la commune ✗ » card is now a checklist with a title that states it (« … : non tenue »):
- carbon per case, against its target;
- volume kept, against the minimum (80 % of the start);
- a sustainability measure, linking to the sources below;
- then what follows next year.

The separate per-case card is gone from this page.

## Revision of 2026-10-19 (n): hours by their real cause, warnings that can be acted on, the vet's support work

The owner's three questions, answered from the model on year 1 (vaccination and preventive opened).

**1. « Ruptures de stock 770 h » on Maya's bar was wrong.** She was assigned 885 h on vaccination, which needed 294 h, and 476 h on preventive, which needed 304 h: about 760 h beyond what the requests needed. Stock-outs cost 30 cases, about 10 h. The bar took each service's main limit as the reason for every idle hour.

`hourSplit` now:
- gives an assignment's idle hours first to the requests its service lost to something other than this role's own hours (room, equipment, the other role, stock-outs), at this person's share of the service;
- counts what is left as « pas assez de demande ».

Maya's bar now reads « pas assez de demande 758 · ruptures de stock 12 ». Before the year, the causes named are closed service, missing skill, stock-outs and lack of demand; the rest reads « non travaillées ». After the year, the results signals use the full split.

**2. Adding the « missing » hours reduced cases.** Two reasons:
- The old « manque » compared the hours needed for every request with the hours assigned, for one role alone, ignoring that the service could be held back by the other role, the room or its demand.
- The hours a student adds are taken from another service.

Measured: moving Amina from 80/20 to 60/40 (consultation/preventive) took cases from 3 402 to 3 046 and the net from 5 858 € to −7 227 €. On the owner's year-5 clinic, giving Maya the « missing » 94 support hours on preventive care: +25 preventive, −26 consultation, −18 vaccination, −19 cases and −339 € in all. The room is full, so extra staff hours only win room time.

`shortageHours` is now:
- the requests the service lost because this role ran out, × this role's time per case;
- zero when the service is also held back by a full room or machine.

A test gives each announced shortage its hours and checks that cases do not fall.

**3. The vet/support split was invisible.** Each service has a fixed time per case and role (consultation 0.55 h vet; vaccination 0.34 h support; preventive 0.25 h vet + 0.47 h support), and a vet can do the support part (vet hours, at vet cost; not the reverse). Now:
- the service sheet shows one case as a bar split by role, with « un vétérinaire peut faire tout le cas : 0,72 h »;
- a vet's hours bar shows « soutien couvert » for support tasks the vet did, from `vetCoverHours`.

Model figures unchanged (snapshot identical); these are outputs only.

## Revision of 2026-10-19 (o): cases, and refusals only when demand moves

Requests = cases served + requests refused, so a card showing all three repeats one of them.

The rule (owner, 2026-10-19):
- « Cas traités » is always shown when it moves.
- « Demandes refusées » is shown only when demand itself moves. Otherwise it is just the mirror of the cases. Stock-outs keep their cause next to it.
- « Demandes » (the sum of the other two) is no longer shown.

Examples:
- opening vaccination: cases +812, refused +52 (stock-outs);
- a consultation room: cases +422;
- targeted communication on a full clinic: cases +25, refused +257.

Noted, not changed: « Étude par l’équipe » shows cases +10 on the full-room clinic. Its 60 reserved support hours shrink preventive care's share of the shared room, and the other services' shorter cases fill it. This is the room-sharing rule the owner kept.
