# act-like-an-owner

Reviews a supplied decision for reversibility, total effects, authority, and follow-through.

It produces:

- **Ownership Decision Review:** a working artifact built from supplied facts, labeled inference, and visible missing fields.

It executes the [Act Like An Owner playbook](https://www.andrewluxem.com/playbooks/act-like-an-owner). The playbook teaches the framework. This skill runs it and returns a working artifact.

**Static by construction: no dependencies, executable code, telemetry, network calls, remote instructions, auto-update, scheduled work, or background behavior.** It reads only the files in its own skill folder. Nothing happens until a user or agent invokes it.

## Install

Clone and copy the skill into Claude Code:

```bash
git clone https://github.com/andrewluxem/act-like-an-owner.git
cp -r act-like-an-owner/skills/act-like-an-owner ~/.claude/skills/
```

For Codex, copy the same complete folder to the Codex skills directory:

```bash
cp -r act-like-an-owner/skills/act-like-an-owner ~/.codex/skills/
```

Or install it as a Claude Code plugin:

```text
/plugin marketplace add andrewluxem/act-like-an-owner
/plugin install act-like-an-owner@act-like-an-owner
```

For clients that install from an archive, use the versioned [act-like-an-owner v1.0.0 ZIP](https://www.andrewluxem.com/downloads/act-like-an-owner-v1.0.0.zip).

## Invoke it

```text
Review this decision through an ownership lens
Use the act-like-an-owner skill.
```

Naming the skill is always valid: `use the act-like-an-owner skill`.

## Files

```text
.claude-plugin/
  plugin.json
  marketplace.json
skills/act-like-an-owner/
  assets/ownership-decision-review-template.md
  LICENSE.md
  meta.yaml
  references/ownership-standard.md
  SKILL.md
README.md
LICENSE
```

The complete canonical package is copied under `skills/act-like-an-owner/`, including every asset, reference, test prompt, source note, changelog entry, and license file present in the source.

## Versioning

Plugin installation is version-pinned. When behavior changes, update the version consistently in `SKILL.md`, `meta.yaml`, `.claude-plugin/plugin.json`, and `.claude-plugin/marketplace.json`, then add a changelog entry. Reinstalling is an explicit update; this repository never auto-updates itself.

## License

MIT. See [LICENSE](LICENSE). The canonical skill folder carries the same authorization in [skills/act-like-an-owner/LICENSE.md](skills/act-like-an-owner/LICENSE.md).

---

## More playbooks

This skill packages one playbook from the free library at [github.com/andrewluxem/playbooks](https://github.com/andrewluxem/playbooks). Every playbook is free to read, with no email required.