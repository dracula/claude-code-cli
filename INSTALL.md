### [Claude Code CLI](https://claude.com/product/claude-code)

This port adds the Dracula theme to the Claude Code CLI.

Dracula is already built into the Claude Code desktop app and [claude.ai](https://claude.ai). If that's what you use, see [draculatheme.com/claude-code](https://draculatheme.com/claude-code) instead.

#### Install using Git

Clone the repository and link the theme so it stays up to date:

```bash
git clone https://github.com/dracula/claude-code-cli.git
mkdir -p ~/.claude/themes
ln -s "$(pwd)/claude-code-cli/Dracula.json" ~/.claude/themes/dracula.json
```

#### Install manually

Download the [GitHub `.zip` archive](https://github.com/dracula/claude-code-cli/archive/main.zip) and unzip it, or save [`Dracula.json`](./Dracula.json) directly. Then copy it into place:

```bash
mkdir -p ~/.claude/themes
cp Dracula.json ~/.claude/themes/dracula.json
```

Claude Code takes the theme's id from the filename, so keep it lowercase as `dracula.json`.

#### Activating the theme

1. Run `claude`, then enter `/theme`.
2. Select **Dracula** from the list.
3. Boom! It's working ✨

Claude Code watches `~/.claude/themes/`, so the theme shows up without a restart. If that folder didn't exist before you created it, restart `claude` once.
