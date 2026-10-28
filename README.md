# Handle with ADHD

[![skills.sh](https://skills.sh/b/lubianiec/handle-with-adhd)](https://skills.sh/lubianiec/handle-with-adhd)

![Handle with ADHD](assets/banner.png)

An AI assistant that tells you what it's doing, doesn't make you answer
questions you don't have energy for, and picks up where you left off.
I wrote it for myself and I've used it every day since July 2026.

## Install

**One command** — installs into whatever agent you use (Claude Code, Codex,
Cursor, Hermes and ~75 more):

```sh
npx skills add lubianiec/handle-with-adhd
```

**Or by hand.** The skill is one file: `SKILL.md`, with standard frontmatter
(`name`, `description`, `user-invocable`). Anything that reads skills reads it.

**Claude Code**

```sh
mkdir -p ~/.claude/skills/handle-with-adhd
cp SKILL.md ~/.claude/skills/handle-with-adhd/
```

Then `/handle-with-adhd` in a session. It stays on until you say "stop adhd
mode".

**Cursor**

Copy `SKILL.md` into `.cursor/rules/handle-with-adhd.mdc` in the project, or
into your global rules directory, and delete the YAML frontmatter — Cursor
wants its own header. Add:

```
---
description: ADHD operating mode
alwaysApply: false
---
```

and paste the body below it.

**Codex**

Put `SKILL.md` in `~/.codex/skills/handle-with-adhd/` (or your project's
skills folder) and reference it at the start of the session, or paste the body
into `AGENTS.md`. It's plain markdown — no tooling required.

**Any other agent**

If it can read a file, it can use this. Load `SKILL.md` as a system or context
document and the rules take effect. No config, no accounts, no dependencies.

## What it changes

- **Nothing runs without you knowing.** One line before or as it happens:
  what's running and why. No discovering afterward that time went somewhere
  you didn't ask for.
- **It doesn't read the whole repo "just in case."** Looks for what the task
  needs, when it needs it. Less waiting, less cost.
- **"Just handle it" means handle it.** Vague input gets acted on. It asks
  back only when a decision genuinely can't be guessed.
- **It picks up where you left off** instead of asking how it can help today.
- **Memory is captured the moment it's said,** not "at the end." Sessions end
  abruptly; nothing should wait for a tidy finish line.
- **Messy input in, organized output out.** A brain dump becomes what it
  means, why it matters, what to do — not the same words with bullets.
- **No sycophancy.** It tells you when you're wrong and moves on. No "done"
  without something you can check.

## Honest limits

Not a clinical tool, not a substitute for anything you and a doctor have
worked out, not tested on anyone but me. It might do nothing for you — ADHD
doesn't work the same way twice.

Two of the rules came from reasoning, one from research. The anti-sycophancy
rule has real backing: LLM sycophancy is linked to eroded trust, emotional
dependency, and worse mental-health outcomes over time. "Proof over promise"
has no study directly behind it — it stays because it works for me, and I'm
labelling it as exactly that. One rule is evidence-backed, the other is a good
bet.

I'm publishing it because the thing that helped me doesn't seem to exist
elsewhere yet, not because I think it's universal.

## License

MIT. Take it, change it, tell me if you fix something I didn't see.
