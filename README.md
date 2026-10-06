# PersonAI

Personas as a communication tool: once we know what a product will be, a set of personas shows the different situations it serves.

## Idea

Each persona is a person in one of the situations a product serves. Every persona has a personal, emotional story: who they are, what they live with, what they need, and what would make them trust or give up on what we build.

Given a description of a product, PersonAI helps us:

1. **Show the range of situations we serve**, so the team, partners and funders can see who the product is for and what their lives are like.
2. **Name who we are not serving**: not yet, or deliberately, and why.
3. **Test what we build** (secondary use): walk each persona through the product and ask whether it makes sense for them.

Personas don't decide what the product is. That comes first.

## Input

At minimum: a description of the product, meaning what it is, what it does and who it serves. Optional extras include the setting, constraints, and existing specs.

## Structure

| Folder | Contents |
|---|---|
| [`personas/`](personas/) | The persona library: one file per persona |
| [`projects/`](projects/) | One file per product: its description and its persona map |
| [`evaluations/`](evaluations/) | Results of testing a product against its personas |

Templates: [`personas/_template.md`](personas/_template.md) and [`projects/_template.md`](projects/_template.md).

## Scope groups

Personas are reusable across projects. Each project places them in one of three groups:

- **Building for now**: the situations the product serves. This is the set we show, and test against.
- **Not building for, yet**: named on purpose, with why, and what would change that.
- **Deliberately not for**: people the product shouldn't target, or could harm.

## Using it

Open this repo with Claude Code and ask, for example, *"create personas for &lt;product&gt;"* or *"test this spec against the personas"*. The process is described in [`CLAUDE.md`](CLAUDE.md).

## Status

Early setup: a draft persona template, a draft project template, and a first persona set for PLH Digital. How a set is presented to people outside the team, and the evaluation format, come next.
