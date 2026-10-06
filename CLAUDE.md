# PersonAI: instructions for Claude

## Purpose

PersonAI builds **personas for specification guidance**. Each persona is a person we are trying to reach with the systems we build. Each one has a personal, emotional story. Personas are used to:

1. **Shape the spec**: what each persona needs from the system, and what would fail them.
2. **Show the whole set** of people we are building for, and who we are **not** building for at the moment.
3. **Test what we build**: does it make sense for these people?

The minimum input is **a description of the tech/system being developed**.

Owner: Michele Pancera (IDEMS International). Personas often come from IDEMS and Parenting for Lifelong Health (PLH) work. The repo is **public** on GitHub: https://github.com/MichelePancera/PersonAI

## Layout

| Path | Contents |
|---|---|
| `personas/` | Persona library: one file per persona, `firstname-lastname.md` |
| `personas/_template.md` | Persona template. Always use it. |
| `projects/` | One file per system: the input description plus its persona map |
| `projects/_template.md` | Project template |
| `evaluations/` | Results of testing a spec/build against its personas (format not settled yet) |
| `sources/` | Raw source material (slides, decks, photos). **Committed and public**, so only add material Michele has cleared. Includes the 2020 PLH Digital decks: 14 personas plus their user stories. |

## Decisions so far

1. **Personas are reusable; scope is per project.** A persona file never says whether it is in or out of scope. The project file assigns each persona to a group, so the same person can be "building for" in one system and "not yet" in another.
2. **Three scope groups** in every project map:
   - **Building for now**: the spec must serve them, and we test against them.
   - **Not building for, yet**: named on purpose, with why, and what would change that.
   - **Deliberately not for**: people the system shouldn't target, or could harm.
3. **The format follows the team's existing persona slides.** Reference example: Vimbai Moyo, a PLH facilitator, in `sources/` and `personas/vimbai-moyo.md`. Keep their sections: name + tagline ("the Bubbly Zimbabwean PLH Facilitator"), a quote, background, a day in the life, hopes & dreams, worries & fears, and what they're looking for. PersonAI adds:
   - **Their story**: a short narrative and the emotional core. The slides only carry emotion through the quote.
   - **Context & constraints**: device, connectivity/data cost, apps, language, time, support network.
   - **Where we'd lose them**: what makes them stop using or trusting the tech. Note that worries & fears are usually about their life or programme, not about the tech.
   - **Test questions**: concrete yes/no checks you can answer by looking at the spec or the system.
4. **Role relative to the system is explicit** (`role:` in the front matter). For example, Vimbai *delivers* PLH; caregivers and teens *receive* it. A set should cover the roles a system touches.
5. **Keep source material separate from invention.** Anything not taken from a source is marked `[draft]` or `[to confirm]`. Never present invented details as researched fact.
6. **Coverage dimensions.** For each project, pick a few dimensions that matter (e.g. role, digital confidence, connectivity, language, motivation, rural/urban). Use them to spot gaps in the set.

## Workflow: "create personas for <system>"

1. **Input.** If `projects/<system>.md` doesn't exist, create it from the template using what Michele said. Only ask questions if it's unclear what the system *is*. Everything else can be a marked assumption.
2. **Reuse first.** Check `personas/` for existing personas that fit before writing new ones.
3. **Plan the set.** List the roles the system touches and the coverage dimensions. Propose people for all three scope groups, not just "building for". Usually that's around 5–10 personas in total.
4. **Write new personas** from `personas/_template.md`. Make them specific, warm and plausible for the setting. Avoid stereotypes. Mark invented details. Use the persona's own pronouns.
5. **Fill the project map** with the groups, a reason for each placement, and the coverage gaps.
6. **Report back briefly**: the set, the gaps, and what needs confirming with real people.

## Workflow: "test <spec/build> against the personas"

Write a file in `evaluations/` named `<project>-<yyyy-mm-dd>.md`. Go through each "building for" persona's test questions and mark each one **pass / fail / unclear**, with evidence. Also flag anything in the spec that serves a "not for" persona at the expense of a "building for" one. The format isn't settled yet, so propose improvements as you go.

## Rules

- **The repo is public.** Don't commit or push persona content taken from real programmes, or any real photos or people, until Michele has confirmed it can be public. Raw material goes in `sources/`. When in doubt, ask before pushing.
- **Cleared for public (2026-10-06):** the PLH material, i.e. the persona decks and user stories in `sources/` and personas derived from them.
- Commit only when asked.

## Open questions

- No license chosen yet (e.g. MIT for code, CC-BY for content).
- The 2020 PLH Digital decks cover caregivers, teens, a facilitator, an intermediary and data users (M&E, research). Still missing: a manager role, and people already considered "not building for now".
- Is the library mainly shared and reused, or generated fresh per system? Current default: a shared library, reuse first.
- The evaluation format still needs designing.
