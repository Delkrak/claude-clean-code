# Clean Code skill for Claude Code

A Claude Code plugin marketplace containing the `clean-code` plugin: a skill with Clean Code style rules that keep Claude's code readable and maintainable — clean comments, clean variable and function naming, and incremental refactoring.

## Install

```
/plugin marketplace add Delkrak/claude-clean-code
/plugin install clean-code@claude-clean-code
```

A local clone works too: `/plugin marketplace add <path-to-this-repo>`.

## Project modifications

A project can adjust the rules by adding `clean-code-modifications.md` to its root, with rules numbered `§M.*`. Modifications take precedence over the base rules and clarifications (see §1.3 in the skill).

## License

Copyright 2026 Delkrak. Licensed under the [Apache License 2.0](LICENSE).
