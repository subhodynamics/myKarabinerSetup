# Keyboard remapping note

Here is a summary of the shortcuts defined in my **Karabiner configuration** :

-------------------------------------------------------------------------------------------------------------------------------------------

### Hyper Key (⌃⌥⇧⌘) Mapping

If using windows, for hyper key use [**ctrl + alt + shift + windows key**]

1. **Caps Lock** is remapped to the **Hyper Key** (⌃⌥⇧⌘) by default, and if pressed alone, it triggers the **Escape** key.

---

### Hyper Key Sub-Layers and Actions:

- **Hyper + spacebar** : Backspace and delete (continuous until held)

### **o** (Open Applications):

- **Hyper + o + 1**: Open 1Password.
- **Hyper + o + g**: Open Google Chrome.
- **Hyper + o + c**: Open Visual Studio Code.
- **Hyper + o + v**: Open Zed.
- **Hyper + o + d**: Open Discord.
- **Hyper + o + s**: Open Slack.
- **Hyper + o + e**: Open Superhuman.
- **Hyper + o + n**: Open Notion.
- **Hyper + o + t**: Open Terminal.
- **Hyper + o + h**: Open Hypersonic Todo List in Notion.
- **Hyper + o + z**: Open Zoom.
- **Hyper + o + m**: Open Reflect.
- **Hyper + o + r**: Open Reflect.
- **Hyper + o + f**: Open Finder.
- **Hyper + o + i**: Open Texts (for iMessage).
- **Hyper + o + p**: Open Spotify.
- **Hyper + o + a**: Open iA Presenter.
- **Hyper + o + w**: Open WhatsApp (replaced by Texts).
- **Hyper + o + l**: Open Raycast Shortlink.

### **w** (Window Management using Rectangle.app):

- **Hyper + w + ;**: Hide the window (⌘ + h).
- **Hyper + w + y**: Move window to the previous display.
- **Hyper + w + o**: Move window to the next display.
- **Hyper + w + k**: Move window to the top half.
- **Hyper + w + j**: Move window to the bottom half.
- **Hyper + w + h**: Move window to the left half.
- **Hyper + w + l**: Move window to the right half.
- **Hyper + w + f**: Maximize the window.
- **Hyper + w + u**: Switch to the previous tab (Control + Shift + Tab).
- **Hyper + w + i**: Switch to the next tab (Control + Tab).
- **Hyper + w + n**: Switch to the next window (⌘ + `).
- **Hyper + w + b**: Go back in the window (⌘ + [).
- **Hyper + w + m**: Go forward in the window (⌘ + ]).

### **s** (System Controls):

- **Hyper + s + u**: Increase volume.
- **Hyper + s + j**: Decrease volume.
- **Hyper + s + i**: Increase display brightness.
- **Hyper + s + k**: Decrease display brightness.
- **Hyper + s + l**: Lock the screen (⌃⌘Q).
- **Hyper + s + p**: Play/Pause media.
- **Hyper + s + ;**: Fast forward media.
- **Hyper + s + e**: Toggle Elgato Key Light (via Raycast).
- **Hyper + s + d**: Toggle Do Not Disturb (via Raycast).
- **Hyper + s + t**: Toggle system appearance (Light/Dark Mode).
- **Hyper + s + c**: Open camera (via Raycast).
- **Hyper + s + v**: Voice input (Option + Spacebar).

### **v** (Vim-like Navigation):

- **Hyper + v + h**: Move cursor left.
- **Hyper + v + j**: Move cursor down.
- **Hyper + v + k**: Move cursor up.
- **Hyper + v + l**: Move cursor right.
- **Hyper + v + m**: Trigger Magicmove (Control + f).
- **Hyper + v + s**: Scroll mode (Control + j).
- **Hyper + v + d**: Move (Shift + Command + d).
- **Hyper + v + u**: Page down.
- **Hyper + v + i**: Page up.

### **c** (Music Controls):

- **Hyper + c + p**: Play/Pause music.
- **Hyper + c + n**: Skip to next track.
- **Hyper + c + b**: Rewind to the previous track.

### **r** (Raycast Actions):

- **Hyper + r + c**: Pick color via Raycast.
- **Hyper + r + n**: Dismiss notifications via Raycast.
- **Hyper + r + l**: Create MXSB shortlink.
- **Hyper + r + e**: Search Emoji Symbols.
- **Hyper + r + p**: Show Raycast confetti.
- **Hyper + r + a**: Open Raycast AI chat.
- **Hyper + r + s**: Trigger Silent Mention.
- **Hyper + r + h**: Open Raycast clipboard history.
- **Hyper + r + 1**: Connect favorite Bluetooth device 1.
- **Hyper + r + 2**: Connect favorite Bluetooth device 2.


"**Swapped Left Option and Left Command**"

- ----------------------------------------------------------------------------------------------------------------------------------------------------------


## Installation

1. Install & start [Karabiner Elements](https://karabiner-elements.pqrs.org/)
1. Clone this repository
1. Delete the default `~/.config/karabiner` folder
1. Create a symlink with `ln -s ~/github/mxstbr/karabiner ~/.config` (where `~/github/mxstbr/karabiner` is your local path to where you cloned the repository)
1. [Restart karabiner_console_user_server](https://karabiner-elements.pqrs.org/docs/manual/misc/configuration-file-path/) with `` launchctl kickstart -k gui/`id -u`/org.pqrs.karabiner.karabiner_console_user_server ``

## Development

```
yarn install
```

to install the dependencies. (one-time only)

```
yarn run build
```

builds the `karabiner.json` from the `rules.ts`.

```
yarn run watch
```

watches the TypeScript files and rebuilds whenever they change.
