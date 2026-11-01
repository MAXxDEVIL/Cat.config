# Cat.config

Personal Arch Linux desktop configuration — **Niri** (Wayland) with kitty, fish, starship, cava and fastfetch, plus a curated library of AI agent skills, frontend UI resources and Omarchy themes.

Everything here is stored as copy-paste-ready Markdown snippets rather than live dotfiles, so the repo doubles as a reference sheet you can read on GitHub and a source you can pull configs from.

```
Arch Linux · Niri · Noctalia Shell · kitty · fish · starship · fastfetch · cava
```

---

## Repository layout

```
Cat.config/
├── configs/                 # Desktop configuration snippets
│   ├── niri-config.md       # Niri keybindings (config.kdl)
│   ├── k-win.md             # Window layout presets as percentage zones
│   ├── kitty.md             # Terminal appearance + keymaps
│   ├── fish.md              # Shell init, PATH and prompt wiring
│   ├── starship_tomel.md    # Starship prompt (purple powerline theme)
│   ├── fastfetch.md         # Fastfetch JSON with a custom kitty logo
│   └── cava.md              # Audio visualizer (blue gradient bars)
├── themes/
│   └── Omarchy.md           # Omarchy themes with previews + clone URLs
├── img/
│   ├── background/          # Wallpapers (2560×1440 JPEG, 1280×720 PNG)
│   └── pokimons/            # Transparent mascot PNGs used as terminal logos
├── agents_skill.md          # Curated AI agent skill repositories by category
├── Web_component.md         # Frontend component / inspiration sites
├── codes.md                 # Cheat sheet: git, disks, pacman, yay, BitLocker
└── README.md
```

---

## Desktop stack

| Layer | Choice |
| --- | --- |
| OS | Arch Linux |
| Compositor | [Niri](https://github.com/YaLTeR/niri) — scrollable tiling on Wayland |
| Shell / bar | [Noctalia Shell](https://docs.noctalia.dev) via `qs` (Quickshell IPC) |
| Terminal | kitty |
| Shell | fish |
| Prompt | starship |
| System info | fastfetch |
| Visualizer | cava |
| File manager | dolphin |
| Apps | kitty, VS Code, Chrome (Flatpak), Spotify (Flatpak), Discord, WhatsApp Desktop |

---

## Configuration files

| File | Copy to | What it does |
| --- | --- | --- |
| `configs/niri-config.md` | `~/.config/niri/config.kdl` | Full `binds {}` block: app launchers, media/brightness keys, window + workspace movement, layout sizing, screenshots, power |
| `configs/k-win.md` | Layout JSON read by the layout tool | Named presets for 1–9 windows plus 70/30 vertical and horizontal splits, defined as percentage zones |
| `configs/kitty.md` | `~/.config/kitty/kitty.conf` | JetBrainsMono Nerd Font at 11.5pt, 0.88 opacity, cyan-on-navy palette, `ctrl+shift+f2` split |
| `configs/fish.md` | `~/.config/fish/config.fish` | Starship init, opencode / pnpm / nvm paths, and the command to silence the login greeting |
| `configs/starship_tomel.md` | `~/.config/starship.toml` | Purple powerline prompt: OS, user, directory, git, 10 language modules, time |
| `configs/fastfetch.md` | `~/.config/fastfetch/config.jsonc` | Boxed Hardware / Software / Uptime sections in `#926ee4`, kitty image logo |
| `configs/cava.md` | `~/.config/cava/config` | 60 fps noncurses bars with an 8-stop blue gradient and a transparent background |

> **Snippets are fenced.** Each file wraps its content in a Markdown ```` ``` ```` block. Copy only the lines inside the fence — not the headings or the fence markers.

### Keybindings at a glance

`Mod` is the Niri modifier (Super). Highlights from `configs/niri-config.md`:

| Keys | Action |
| --- | --- |
| `Mod+Return` | kitty |
| `Mod+Space` | Noctalia launcher |
| `Mod+B` / `Mod+S` / `Mod+D` | Chrome / Spotify / Discord |
| `Mod+W` / `Mod+V` / `Mod+E` | WhatsApp / VS Code / dolphin |
| `Mod+H J K L` / arrows | Focus window |
| `Mod+Ctrl+H J K L` | Move column / window |
| `Mod+1…9` / `Mod+Ctrl+1…9` | Focus / move to workspace |
| `Mod+F` / `Mod+T` | Fullscreen / floating |
| `Mod+F1` / `Mod+F2` / `Ctrl+Shift+3` | Screenshot screen / picker / window |
| `Mod+Shift+Q` / `Mod+Alt+L` | Session menu / lock screen |

---

## Setup

```bash
git clone https://github.com/MAXxDEVIL/Cat.config.git
cd Cat.config
```

1. **Install packages** (see `codes.md`), then create the target directories:

   ```bash
   mkdir -p ~/.config/{niri,kitty,fish,fastfetch,cava}
   ```

2. **Copy each snippet** from `configs/` into its destination from the table above.
3. **Reload**: `niri msg action reload-config` for Niri, and open a new terminal for kitty/fish/starship changes.

### Edit before you copy

These values are specific to the original machine:

- **fastfetch** — `logo.source` points at `/home/mr_cat/Pictures/imp/dra.png`. Change it to your own path, or use one of the PNGs in `img/pokimons/`.
- **fish** — the Node path is pinned to `~/.nvm/versions/node/v22.21.1/bin`; update it for your installed version.
- **niri** — WhatsApp is launched from `/opt/WhatsApp Desktop/whatsapp-linux-desktop`, and Noctalia Shell must be installed for the `qs -c noctalia-shell ipc call …` bindings to work.
- **kitty / fastfetch** — install `ttf-jetbrains-mono-nerd` (or any JetBrainsMono Nerd Font) or the glyphs will fall back to boxes.
- **cava** — `method = noncurses` is meant to be embedded in a bar; switch to `ncurses` to run it standalone in a terminal.

---

## Reference material

### `themes/Omarchy.md`

Ten [Omarchy](https://github.com/basecamp/omarchy) themes with preview images and clone URLs — Space (Event Horizon), Last Horizon, Cyberpunk, Batou, Black Arch, Black Gold, Blackwall, Cpunk, Koyanagi and Rustleaf.

### `agents_skill.md`

Curated skill repositories grouped by what you are building:

- **Application and Web builder** — 30 entries (ECC, GSD, REA, Paperclip, Gravitas, Ponytail, Graphify, Playwright CLI, GSAP, ui-ux-pro-max, humanizer, Scrapling, …)
- **Animation builder**, **Unlimited Token**, **Game builder**, **Job Search**, **Tester**
- **Video builder** and **Documents builder** are placeholders, still to be filled in

### `Web_component.md`

Fifteen frontend sources for components, motion and 3D: reactbits, Aceternity UI, Magic UI, Kokonut UI, 21st.dev, threeui, Spline, GSAP effects, Manus, and more.

### `img/`

- `background/` — wallpapers sized for 1440p displays
- `pokimons/` — transparent mascot art, intended as fastfetch / terminal logos

---

## Command sheet (`codes.md`)

Quick reference for git identity, drive formatting, package installs and Windows BitLocker.

> ⚠️ **`mkfs.btrfs -f` erases the target device.** Verify the device name with `lsblk` first — the sheet writes it as `lsdk`, which is a typo. The BitLocker command is PowerShell, not a Linux shell.

---

## Notes

- This is a personal configuration repo, not a packaged project — expect machine-specific paths and app choices.
- Nothing is automated: there is no install script, so every file is applied by hand.
- Snippets are kept as Markdown so they render with syntax highlighting on GitHub and can be read without cloning.
