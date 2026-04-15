# Coach Day Workshop — Project Context

## What this is

A workshop plan for Visma Tech Lithuania's "Coach Day" — a session for ~25 engineering managers (called "coaches") to work through the real challenges of AI adoption in their teams. The theme is **"AI: Expectations vs. Reality"**.

Tomek (Engineering Department Manager & Software Architect at Visma Tech Lithuania) is organizing this. He runs the engineering department and is also a university lecturer.

## Source data

`survey-responses.csv` contains 9 responses from coaches to a Google Form with 4 open-ended questions (in Lithuanian):

1. **Naujas darbo pobūdis** — How AI is changing team work processes and what new challenges it brings (AI agents, autonomy, team dynamics)
2. **Trintis su išore** — Friction with external stakeholders (partners, non-LT managers) — unrealistic expectations, pressure, bypassed practices
3. **Žmogiškasis faktorius** — The human factor — fears of replacement, loss of meaning, coping with change
4. **Coach rolės pokytis** — How the coach role itself is changing — new challenges coaches didn't face before

### Key themes from the analysis

**Code review crisis (7/9 respondents):** AI generates huge PRs (100+ files), review takes hours, quality is uncertain, devs resent that coding fun went to AI while they became "proofreaders."

**Bottleneck migration (5/9):** Coding got fast but requirements gathering, testing, and release didn't. Teams finish faster but don't ship more. QA is drowning.

**Existential motivation crisis (5/9):** Developers losing meaning — "what's the point of me?", backlogs emptying, some considering leaving. Range from total AI refusal to thriving.

**Pushback against AI pressure (5/9):** People feel forced, unclear WHY Visma Tech is pushing AI so hard. "Is it to be first? Because CTO said so? To avoid layoffs?" Silence breeds worst-case assumptions.

**"AI programmers" conflict (4/9):** POs, analysts, managers using AI to make technical decisions, bypassing architecture and security. Creates power struggle with actual developers.

**Cognitive overload (3/9):** Even managing one AI agent stretches capacity. Multiple agents overwhelm. Human brains can't keep up with AI output speed.

**Unclear communication from leadership (2/9 explicitly, but underlies many responses):** Ambitious targets without concrete steps. Inspirational demos that don't translate into actionable plans.

### Core tensions (used in Phase 2 framing)

1. "AI makes us faster" vs "the bottleneck moved, not disappeared"
2. "Everyone should use AI" vs "nobody explained why, and pressure feels coercive"
3. "AI democratizes building" vs "non-devs making technical decisions is dangerous"
4. "Developers adapt" vs "the meaning and joy of work is disappearing"

## Workshop design

Full plan is in `workshop-plan.md`. Here's the rationale behind key decisions:

### Design decisions made

1. **Cases instead of topics.** Original design had 5 abstract topics groups could choose from. Problem: people avoid hard topics, topics bleed into each other, and abstract framing leads to vague discussion. Cases force concrete thinking — you can't be vague about a situation with a person in it. Each case carries multiple themes.

2. **Pre-assigned groups, no choosing.** Prevents comfort-zone clustering and ensures hard cases (especially Case D — the political one) don't get avoided. Mix tenures, teams, temperaments.

3. **Everyone's voice first (sticky notes).** Only 9/25 responded to the survey. Without Phase 1, 16 people are spectators in a workshop framed by someone else's answers. Green + red sticky notes make the data collective and also surface what's working (not just problems).

4. **Synthesized tensions, not quotes.** Original design used direct quotes from survey responses. Problems: writing styles are recognizable (25 coaches, 9 responses — easy to guess who), and it frames the workshop as "these 9 people's problems" instead of "our shared reality." Phase 2 presents patterns, not attributable words.

5. **"Write the actual words" forcing function.** Task 2 asks coaches to draft the literal conversation they'd have with the person in the case. Not bullet points, not "we should communicate better" — actual sentences. This is where real skill gaps surface and real learning happens.

6. **Stop/Start/Escalate instead of generic "actions".** "Escalate" with a name and date prevents the common workshop failure of "leadership should do X" with no follow-through.

7. **Simple presentations at the end.** Earlier version had gallery walk + dot voting + scripted commitment speech — overengineered. One representative per group presents, open discussion after each, facilitator closes with honest reaction.

### The 5 cases (composites from survey data, no attribution)

- **Case A — The senior who became a proofreader** (themes: review overload, motivation loss, team asymmetry)
- **Case B — The PO who became a developer** (themes: role boundary conflict, architecture bypass, power dynamics)
- **Case C — The team that ran out of work** (themes: bottleneck shift, existential fear, self-sabotage)
- **Case D — The silent room** (themes: missing "why", leadership communication, coach's own uncertainty)
- **Case E — The bug that slipped through** (themes: quality vs speed, false confidence, trust erosion)

### Group task structure (3 tasks, 50 min total)

1. **Peel back the layers** (15 min) — Surface problem → Underlying drivers → Core fear/need. Forcing function: if "core" column has process problems, they haven't gone deep enough.
2. **The conversation you'd actually have** (15 min) — Write actual words, plus what NOT to say. Forcing function: if the answer works for any case, it's too generic.
3. **Stop / Start / Escalate** (15 min) — Structural changes. Forcing function: "Escalate" needs a specific name and date.

## What's left to do

Possible next steps (Tomek hasn't decided yet):

- [ ] Printable case cards (one case per A4 page, for groups)
- [ ] Printable worksheets (A3, three task sections, space to write)
- [ ] Slides for Phase 2 (the 4 tensions framing)
- [ ] Facilitator's guide / run-of-show with timing cues
- [ ] Pre-assign groups (needs the actual list of 25 participants)
- [ ] Decide case-to-group assignment (Case D = most trusted group)
- [ ] Translate any materials to Lithuanian if needed (survey data is in LT, cases are in EN)

## File structure

```
coach-day-workshop/
├── CLAUDE.md                  ← this file (project context)
├── survey-responses.csv       ← raw survey data (9 responses, Lithuanian)
└── workshop-plan.md           ← full workshop plan with all phases, cases, tasks
```
