# tmux config

Prefix: `C-Space`

## Hotkeys (prefix required)

### Navigation
| Key | Action |
|-----|--------|
| `a` | fzf session picker |
| `w` | fzf window picker |
| `s` | enter stack mode (see below) |
| `h/j/k/l` | select pane left/down/up/right |
| `1-9` | select window by number |
| `n/p` | next/previous window (repeatable) |

### Sessions & Windows
| Key | Action |
|-----|--------|
| `b` | break window out to its own session |
| `.` | move window to another session |
| `$` | rename session |
| `,` | rename window |
| `c` | new window |
| `&` | kill window |
| `x` | kill pane |

### Panes
| Key | Action |
|-----|--------|
| `\|` | split horizontal |
| `-` | split vertical |
| `m` | move pane to another window (prompts) |
| `M` | break pane out to its own window |
| `V` | mark pane, then `v` to join below |
| `z` | toggle pane zoom |
| `</>` | swap pane up/down (repeatable) |
| `H/J/K/L` | resize pane (repeatable) |
| `P/N` | swap window left/right (repeatable) |

### Layouts: `W` then...
| Key | Action |
|-----|--------|
| `1` | even-horizontal (side-by-side) |
| `2` | even-vertical (stacked) |
| `3` | main-horizontal (big top) |
| `4` | main-vertical (big left) |
| `5` | tiled |
| `=` | equalize, preserve layout |

### Stacks: `s` then...
| Key | Action |
|-----|--------|
| `2` | new 2-pane stack |
| `3` | new 3-pane stack |
| `c` | new stack with claude in top pane |
| `s` | choose-session (built-in tree) |

### Misc
| Key | Action |
|-----|--------|
| `r` | reload config |
| `C-k` | clear pane + history |
| `S` | toggle synchronized panes |
| `=` | equalize panes |

## No-prefix hotkeys
| Key | Action |
|-----|--------|
| `Alt-Up/Down` | select pane up/down |
| `Cmd-Opt-Up/Down` | select pane up/down (iTerm2) |
| `Ctrl-Left/Right` | select pane left/right |
| `Shift-Left/Right` | delete word backward/forward |
| `PageUp/Down` | enter copy mode / scroll |

## Bash commands (`.tmux-rc`)
| Command | Action |
|---------|--------|
| `tml [pattern ...]` | list sessions (with window names, time, status) |
| `tmlw [pattern ...]` | list all windows, optionally filtered by session |
| `tma <session>` | attach to session |
| `tmc <session>` | attach or create session |
| `tmn <name>` | new session |
| `tmk <session ...>` | kill session(s) |
| `tmkw <sess:win ...>` | kill window(s) |
| `tmka` | kill all detached sessions |
| `tms <session>` | switch to session (from within tmux) |
| `tmr <name>` | rename current session |
| `tmpo [name]` | pop current window out to its own session |

## Copy mode (vi keys)
| Key | Action |
|-----|--------|
| `v` | begin selection |
| `y` | copy to clipboard |
| `C-Up/Down` | scroll 5 lines |
| Mouse drag | select + copy |
| Double-click | select word + copy |
| Right-click | paste |
