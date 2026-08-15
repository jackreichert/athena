# Install Athena

**Skill file (the instructions agents actually load):**  
https://raw.githubusercontent.com/jackreichert/athena/main/athena/SKILL.md

## Quick install patterns

### Grok / xAI agents that support Skills
- Point the skill loader at this repository, or  
- Use the raw skill URL above.

### Claude (Projects / Skills / Custom instructions)
- Add the raw SKILL.md URL as a knowledge / skill file, or  
- Paste the contents of `athena/SKILL.md` into project instructions / custom instructions.  
- The `references/` files (digest template, directory layout) can be added as additional knowledge if the runtime supports multi-file skills.

### Other agents / Custom GPTs / similar
- Many runtimes only discover a skill when given an explicit URL. Always prefer the raw GitHub link above.
- For “install this repo” workflows, the repository root contains `README.md`, `INSTALL.md`, and the `athena/` directory holding `SKILL.md` + `references/`.

## After install

Try:

```
Athena on [topic]
Athena go deep on [topic]
Athena museum guide for [museum or collection]
```

The skill produces a self-contained Markdown package (scope, provenance-annotated sources + full working bibliography, digests, themes, further reading, etc.) that can be opened in Obsidian, VS Code, or any Markdown-friendly reader.
