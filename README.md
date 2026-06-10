# Socrates

A portable agent skill for understanding code and concepts through a source-grounded Socratic dialogue, one question at a time.

## Install in Pi

```bash
pi install git:github.com/juanrgon/socrates
```

Then use:

```text
/socrates why does this retry fail?
```

Pi also exposes the skill directly as `/skill:socrates`.

## Install in Claude Code

```bash
mkdir -p ~/.claude/skills
git clone https://github.com/juanrgon/socrates.git ~/.claude/skills/socrates
```

## Install in Codex CLI

```bash
mkdir -p ~/.codex/skills
git clone https://github.com/juanrgon/socrates.git ~/.codex/skills/socrates
```

## Install in Copilot CLI

```bash
mkdir -p ~/.copilot/skills
git clone https://github.com/juanrgon/socrates.git ~/.copilot/skills/socrates
```

Restart the CLI after installing so it discovers the skill.

If you use multiple agents, clone the repository once and symlink it into each skills directory instead of maintaining duplicate clones.

## How it works

Socrates reads the relevant source first, shows a small piece of evidence, asks one question, and waits. It builds on your answer until you reach the conclusion yourself.
