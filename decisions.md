# Decision log

Decisions about how PersonAI works, in the order they were made. [`CLAUDE.md`](CLAUDE.md) holds the current rules; this file records when and why they changed, and what is still open.

Each entry has a status:
- **Decided**: in effect.
- **Agreed in principle**: the direction is set, but details are open and nothing has changed yet.
- **Superseded**: replaced by a later entry.

Add an entry whenever a decision is made, including partial ones. Don't rewrite old entries: if a decision changes, add a new entry and mark the old one superseded.

---

## 2026-10-06: First decisions (repo setup)
**Status:** decided. Wording updated by the scope change below. Recorded in `CLAUDE.md`, decisions 1–6. Reasons were mostly not recorded at the time.

- **Personas are reusable; scope is per project**, so the same person can be "building for" in one product and "not yet" in another.
- **Three scope groups**: building for now, not building for yet, deliberately not for.
- **The format follows the team's existing PLH persona slides** (Vimbai Moyo is the reference), plus four added sections: their story, context & constraints, where we'd lose them, and test questions.
- **Each persona's role relative to the product is explicit.**
- **Source material is kept separate from invention**: anything not from a source is marked `[draft]` or `[to confirm]`.
- **Each project picks a few coverage dimensions** to spot gaps in the set.
- **Default: a shared persona library, reuse first.** Not settled; still an open question in `CLAUDE.md`.

## 2026-10-06: PLH material cleared for public
**Status:** decided (Michele).

The 2020 PLH Digital persona decks and user stories in `sources/`, and personas derived from them, can be public. Committed in `fb75299`.

## 2026-10-06: Personas come after the product (scope change)
**Status:** decided. `CLAUDE.md` decision 7.

**Decision:** Personas are made once the product is defined, and are mainly a communication tool: a set shows the range of situations the product serves. Testing a spec or build against them stays, as a secondary use. Before this, personas were meant to shape the spec.

**What changed:**
- Each "building for now" persona stands for a distinct situation, given in one line in the project map.
- The project map should make sense to someone outside the team who reads nothing else.
- The minimum input is a description of the product. If it's unclear what the product is or does, Claude asks.
- `projects/plh-team.md` moved to `projects/_archive/`, because how PLH Digital is built and run isn't a product.

**Why:** not recorded.

## 2026-10-06: Personas built on layers of evidence
**Status:** agreed in principle. Templates and workflow not changed yet.

**Decision:** Make personas representative of reality by building them on layers:
1. **Research**: findings about real people (interviews, field notes, programme data, published figures). One short note per finding, with its source, date and the population it covers.
2. **Categories**: the situation types a set has to cover, built from the coverage dimensions. Each links to evidence that it exists and, if known, how common it is.
3. **Personas**: each stands for a category and states how grounded it is (e.g. researched / team workshop / invented). The story can be invented; the traits that define the category should be backed by evidence.
4. **Project map**: picks categories for each scope group, then a persona for each.
5. **Validation**: who checked a persona with real people, when, and what changed.

**Why:** Each persona mixes sourced, invented and assumed details, marked sentence by sentence, so nothing shows how grounded a persona or a set is overall. With 5–10 personas a set can't be statistically representative, but it can trace the traits that matter to evidence and cover the situations that matter. Partners and funders will ask whether the personas are real.

**Consequence:** the pipeline needs more input than a product description: existing research, confirmation of the categories, and checks with real people.

**Still open:**
- How was the 2020 PLH Digital deck made: field research with families, or a team workshop? This decides how much of the current library counts as researched.
- What research exists or is planned, and where raw research can live given the repo is public. Proposal: raw material stays private; only anonymised findings are committed.
- Are categories shared across products (per population, like the persona library), or defined per project?
- How much of the new input is required before a set can be made. Proposal: only the product description; the rest is optional but sets the grounding level, and the report says what's missing.

## 2026-10-06: Keep a decision log
**Status:** decided (Michele).

**Decision:** Log every decision in this file when it's made: the date, the decision, why, its status and what's still open. When a decision changes how Claude works, update `CLAUDE.md` too.

**Why:** `CLAUDE.md` shows only the current rules, not when or why they changed.

## 2026-10-06: Repo moved to the IDEMS International organization
**Status:** decided (Michele).

**Decision:** Transfer the repo from Michele's GitHub account to `IDEMSInternational/PersonAI`, so anyone at IDEMS can find it and contribute. It stays public. Old `MichelePancera/PersonAI` links redirect.

**Why:** Michele wants everyone at IDEMS to have access.

**Still open:**
- Who can push. After the transfer Michele has push rights but not admin, so an IDEMS org owner has to give IDEMS members write access (base permission or a team) and, if wanted, make Michele an admin of the repo.
