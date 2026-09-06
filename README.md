# ai-tools

Personal AI tools, reusable prompts, and skill definitions.

Each tool comes in two equivalent forms:

- `PROMPTS/`: standalone prompts to copy, adapt, or use as the basis for new workflows.
- `SKILLS/`: the same instructions packaged for installation or syncing into a compatible AI assistant skills directory.

`AGENTS.md` provides shared behavioral guidelines for coding and non-coding work.

## Structure

```text
.
├── AGENTS.md
├── PROMPTS/
│   ├── CODE-REVIEW-PROMPT.md
│   ├── DOCUMENTATION-PROMPT.md
│   ├── PLAN-PROMPT.md
│   └── PROMPT-ENHANCER.md
├── SKILLS/
│   ├── code-review/
│   │   └── SKILL.md
│   ├── implementation-docs/
│   │   └── SKILL.md
│   ├── implementation-plan/
│   │   └── SKILL.md
│   └── prompt-enhancer/
│       └── SKILL.md
└── README.md
```

## Tools

Use a prompt directly or install its matching skill:

| Prompt (`PROMPTS/`) | Skill (`SKILLS/`) | Purpose |
|---|---|---|
| `CODE-REVIEW-PROMPT.md` | `code-review` | Senior-engineer review of code or changes for concrete engineering issues. |
| `DOCUMENTATION-PROMPT.md` | `implementation-docs` | Comprehensive, beginner-friendly implementation reports. |
| `PLAN-PROMPT.md` | `implementation-plan` | Detailed implementation plans without modifying code. |
| `PROMPT-ENHANCER.md` | `prompt-enhancer` | Rewrite draft prompts into stronger reusable prompts. |

## Maintaining both forms

Each skill has its own directory and a `SKILL.md` containing `name` and `description` frontmatter followed by the tool instructions. Keep those instructions identical to the matching prompt when editing either form. Packaging is the only difference: skills add discovery metadata; standalone prompts may add an input placeholder, such as the draft block in `PROMPT-ENHANCER.md`.
