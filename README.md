# Prevent Defensive AI Writing Skill

This repository contains a Codex skill for preventing defensive, self-undermining, over-apologetic AI writing.

The skill trains Codex to write with confident precision: foreground the strongest evidence-backed contribution, narrow claims when needed, handle weak results without self-attack, and avoid giving reviewers or readers unnecessary attack surfaces.

## What It Does

- Rewrites drafts to remove defensive caveats and self-weakening language.
- Helps academic, technical, and research writing focus on the strongest supported story.
- Reframes weak or mixed results as scoped claims, tradeoffs, or evidence boundaries.
- Keeps necessary limitations honest, exact, and proportional.
- Encourages launch-style writing instead of lab diary, project report, or apology-driven prose.

## Install

Clone this repository, then copy the skill folder into your Codex skills directory:

```bash
git clone https://github.com/Tina0514/prevent-defensive-ai-writing-skill.git
cd prevent-defensive-ai-writing-skill
mkdir -p "${CODEX_HOME:-$HOME/.codex}/skills"
cp -R prevent-defensive-ai-writing "${CODEX_HOME:-$HOME/.codex}/skills/"
```

Restart Codex after installation if the skill does not appear immediately.

## Usage

Example prompts:

```text
Use $prevent-defensive-ai-writing to revise this abstract so it foregrounds the strongest supported contribution and removes unnecessary caveats.
```

```text
Use $prevent-defensive-ai-writing to audit this manuscript introduction for defensive framing, weak claims, and reviewer-facing attack surfaces.
```

```text
Use $prevent-defensive-ai-writing to rewrite this reviewer response so it is direct, evidence-based, and not over-apologetic.
```

```text
Use $prevent-defensive-ai-writing to turn these mixed results into a narrower, stronger, evidence-aligned story.
```

## Publish To GitHub

From this repository directory:

```bash
git init
git add .
git commit -m "Add prevent defensive AI writing skill"
git branch -M main
```

Create a new empty repository on GitHub named `prevent-defensive-ai-writing-skill`, then push:

```bash
git remote add origin https://github.com/Tina0514/prevent-defensive-ai-writing-skill.git
git push -u origin main
```

If you use GitHub CLI:

```bash
gh repo create Tina0514/prevent-defensive-ai-writing-skill --public --source=. --remote=origin --push
```

## Repository Structure

```text
prevent-defensive-ai-writing-skill/
├── README.md
├── LICENSE
└── prevent-defensive-ai-writing/
    ├── SKILL.md
    └── agents/
        └── openai.yaml
```

## License

MIT
