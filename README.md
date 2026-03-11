# SkillProof Marketplace

This is the **marketplace repo** for the [SkillProof](https://github.com/m24927605/skillproof) Claude Code plugin. It tells Claude Code where to download and install the plugin.

> **What is SkillProof?** A Claude Code plugin that generates verifiable developer resumes by scanning your source code. See the [main repo](https://github.com/m24927605/skillproof) for full documentation.

## Installation

> **Prerequisites:** [Claude Code CLI](https://docs.anthropic.com/en/docs/claude-code) installed and working.

**Step 1.** Add this marketplace — run one of the following:

```bash
# Inside a Claude Code session:
/plugin marketplace add m24927605/skillproof-marketplace

# Or from the terminal:
claude plugin marketplace add https://github.com/m24927605/skillproof-marketplace.git
```

**Step 2.** Install the plugin:

```bash
# Inside a Claude Code session:
/plugin install skillproof@skillproof-marketplace

# Or from the terminal:
claude plugin install skillproof@skillproof-marketplace --scope user
```

**Step 3.** Restart your Claude Code session.

**Step 4.** Verify — type `/skillproof` in Claude Code. You should see 7 commands in the autocomplete menu:

| Command | Description |
|---------|-------------|
| `/skillproof-all` | Run the entire resume generation pipeline |
| `/skillproof-scan` | Scan repository and generate evidence graph |
| `/skillproof-infer` | Infer skills from evidence |
| `/skillproof-render` | Generate a locale-aware resume from verified skills |
| `/skillproof-sign` | Sign resume manifest |
| `/skillproof-pack` | Create distributable resume bundle |
| `/skillproof-verify` | Verify resume bundle authenticity |

## Updating

```bash
/plugin update skillproof@skillproof-marketplace
```

## Uninstalling

```bash
/plugin uninstall skillproof@skillproof-marketplace
```

## What's Included

| Plugin | Description |
|--------|-------------|
| **[skillproof](https://github.com/m24927605/skillproof)** | Generate verifiable developer resumes from source code repositories |
