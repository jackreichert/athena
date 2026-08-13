# Installing Athena

Athena follows the open **Agent Skills** format (`SKILL.md` with YAML frontmatter + optional references).

## Quick install phrases you can use with agents

- “Install the Athena skill from https://github.com/jackreichert/athena”
- “Load the Athena skill from this repo”
- “Add the Athena study-guide skill”

## Grok / xAI

Point the agent at the repository or the `athena/` folder. It should recognize the standard skill layout and load `SKILL.md` + references.

## Claude (Claude.ai, Claude Code, API)

1. Place the `athena/` directory in the location your Claude Skills system expects (commonly a skills folder or via the skill-creator flow).
2. The `name` and `description` in the YAML frontmatter are used for progressive disclosure / triggering.
3. Claude will load the full skill when a matching task appears.

## ChatGPT Custom GPT

1. Create a new Custom GPT.
2. Copy the Markdown body of `athena/SKILL.md` (everything after the frontmatter) into the **Instructions** field.  
   (For very long contexts you may prefer a condensed operating prompt + the full skill as a knowledge file.)
3. Upload the contents of `athena/references/` as **Knowledge**.
4. Optionally upload example finished packages.
5. In the instructions, note that output should be a portable set of Markdown files.

## Other agents / frameworks

Treat `SKILL.md` as the system or skill prompt and the `references/` files as supporting knowledge. Adapt file-writing paths to the tools the agent actually has.

## After installation

Ask for something like:

> Athena: build a study guide to the top things to see in the Prado Museum, focusing on Velázquez, Goya, and El Greco.

or

> Athena research: produce a thematic study guide on Rawls’ original position / veil of ignorance.
