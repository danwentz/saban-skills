# Saban Skills for Claude

Three AI agent skills (Claude, Codex and other Agent Skills tools) based on how Nick Saban ran his programs. He won seven national titles (LSU 2003; Alabama 2009, 2011, 2012, 2015, 2017, 2020). Each skill takes one part of his approach and turns it into a step-by-step workflow you can use for sales, hiring, projects or any other goal.

| Skill | Use it when | What you get |
|---|---|---|
| [`saban-process-plan`](skills/saban-process-plan/SKILL.md) | You have a big goal: a quota, a launch, a renewal, a season | The goal turned into daily and weekly tasks you control, each with a written standard, plus practice steps, an 18-month calendar, a daily schedule and a list of distractions to cut |
| [`saban-24-hour-review`](skills/saban-24-hour-review/SKILL.md) | You just won, lost or finished something big | The 24-hour rule, a grade on how you worked (not the result), a check for complacency after wins or the lesson after losses, a check on whether your methods need updating, and your next step |
| [`saban-standard-roster`](skills/saban-standard-roster/SKILL.md) | You're hiring or picking clients, prospects or partners | A short list of must-have traits for the role, evidence-based grading, character checks through references, a trial period, and one standard for everyone |

They work as a loop: plan the process, run it, review it, keep the right people in it.

## Install

### Claude apps (claude.ai, desktop, mobile)

1. Download a skill zip from the [`dist/`](dist/) folder (or from the [latest release](https://github.com/danwentz/saban-skills/releases/latest)).
2. In Claude, open the Skills section of your settings and upload the zip.
3. Do the same for each skill you want.

### Claude Code: plugin marketplace

```
/plugin marketplace add danwentz/saban-skills
/plugin install saban-skills@saban-skills
```

### Claude Code: manual

Copy each folder in `skills/` into `~/.claude/skills/` (just for you) or `.claude/skills/` (for one project):

```bash
git clone https://github.com/danwentz/saban-skills.git
cp -r saban-skills/skills/* ~/.claude/skills/
```

### OpenAI Codex (CLI, IDE extension, ChatGPT desktop app)

Install as a plugin:

```
codex plugin marketplace add danwentz/saban-skills
codex plugin add saban-skills@saban-skills
```

Or install manually. These skills follow the open [Agent Skills](https://agentskills.io) format, which Codex also reads. Copy them into `~/.agents/skills/` (just for you) or `.agents/skills/` in a repo (for one project):

```bash
git clone https://github.com/danwentz/saban-skills.git
mkdir -p ~/.agents/skills
cp -r saban-skills/skills/* ~/.agents/skills/
```

Restart Codex if they don't show up. Invoke one with `$saban-process-plan`, or just describe your goal and Codex will pick the right skill.

### Other agents

Any tool that supports Agent Skills (`SKILL.md` folders) can use these. Copy the folders in `skills/` into that tool's skills directory.

## Example prompts

- "I need to write $400K in new commercial premium by Q3 next year. Build me the process."
- "I lost the Hendricks renewal to a competitor today. Run the review."
- "We closed our biggest deal of the year. Rat-poison check me."
- "Here are five prospects. Grade them like Saban would grade recruits."
- "I'm hiring an account manager. Help me define the critical factors."

## Where the material comes from

The skills are based on Saban's own public statements and reporting on his programs. See [SOURCES.md](SOURCES.md). Quotes that are often credited to him without good evidence were left out.

## Disclaimer

This is an independent project. It isn't affiliated with or endorsed by Nick Saban, the University of Alabama, Michigan State University, LSU or any team. Names are used only to describe the source of the ideas.

## License

MIT. See [LICENSE](LICENSE).
