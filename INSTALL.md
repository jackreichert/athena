# Installing & Trying Athena

Athena follows the open **Agent Skills** format (`SKILL.md` with YAML frontmatter + optional references).

## Quick phrases

- “Install the Athena skill from https://github.com/jackreichert/athena”
- “Load the Athena skill from this repo”
- “Add the Athena study-guide skill”

## Try without permanently installing

Some agents let you load a skill directly from GitHub for a single session or evaluation, without writing it into the system prompt or skill library. This is useful when you want to see Athena’s syllabus + digest + theme approach before committing.

**AdaL / Adalagent** (example from the community):
```
skills:gh:jackreichert/athena
```
(Prefix with `@` if your client requires it for mentions.)  
The agent reads the skill straight from the public repo — nothing is saved.

Other platforms may support similar patterns (`skills:gh:owner/repo`, “load skill from URL”, etc.). Prefer the remote form when experimenting.

## Grok / xAI

Point the agent at the repository or the `athena/` folder. It should recognize the standard skill layout and load `SKILL.md` + references.

## Claude (Claude.ai, Claude Code, API)

1. Place the `athena/` directory where Claude Skills are expected, or use the skill-creator / Project skills flow.
2. The `name` and `description` in the YAML frontmatter drive progressive disclosure / triggering.
3. Claude loads the full skill when a matching task appears.

## ChatGPT Custom GPT

1. Create a new Custom GPT.
2. Copy the Markdown body of `athena/SKILL.md` (everything after the frontmatter) into the **Instructions** field.  
   For long contexts you can use a shorter operating prompt and keep the full skill as a knowledge file.
3. Upload `athena/references/` as **Knowledge**.
4. Optionally upload example finished packages.
5. Note in the instructions that output should be a portable set of Markdown files.

## Other agents / frameworks

Treat `SKILL.md` as the system or skill prompt and the `references/` files as supporting knowledge. Adapt file-writing paths to the tools the agent actually has.

## After loading

Try:

> Athena: teach me cognitive behavioral therapy

or

> Athena: build a study guide to the top things to see in the Prado Museum, focusing on Velázquez, Goya, and El Greco

or

> Athena research: produce a thematic study guide on Rawls’ original position / veil of ignorance.
