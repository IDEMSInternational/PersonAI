# PersonAI

Personas for specification guidance: a way to check whether the systems we build make sense for the people we want to reach.

## Idea

Each persona is a person we are trying to reach with our work. Every persona has a personal, emotional story: who they are, what they live with, what they need, and what would make them trust or give up on what we build.

Given a description of the technology we are developing, PersonAI helps us:

1. **Generate or select personas** relevant to that technology.
2. **Guide the specification**: what each persona needs from the system, and what would fail them.
3. **Test what we build**: walk each persona through the system and ask whether it actually makes sense for them.

## Input

At minimum: a description of the tech being developed. Optional extras include the context, target users, constraints, and existing specs.

## Structure

| Folder | Contents |
|---|---|
| [`personas/`](personas/) | The persona library: one file per persona |
| [`projects/`](projects/) | Inputs: descriptions of the tech/systems being developed |
| [`evaluations/`](evaluations/) | Results of testing a project against its personas |

## Status

Early setup. The persona format, generation and evaluation process come next.
