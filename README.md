# config_qtile

My [qtile](https://qtile.org) configuration (X11), set up for an **AZERTY** keyboard with keybindings close to i3 and sway.

## Installation

Dependencies (Debian):

```sh
sudo apt install qtile rofi i3lock
```

Get the config:

```sh
git clone git@github.com:antikkorps/config_qtile.git ~/.config/qtile
```

Then pick the **Qtile** session on the login screen, or reload a running session with `Super + Ctrl + r`.

## Keybindings

`Super` = Windows key. Arrow keys work wherever `h/j/k/l` do.

### Launch

| Keys | Action |
|---|---|
| `Super + d` | App launcher (rofi) |
| `Super + Tab` | Window switcher (rofi) |
| `Super + Enter` | Terminal |
| `Super + r` | Command prompt in the bar |
| `Super + Shift + e` | Session menu: lock, suspend, log out, reboot, power off |

### Windows

| Keys | Action |
|---|---|
| `Super + h/j/k/l` | Move focus |
| `Super + Shift + h/j/k/l` | Move window |
| `Super + Ctrl + h/j/k/l` | Grow window |
| `Super + n` | Reset window sizes |
| `Super + Space` | Next window |
| `Super + f` | Toggle fullscreen |
| `Super + t` | Toggle floating |
| `Super + w` | Close window |
| `Super + z` | Switch layout (columns / single window) |

### Workspaces

| Keys | Action |
|---|---|
| `Super + & é " ' ( - è _ ç` | Go to workspace 1 to 9 |
| `Super + Shift + & é " …` | Move window to that workspace and follow it |

Number keys are pressed without Shift: it's the top row of an AZERTY keyboard.

### Qtile

| Keys | Action |
|---|---|
| `Super + Ctrl + r` | Reload config |
| `Super + Ctrl + q` | Quit qtile |

## Files

- `config.py`: keybindings, workspaces, layouts, borders (dark blue, 3 px), bar
- `scripts/power-menu`: rofi session menu

Log file for troubleshooting: `~/.local/share/qtile/qtile.log`
