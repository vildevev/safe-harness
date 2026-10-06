# Safe Harness

Teach software engineering while building with an AI coding agent.

Safe Harness is a small set of project instructions for beginners. It asks the agent to explain important decisions as they arise, make focused changes, check its work, and follow practical rules for authentication, data, secrets, and recovery.

Start with one file. No separate application or runtime is included.

## Choose your language

| Version | File | Teaching language |
| --- | --- | --- |
| English | [english/AGENTS.md](english/AGENTS.md) | English |
| Norsk bokmål | [norwegian/AGENTS.md](norwegian/AGENTS.md) | Norwegian Bokmål |

Both versions cover the same engineering principles. The Norwegian version is translated throughout. Code identifiers and commands retain their normal form; new code identifiers default to English.

## Get started

1. Choose one version above and open the file. On GitHub, use **Raw** to view or save the plain text.
2. Save it as `AGENTS.md` in the root of your project. If the project already has that file, merge the relevant sections into it and preserve its existing instructions.
3. Use a coding tool that supports `AGENTS.md`, or add the text through your tool's documented project-instruction mechanism. Loading and precedence rules vary by tool. The language folders in this repository are distribution copies; the chosen file belongs at your target project's root.
4. Start a new session if your tool requires it to reload instructions. Ask the agent to confirm it can see Safe Harness's instructions and its teaching language, then give it a small feature to build.

Example request:

> Help me build a recipe app. Start with adding and listing recipes. Explain important decisions briefly as we go.

## What to expect

- Short explanations tied to the feature being built.
- Meaningful product choices, without approval requests for every routine edit.
- Server-side authorization, careful secret handling, and appropriate validation.
- Relevant tests and honest reporting of what was actually checked.
- Careful handling of existing work and realistic recovery instructions.

For example, while adding private recipes, the agent should explain the difference between signing in and permission to access a recipe, then check that a different account is denied access.

## Norsk: Kom i gang

Åpne [den norske versjonen](norwegian/AGENTS.md), og lagre den som `AGENTS.md` i prosjektets rotmappe. Har du allerede en slik fil, fletter du inn instruksjonene uten å overskrive prosjektets egne regler. Bruk et kodeverktøy som støtter filen, eller legg teksten inn som prosjektinstruksjoner slik verktøyets dokumentasjon beskriver. Start en ny økt ved behov, og be agenten bekrefte at den ser instruksjonene og skal forklare på norsk.

Prøv for eksempel:

> Hjelp meg med å lage en oppskriftsapp. Begynn med å legge til og vise oppskrifter. Forklar viktige valg kort underveis.

## Scope and limitations

This is an instruction template. It does not enforce permissions, sandbox execution, create backups automatically, or guarantee secure code. Actual behavior depends on the coding tool, model, available capabilities, and other instructions. Tests passing does not establish production readiness.

The instructions have been reviewed for consistency; they have not yet been evaluated in controlled agent runs or user studies. Use a small project with synthetic data for your first trial.

## Improving the instructions

Keep changes concise and grounded in an observed problem. When changing an engineering rule, update both language versions. Reports are most useful when they include the coding tool, the task, expected behavior, and what happened, with secrets and personal data removed.
