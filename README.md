# Handle with ADHD

![Handle with ADHD](assets/banner.png)

A behavior skill for Claude Code. Built by one ADHD adult, for himself, over
months of actually using it — not designed on a whiteboard.

## Why this exists

Two things about working with an AI assistant kept wearing me out:

**I never knew what it was actually doing.** Background processes I hadn't
asked about. Tool calls piling up while I waited. Reading half the codebase
before answering a one-line question. None of that is a bug in the normal
sense — it's just how these tools default to working. But if you have ADHD,
"I don't know what's happening right now" is its own kind of exhausting, on
top of whatever you were actually trying to get done.

**It kept asking me things I didn't have the energy to answer.** "Should I
do X or Y?" "Can you clarify?" Every one of those is a small decision, and
small decisions are the thing ADHD makes expensive. I wanted to say "just
handle it" and have that actually work.

So I wrote down the rules that fixed both, for me. This is that file.

## What it actually changes

- **Nothing runs without you knowing.** One line, before or as it happens —
  what's running and why. No discovering afterward that time got spent on
  something you didn't ask about.
- **It doesn't read everything up front "just in case."** It looks for what
  the task needs, when it needs it. Less waiting, less wasted cost.
- **Vague input gets acted on, not interrogated.** "Just handle it" means
  handle it. It only asks back when the decision genuinely can't be guessed.
- **It picks up where you left off, unprompted.** No "how can I help today" —
  a quick "here's where we were" instead.
- **Nothing gets written down only "at the end."** The moment something
  worth remembering gets said, it's saved. Sessions end abruptly sometimes —
  nothing should depend on reaching a tidy finish line first.
- **Messy input in, organized output out.** A brain dump becomes: what it
  means, why it matters, what to actually do — not a pile of the same words
  handed back with bullet points added.
- **It talks like a person, not a brochure.** Short. Direct. If you're wrong
  about something it says so and moves on, instead of cushioning it into
  three sentences.

## Why "proof over promise" and "no sycophancy" are in here

I went looking for research on AI-ADHD communication patterns that actually
drive engagement. There isn't much — mostly productivity-tool marketing and
general ADHD literature stretched to cover AI. The one concrete risk that
kept surfacing: LLMs trained to keep users engaged tend toward sycophancy —
agreeing, validating, softening — which reads as supportive but can quietly
build dependency without building anything real. For a brain that already
struggles to tell "felt reassured" apart from "actually handled," an AI that
optimizes for the former is a bad trade. So this skill deliberately doesn't:
no engagement-maximizing agreement, and no "done" without something you can
check. Boring and verifiable beats validating and vague.

## What this isn't

Not a clinical tool. Not a substitute for anything you and a doctor have
worked out. Not tested on anyone but me. It might do nothing for you — ADHD
doesn't work the same way twice. I'm publishing it because the thing that
helped me doesn't seem to exist anywhere else yet, not because I think it's
universal.

## Install

Drop this folder into `~/.claude/skills/handle-with-adhd/`, then start a
session with `/handle-with-adhd`. That's it — no config, no accounts, no
dependencies.

## License

MIT. Take it, change it, tell me if you fix something I didn't see.
