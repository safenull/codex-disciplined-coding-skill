# Codex Disciplined Coding Skill

A native OpenAI Codex skill for disciplined coding workflows.

The skill helps Codex stay focused on:

- thinking before coding
- simple implementations
- surgical diffs
- explicit assumptions
- verification before claiming success

## Structure

```text
.agents/skills/disciplined-coding/SKILL.md
```

## Install in a repository

Copy the skill folder into your target project:

```bash
mkdir -p .agents/skills
cp -R .agents/skills/disciplined-coding /path/to/your-project/.agents/skills/
```

Commit it in the target project:

```bash
git add .agents/skills/disciplined-coding/SKILL.md
git commit -m "Add disciplined coding Codex skill"
```

## Install globally

```bash
mkdir -p "$HOME/.agents/skills"
cp -R .agents/skills/disciplined-coding "$HOME/.agents/skills/"
```

## Usage

Ask Codex explicitly:

```text
Use disciplined-coding. Fix this bug with the smallest safe change and verify it.
```

Other useful prompts:

```text
Use disciplined-coding. Review this PR for overengineering, unrelated edits, and missing verification.
```

```text
Use disciplined-coding. Refactor only the requested area and preserve behavior.
```

## Credits

Inspired by Andrej Karpathy's public guidance on coding agents, especially the ideas of thinking before coding, simplicity, surgical changes, and verification loops.

Also inspired by the community project commonly referred to as `andrej-karpathy-skills`.

This is an independent Codex-native adaptation. It is not affiliated with or endorsed by Andrej Karpathy.

## License

MIT.
