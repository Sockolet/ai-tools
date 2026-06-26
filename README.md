# ai-tools

Personal AI tools, reusable prompts, and skill definitions.

This repository keeps reusable AI assistant assets in two forms:

- `PROMPTS/`: source prompts that can be copied, adapted, or used as the basis for new workflows.
- `SKILLS/`: packaged skill definitions derived from selected prompts, ready to install or sync into a compatible AI assistant skills directory.

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

## Prompts

The `PROMPTS/` folder contains the original reusable prompt templates:

| Prompt | Purpose |
|---|---|
| `CODE-REVIEW-PROMPT.md` | Review code or changes for concrete engineering issues. |
| `DOCUMENTATION-PROMPT.md` | Produce beginner-friendly implementation documentation. |
| `PLAN-PROMPT.md` | Create detailed implementation plans without modifying code. |
| `PROMPT-ENHANCER.md` | Rewrite draft prompts into stronger reusable prompts. |

## Skills

The `SKILLS/` folder contains skill-ready versions of selected prompts:

| Skill | Purpose |
|---|---|
| `code-review` | Senior-engineer code review. |
| `implementation-docs` | Technical implementation report generation. |
| `implementation-plan` | Detailed implementation planning. |
| `prompt-enhancer` | Prompt improvement and rewrite. |

Each skill is stored in its own directory with a `SKILL.md` file containing frontmatter metadata and the skill instructions.
