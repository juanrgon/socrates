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

## Install in other agents

Clone or copy this repository into your agent's skills directory.

## How it works

Socrates reads the relevant source first, shows a small piece of evidence, asks one question, and waits. It builds on your answer until you reach the conclusion yourself.
