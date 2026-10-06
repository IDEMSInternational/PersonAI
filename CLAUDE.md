# PersonAI: instructions for Claude

## Purpose

PersonAI builds personas **once we know what the product will be**. Personas are a **communication tool**: a set shows the different situations a product serves. Each persona is a person in one of those situations, with a personal, emotional story. A set is used to:

1. **Show the range of situations we serve**, so the team, partners and funders can see who the product is for and what their lives are like.
2. **Name who we are not serving**: not yet, or deliberately, and why.
3. **Test what we build** (secondary use): does the product make sense in each of these situations?

Personas don't decide what the product is. That comes first.

The minimum input is **a description of the product**: what it is, what it does, and who it serves.

Owner: Michele Pancera (IDEMS International). Personas often come from IDEMS and Parenting for Lifelong Health (PLH) work. The repo is **public** on GitHub, in the IDEMS International organization: https://github.com/IDEMSInternational/PersonAI

## Layout

| Path | Contents |
|---|---|
| `personas/` | Persona library: one file per persona, `firstname-lastname.md` |
| `personas/_template.md` | Persona template. Always use it. |
| `projects/` | One file per product: its description plus its persona map |
| `projects/_template.md` | Project template |
| `projects/_archive/` | Maps written under the earlier scope that don't fit the current one |
| `evaluations/` | Results of testing a spec/build against its personas (secondary use; format not settled yet) |
| `sources/` | Raw source material (slides, decks, photos). **Committed and public**, so only add material Michele has cleared. Includes the 2020 PLH Digital decks: 14 personas plus their user stories. |
| `decisions.md` | Dated log of every decision: what, why, status, and what's still open |

## Decisions so far

The current rules. When and why each was made is in `decisions.md`.

1. **Personas are reusable; scope is per project.** A persona file never says whether it is in or out of scope. The project file assigns each persona to a group, so the same person can be "building for" in one product and "not yet" in another.
2. **Three scope groups** in every project map:
   - **Building for now**: the situations the product serves. This is the set we show, and test against.
   - **Not building for, yet**: named on purpose, with why, and what would change that.
   - **Deliberately not for**: people the product shouldn't target, or could harm.
3. **The format follows the team's existing persona slides.** Reference example: Vimbai Moyo, a PLH facilitator, in `sources/` and `personas/vimbai-moyo.md`. Keep their sections: name + tagline ("the Bubbly Zimbabwean PLH Facilitator"), a quote, background, a day in the life, hopes & dreams, worries & fears, and what they're looking for. PersonAI adds:
   - **Their story**: a short narrative and the emotional core. The slides only carry emotion through the quote.
   - **Context & constraints**: device, connectivity/data cost, apps, language, time, support network.
   - **Where we'd lose them**: what makes them stop using or trusting the tech. Note that worries & fears are usually about their life or programme, not about the tech.
   - **Test questions**: concrete yes/no checks you can answer by looking at the spec or the product. They serve the secondary use, testing.
4. **Role relative to the product is explicit** (`role:` in the front matter). For example, Vimbai *delivers* PLH; caregivers and teens *receive* it. A set should cover the roles a product touches.
5. **Keep source material separate from invention.** Anything not taken from a source is marked `[draft]` or `[to confirm]`. Never present invented details as researched fact.
6. **Coverage dimensions.** For each project, pick a few dimensions that make situations differ (e.g. role, digital confidence, connectivity, language, motivation, rural/urban). Use them to make each persona a distinct situation, and to spot gaps in the set.
7. **Personas come after the product, and are mainly for communication** (scope change, 2026-10-06). They used to be meant for shaping the spec. Now the product is defined first, and the set shows the range of situations it serves. In practice:
   - Each "building for now" persona stands for a distinct situation, given in one line in the project map. If two personas share a situation, one of them is probably redundant.
   - The project map should make sense to someone outside the team who reads nothing else.
   - Testing stays, as a secondary use.
8. **Personas rest on layers of evidence** (agreed in principle, 2026-10-06): research → categories (situation types) → personas (each with a category and a grounding level) → project map → validation with real people. The pipeline will need more input than a product description. Details are still open (see `decisions.md`), and the templates and workflow haven't changed yet, so keep using the workflow below until they do.

## Workflow: "create personas for <product>"

1. **Input.** The product must already be defined. If it's unclear what the product *is* or *does*, ask: don't build personas around a guessed product. If `projects/<product>.md` doesn't exist, create it from the template using what Michele said. Other details (countries, languages, devices) can be marked assumptions.
2. **Reuse first.** Check `personas/` for existing personas that fit before writing new ones.
3. **Plan the set.** List the roles the product touches, the coverage dimensions, and the distinct situations they combine into. Propose people for all three scope groups, not just "building for". Usually that's around 5–10 personas in total.
4. **Write new personas** from `personas/_template.md`. Make them specific, warm and plausible for the setting. Avoid stereotypes. Mark invented details. Use the persona's own pronouns.
5. **Fill the project map** with the groups, a one-line situation and a reason for each placement, and the coverage gaps.
6. **Report back briefly**: the set, the gaps, and what needs confirming with real people.

## Workflow (secondary): "test <spec/build> against the personas"

Write a file in `evaluations/` named `<project>-<yyyy-mm-dd>.md`. Go through each "building for" persona's test questions and mark each one **pass / fail / unclear**, with evidence. Also flag anything in the spec that serves a "not for" persona at the expense of a "building for" one. The format isn't settled yet, so propose improvements as you go.

## Rules

- **The repo is public.** Don't commit or push persona content taken from real programmes, or any real photos or people, until Michele has confirmed it can be public. Raw material goes in `sources/`. When in doubt, ask before pushing.
- **Cleared for public (2026-10-06):** the PLH material, i.e. the persona decks and user stories in `sources/` and personas derived from them.
- Commit only when asked.
- **Log decisions as they're made.** When Michele makes or agrees a decision, including a partial one, add a dated entry to `decisions.md` in the same session, with why, its status and what's still open. Don't rewrite old entries: add a new one and mark the old one superseded. If the decision changes how Claude works, update this file too.

## Open questions

- How do we know a persona, or a set, is good? There's no definition of quality and no review step yet: the only check is Michele reading them (raised 2026-10-06).

- No license chosen yet (e.g. MIT for code, CC-BY for content).
- How a set is shown to people outside the team: one slide per persona like the original PLH slides, a one-page overview of the whole set, or both. The project map works for us, but isn't yet something to hand to a partner.
- The 2020 PLH Digital decks cover caregivers, teens, a facilitator, an intermediary and data users (M&E, research). Still missing: a manager role, and people already considered "not building for now".
- Is the library mainly shared and reused, or generated fresh per product? Current default: a shared library, reuse first.
- The evaluation format still needs designing (lower priority now that testing is secondary).
