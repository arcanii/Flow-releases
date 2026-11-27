<p align="center">
  <img src="images/icon.png" width="128" height="128" alt="The Flow icon: a terminal prompt over swirling liquid">
</p>

<h1 align="center">Flow</h1>

<p align="center"><i>A terminal for macOS, Windows and Linux with a liquid-glass look, old machines' themes, pictures and 3D in the terminal, and an AI assistant built in.</i></p>

<p align="center">
  <img src="images/badges/assistant.svg" alt="Assistant: Claude, GPT or Gemini">
  <img src="images/badges/pictures.svg" alt="Pictures: kitty, Sixel and iTerm2">
  <img src="images/badges/3d.svg" alt="3D models: glTF and OBJ">
  <img src="images/badges/mcp.svg" alt="MCP: the assistant uses servers, and outside apps use Flow">
  <img src="images/badges/rust.svg" alt="Written in Rust, drawn with wgpu">
  <img src="images/badges/languages.svg" alt="English and Japanese">
  <img src="images/badges/updates.svg" alt="Signed updates">
</p>

<p align="center">
  <a href="https://github.com/arcanii/Flow-releases/releases/tag/v0.1.48-macos"><b>Download for macOS</b></a> ·
  <a href="https://github.com/arcanii/Flow-releases/releases/latest"><b>Download for Windows</b></a> ·
  <a href="https://github.com/arcanii/Flow-releases/releases/tag/v0.1.48-linux"><b>Download for Linux</b></a> ·
  <a href="https://github.com/arcanii/Flow-Terminal"><b>Source</b></a>
</p>

---

Type commands as usual, or tell the assistant in plain English what you want
done: it suggests the steps or runs them in your own shell, where you can
watch, and asks before anything risky. It's Anthropic's Claude, OpenAI's GPT
or Google's Gemini, whichever you prefer, and Flow works as a terminal without
any of them.

Flow runs the shells you already have: zsh and bash on the Mac and Linux;
cmd, PowerShell, Git Bash, MSYS2 and WSL on Windows, where Flow also brings
BusyBox, a small POSIX shell with the usual Unix tools, for those who have
none of those. Behind the text is a live
fluid your typing stirs, and programs can draw pictures and 3D models in the
terminal that ride the liquid like the letters around them.

![Flow with the assistant panel open](images/main.png)

## Why Flow

The terminal is where you tell a computer what to do. Flow is built to
make it the best place on your computer to be: a window of live liquid
glass, an assistant that does the work beside you while you watch, and
the same terminal on Windows, macOS and Linux.

**Do you want a taste of [Omarchy](https://omarchy.org) without switching
everything over yet?** Omarchy, DHH's "beautiful, fun & agentic" Linux,
puts the keyboard, the terminal, good looks and AI agents at the heart of
the computer. Flow brings that way of working to the Windows, Mac or
Linux you already have, as one app:
- a theme for the whole window, chosen in one place;
- [split panes](#tabs-panes-and-finding-your-way), tiled and moved
  between with the keys;
- a [command palette](#tabs-panes-and-finding-your-way) that reaches
  everything;
- a [hotkey](#and-more) that drops Flow down over whatever you're doing;
- every key yours to change, in **Settings → Keys**;
- an assistant in the window;
- [`flowapp`](#apps-with-flowapp), which installs terminal tools written
  again for Flow: `ls`, `tree`, `top`, `btop` and `du`, with pictures,
  bars and graphs.

When you're ready for the real thing, your habits come with you.

**Do you want AI to help manage your PC, so you don't have to?** Say what
you want in plain words: *"why is my disk full?"*, *"update everything
Homebrew installed"*, or *"what's listening on port 8080? stop it"*.
Flow's [assistant](#the-assistant) works it out and runs it in your real
shell, where you see every command. It uses Claude, GPT or Gemini, with
your own key.
- **Guide mode:** it waits for your yes at each step.
- **Auto mode:** it goes ahead by itself, but still asks before anything
  risky: deleting, `sudo`, registry edits, or files that look like
  secrets.
- **When a command fails,** Flow offers **✦ Ask why**.
- **It remembers** what it learned and where a task got to, and carries
  on after a restart.
- **It can work on its own** for the time and tokens you give it.
- **`/undo`** puts back the files a task changed.
- **[MCP servers](#mcp-both-ways)** let it reach your other tools.

**Do you want the nostalgia of the computers of yesteryear?** Put on one
of ten old machines' [themes](#themes) and a tab becomes that machine:
- an 8-bit home computer on a television;
- a minicomputer's green or amber screen;
- a teletype typing its start screen at 300 baud;
- a British school's page of teletext;
- an eighties PC counting its memory as it starts;
- a workstation whose PROM probes your own computer's memory banks and
  buses;
- a 16-bit home computer that asks for its disk before its ball spins.

Each comes with its own fonts, start screen and prompt, and a
[CRT](#crt): curved glass, scanlines and a phosphor that lingers. Each
makes its own sounds: the tube's hum, the PC's fan, the teletype's clack
and bell, the floppy drive's seek. Every tab, and every pane of a split,
can wear a different one.

**Do you want to turn your boring terminal into something exciting?**
Flow's glass is a [live fluid](#liquid-glass) that your cursor and typing
stir. Pick clouds with lightning, water seen from above or below, glossy
oil, or rain on a window that beads, runs and flashes with thunder in a
storm. The glass reacts:
- a finished command splashes;
- a build's progress fills the glass like a tank;
- the liquid leans toward the assistant while it thinks;
- programs can ask for bolts and bursts of their own.

Programs show [pictures and moving 3D models](#pictures-and-3d-models)
right in the terminal (pictures in kitty's, iTerm2's and sixel formats),
and the [games](#apps-with-flowapp) made for Flow install with one
command. To share what you did, [record it](#and-more) as an animated
WebP.

**Do you want a terminal that does the everyday things well, and works
much the same on Windows, macOS and Linux?**
- **[Full-text search](#tabs-panes-and-finding-your-way)** of every
  command you've run, in every shell, cmd included. Type any words in any
  order, or any three letters, and see the folder each one ran in and how
  it ended.
- **Different shells in tabs:**
  - on Windows, cmd, PowerShell and bash (Git Bash, MSYS2, WSL, or the
    BusyBox that comes with Flow);
  - on the Mac and Linux, zsh and bash.

  Any tab splits into panes.
- **One Flow on all three systems,** as far as each one allows: the same
  features, settings and config file, with `Ctrl+Shift` where the Mac
  has `⌘`.
- **Find in the scrollback,** with patterns if you like, and jumps from
  command to command.
- **The small things:**
  - links you can click;
  - a click that moves the cursor along the line you're typing;
  - a [notification](#and-more) when a long command finishes behind
    other windows;
  - tabs that come back as you left them.

**And more:**
- **Safe by default.** Flow works as a terminal with no account and no
  key.
  - A key you add stays in the system's own credential store.
  - Secrets are kept out of the command history and the assistant's
    memory.
  - Outside apps get in only when you let them.
  - [Updates are signed](#download) on every system, and Flow refuses
    any that aren't.
- **Light when it needs to be.** **🌱e-mode** turns the show off in one
  click, and can turn it off by itself on battery.
- **Open to everyone.** VoiceOver, Narrator and Orca read Flow's tabs,
  panes, assistant and Settings. Its words come in English and Japanese.
- **Yours to build on.**
  - Programs reach Flow with escape codes and
    [its SDK](https://github.com/arcanii/Flow-SDK) for C and Python, and
    change its settings with `flow-settings`.
  - Themes and skills come as [packages](#apps-with-flowapp).
  - [Outside apps](#mcp-both-ways) such as Claude Code, Claude Desktop
    and Cursor can use your tabs through MCP, as far as you allow.
- **Native.** Flow is written in Rust and drawn on the GPU: an app of
  each system's own, not a web page in a window.

## Quick start

**TL;DR:** install it, open it, and use it as your terminal. Everything else
is there when you want it.

1. **Install.**
   - **macOS** (Apple silicon, macOS 11 or later): open the `.dmg` and drag
     Flow to Applications.
   - **Windows** (10 or 11, x64): run `Flow-<version>-setup.exe`. Windows
     may say it protected your PC: choose **More info → Run anyway**.
   - **Linux** (x86-64, glibc 2.31 or newer): `sudo apt install
     ./Flow-<version>-linux-amd64.deb`, or unpack the tarball and run its
     `install.sh`, which needs no root.

   Each installed Flow updates itself. [Download](#download) has the details.
2. **Open a tab.** Flow starts in your usual shell. **⌘T** (**Ctrl+Shift+T**)
   opens another, and the **…** beside **+** picks its shell and theme.
   **⌘D** (**Ctrl+Shift+D**) splits the tab in two.
3. **Make it yours.** **⌘,** (**Ctrl+,**) opens Settings: the liquid style, an
   old machine's theme, the font, the colors and the CRT. Changes show as you
   make them.
4. **Ask the assistant** (optional). In **Settings → Assistant**, pick Claude,
   GPT or Gemini and add that provider's API key. Then press **⌃Space**
   (**Ctrl+Space**) and ask, say, *"show me what's using the most disk
   space"*.
5. **Get the apps.** In any Flow tab, `flowapp install flow-rogue` installs a
   game, and `flowapp search` lists the rest. See [Apps](#apps-with-flowapp).
6. **Lost?** **⇧⌘P** (**Ctrl+Shift+P**) opens the command palette, which finds
   every command, setting and theme by typing. **F1** shows help for the screen
   in front, and `flow-help` prints it in a tab.

| | macOS | Windows and Linux |
| --- | --- | --- |
| Settings | `⌘,` | `Ctrl+,` |
| The assistant | `⌃Space` | `Ctrl+Space` |
| New tab, close tab | `⌘T`, `⌘W` | `Ctrl+Shift+T`, `Ctrl+Shift+W` |
| Split side by side, one above the other | `⌘D`, `⇧⌘D` | `Ctrl+Shift+D`, `Ctrl+Shift+Alt+D` |
| Command palette | `⇧⌘P` | `Ctrl+Shift+P` |
| Find in the scrollback | `⌘F` | `Ctrl+Shift+F` |
| Command history | `⌘R` | `Ctrl+Shift+R` |
| Record the terminal | `⇧⌘R` | `Ctrl+Shift+Alt+R` (Linux: `Ctrl+Shift+Alt+V`) |
| Help | `F1`, `⌘?` | `F1`, `Ctrl+Shift+?` |

## Apps with `flowapp`

`flowapp` comes with Flow, on the path of every Flow tab, and installs Flow's
apps the way Homebrew installs formulae. Flow itself carries none of them, so
you take only what you want:

| App | What it is |
| --- | --- |
| `flow-rogue` | **Flow Rogue**, a roguelike with a town, the wilds, lairs and a dungeon to go down, drawn in animated sprites |
| `flow-mines` | **Flow Mines**, the mine-finding puzzle, drawn over Flow's liquid |
| `flow-invaders` | **Flow Invaders**, ships coming down in waves in 3D, fought from a truck with a shop between the waves |
| `flow-utils` | **Flow-Utils**, `ls`, `tree`, `man`, `top`, `btop`, `du`, `df` and more written again for Flow, with pictures, bars and graphs in its tabs |
| `flow-phonebook` | **Flow Phonebook**, `dial` to call a BBS over SSH, its pictures, models and sounds reaching your tab |
| `flow-sdk` | **Flow's SDK** for C and Python, with `flow-demo` and its demos |
| `flow-core-themes` | **Flow's machines** as a package of themes, kept up to date |

```sh
flowapp search              # the apps there are
flowapp install flow-rogue  # install one, then run it: flow-rogue
flowapp list                # what you have, and its versions
flowapp upgrade             # update everything you have
flowapp remove flow-rogue   # take one off (your saves stay)
```

**Settings → Apps** does the same with buttons, and can check for newer
versions for you. Every download is checked against the catalog's size and
checksum and Flow's own signature before anything is put in place.

`flowapp` is in the catalog too, so a newer one can come out between Flow's
releases: `flowapp upgrade` offers it, and from then on Flow's tabs run it in
place of the one your Flow carries (`flowapp remove flowapp` goes back to
that one).

What `flowapp` installs comes after your system's own commands, so Flow-Utils'
`ls` never replaces the system's unasked. `flowapp first flow-utils` puts its
programs first in Flow's tabs, and `flowapp last flow-utils` puts the system's
back. `flowapp --help` lists everything it does.

<table>
  <tr>
    <td><img src="images/rogue-town.png" alt="Flow Rogue's town: three shops, a well, and roads west to the dungeon and east to the castle"></td>
    <td><img src="images/rogue-castle.png" alt="A warrior facing a skeleton, a ghost, a vampire and a zombie in the castle, over the Clouds style"></td>
  </tr>
  <tr>
    <td>Flow Rogue's town: the shops, the well, and the roads out</td>
    <td>In the castle, over the <b>Clouds</b> style. The ghost is see-through.</td>
  </tr>
</table>

### Checking a download yourself

Every app's download here is signed with Flow's own Ed25519 key, and
`flowapp` checks each one before it puts anything in place. You can check
one yourself with OpenSSL 3 or later. `flow-update.pem`, in this
repository, is Flow's key, and its fingerprint is:

```
f1866b49b0b42871463772bf1c9d77fae2091c32dc01681ae5d752f13008b4d0
```

```sh
curl -LO https://raw.githubusercontent.com/arcanii/Flow-releases/main/flow-update.pem
openssl pkey -pubin -in flow-update.pem -outform DER | openssl dgst -sha256   # the fingerprint above
curl -LO https://github.com/arcanii/Flow-releases/releases/download/flow-say-v0.1.1/flow-say-0.1.1-macos-aarch64.tar.gz
curl -LO https://github.com/arcanii/Flow-releases/releases/download/flow-say-v0.1.1/flow-say-0.1.1-macos-aarch64.tar.gz.sig
openssl pkeyutl -verify -pubin -inkey flow-update.pem -rawin -in flow-say-0.1.1-macos-aarch64.tar.gz -sigfile flow-say-0.1.1-macos-aarch64.tar.gz.sig
```

For a download Flow signed, the last line says "Signature Verified
Successfully". Each download's signature is beside it on its release as
`<file>.sig`, and in `apps.json` as base64, with the date it was signed.

The Mac's own `/usr/bin/openssl` is LibreSSL, which can't read an Ed25519
key: use Homebrew's (`brew install openssl`). On Windows, use Git Bash's.

## What's in it

### The assistant

Say what you want done, and the assistant works in the tab in front. In
**guide** mode it suggests each command for you to run, edit or skip; in
**auto** mode it runs them itself and stops to ask before anything risky: a
high-risk command, overwriting a file, or touching a sensitive one. When a command of yours
fails, **Ask why** offers to explain it. It sees your system, the shell, the
folder and the last 40 lines of the terminal, so mind what's on screen if it
shows secrets. Each provider's key is kept in the macOS Keychain, Windows
Credential Manager, or on Linux the Secret Service, and a token cap in
Settings stops it at a total you choose.

### MCP, both ways

<table>
  <tr>
    <td><img src="images/mcp-call.png" alt="The assistant calling a notes app's MCP server, its next call waiting for a yes"></td>
    <td><img src="images/settings-mcp-servers.png" alt="Settings' MCP servers"></td>
  </tr>
  <tr>
    <td>The assistant using a notes app's MCP server, asking before a call</td>
    <td><b>Settings → MCP servers</b>: each server, and a switch for each tool</td>
  </tr>
  <tr>
    <td><img src="images/mcp-ask-form.png" alt="An MCP server asking a question as a form"></td>
    <td><img src="images/mcp-ask.png" alt="Claude Code asking to use Flow"></td>
  </tr>
  <tr>
    <td>A server asking you something, as a form of its own</td>
    <td>An outside app asking to use Flow, the first time</td>
  </tr>
</table>

**The assistant uses your MCP servers:** a notes app, an issue tracker, a
database, whatever you already use with Claude Desktop or Claude Code. Add
them in Settings, or paste in their config as those apps write it. A server
is a program Flow starts, or a remote one, which Flow signs in to through
your browser. Nothing runs until you connect a server, each of its tools
stays off until you turn it on, and each call asks first unless you allow
it. The assistant can read a server's resources, you can run its prompts
from the panel (`/<server>:<prompt>`), a server can ask you something on a
card of its own, and the assistant's journal keeps every call.

**Outside apps use Flow:** turn on **Settings → Outside apps**, and Claude
Code, Claude Desktop or Cursor can use Flow through `flow-mcp`, which comes
with it: read your tabs, open tabs and panes, change Flow's settings, and
run commands in panes of their own. Each app is asked the first time what it
may do, commands can ask each time (a risky one always does), and Flow
listens only where you alone can reach it, never on the network.

### Tabs, panes and finding your way

<table>
  <tr>
    <td><img src="images/split.png" alt="A tab split in two, its new pane in the green screen's theme"></td>
    <td><img src="images/palette.png" alt="The command palette"></td>
  </tr>
  <tr>
    <td>A split tab, each pane in a theme of its own</td>
    <td>The command palette: every command, setting and theme</td>
  </tr>
  <tr>
    <td><img src="images/history.png" alt="The command history's search"></td>
    <td><img src="images/find.png" alt="Find in the scrollback"></td>
  </tr>
  <tr>
    <td>The command history, found by any words</td>
    <td>Find in the scrollback, words or a pattern</td>
  </tr>
</table>

Each tab runs the shell you pick, in a theme of its own if you like, and
splits into panes that each keep their own. Flow keeps the commands you run,
whatever the shell, with the folder each ran in and how it ended, and finds
them again by any words in them. It reopens your tabs where you left them,
and links that programs write, or plain addresses in the text, open with a
⌘-click (Ctrl+click).

### Pictures and 3D models

<table>
  <tr>
    <td><img src="images/images-clouds.png" alt="A screenshot shown with timg in Flow, over the Clouds style"></td>
    <td><img src="images/images-crt.png" alt="The same picture under the CRT"></td>
  </tr>
  <tr>
    <td>A picture from <code>timg</code>, over the <b>Clouds</b> style</td>
    <td>The same picture under the <b>CRT</b>: scanlines, curve and glow</td>
  </tr>
</table>

Programs can show pictures in the terminal through the kitty graphics
protocol (`viu`, `timg -pk`, `kitten icat`, yazi), Sixel (`chafa`,
`img2sixel`) and iTerm2's inline images (`imgcat`): PNG, JPEG, GIF, WebP,
BMP and TIFF, and animations play. A picture sits in the terminal like text:
it scrolls, goes into the scrollback and clears, rides the liquid, and glows
under the CRT. On Windows, the console layer between Flow and the shell
drops kitty's escapes, so tools that speak Sixel or iTerm2's protocol show
pictures there, and Flow's own apps send theirs down a pipe Flow opens for
each tab.

![A 3D model in Flow](images/model.png)

3D models come through the [Ratty graphics
protocol](https://docs.rs/crate/ratty/0.4.1/source/protocols/graphics.md):
OBJ and glTF (`.glb`), lit with their materials and textures, still, turning
or animated, and clickable where a program asks. A model sits in the terminal
as a picture does. If a program asks Flow to read one from a file, Flow asks
you first.

### Themes

<table>
  <tr>
    <td><img src="images/theme-home.webp" alt="Flow as an 8-bit home computer on a television"></td>
    <td><img src="images/theme-green.png" alt="Flow as a minicomputer's green screen"></td>
  </tr>
  <tr>
    <td>The <b>Home computer</b></td>
    <td>The <b>Green screen</b>, every color a shade of its phosphor</td>
  </tr>
  <tr>
    <td><img src="images/theme-instruments.webp" alt="Flow as the Flow Instruments Home Computer"></td>
    <td><img src="images/theme-amiga.webp" alt="Flow as the Flow notanAmiga CLI, in its window frame"></td>
  </tr>
  <tr>
    <td>The <b>Flow Instruments Home Computer</b></td>
    <td>The <b>Flow notanAmiga CLI</b>, framed as its window was</td>
  </tr>
</table>

**Settings → Theme** dresses Flow as an old machine: an 8-bit home computer
on a television, two workstations booting as their PROMs did, a
minicomputer's green screen, an amber screen, a teletype, a British school's
micro in teletext, an eighties PC, an early-eighties home computer and a
16-bit home computer's shell. Each new tab types out the machine's start
screen at the speed of its line and takes its prompt, in the font of its
time, and with **Machines' sounds** on each sounds like itself: a tube's
hum, a teletype's carriage, a disk drive, a fan. The green and amber screens
show everything as a monochrome monitor did, white as the phosphor at full.
**Your own** theme takes a start screen and prompt you type, **Save as
theme…** keeps what you've made under a name, and the **Theme gallery**
previews and installs more.

### Liquid glass

The glass is a live fluid simulation, and your cursor and typing stir it up.
Pick a style in Settings, and slow it down if you like:

<table>
  <tr>
    <td><img src="images/clouds.webp" alt="Clouds with lightning"></td>
    <td><img src="images/water-above.webp" alt="Water seen from above"></td>
  </tr>
  <tr>
    <td><b>Clouds</b>, with lightning if you like</td>
    <td><b>Water from above</b>: ripples, sunlight and caustics</td>
  </tr>
  <tr>
    <td><img src="images/water-below.webp" alt="Water seen from below"></td>
    <td><img src="images/oil.webp" alt="Oil"></td>
  </tr>
  <tr>
    <td><b>Water from below</b>: light shafts and bubbles</td>
    <td><b>Oil</b>: a glossy, thin-film sheen</td>
  </tr>
  <tr>
    <td><img src="images/rain.webp" alt="Rain on the window"></td>
    <td><img src="images/none.webp" alt="Plain glass"></td>
  </tr>
  <tr>
    <td><b>Rain</b> on a fogged window, from a drizzle to a storm, your cursor wiping the glass</td>
    <td><b>None</b>: plain tinted glass</td>
  </tr>
</table>

The glass also shows what the terminal is up to: a ring spreads when a
command finishes (red if it failed), programs that report progress fill it
like a tank, a tab glows when a long command ends behind it, and programs can
set off lightning, splashes and ripples of their own. **🌱e-mode** in the
title bar stills it all to save power, and Flow can do that by itself on
battery.

### CRT

![Flow with the Arcade CRT preset over the None style, in green](images/crt.webp)

**Settings → CRT** shows everything as an old tube monitor would: scanlines,
interlace, the phosphor's glow and afterglow, the grille, a vignette and the
tube's curve, which clicks and selections follow. Pick a preset (Subtle,
Classic, Arcade, Phosphor or Television) or save your own.

### And more

- **Record the terminal** (**⇧⌘R**) to a looping animated WebP, the liquid
  and the tube in it, to share anywhere that plays one. A countdown comes
  first, and Flow says if your prompt shows your user or computer name.
- **A drop-down terminal:** pick a **Hotkey** in Settings and Flow drops down
  from the top of the screen over whatever you're doing, and away again
  (not on Wayland, which keeps hotkeys to itself).
- **Notifications:** a long command that finishes while you're elsewhere is
  told of by Notification Center, a Windows toast or your Linux desktop.
- **English and Japanese**, Flow's menus, Settings and help alike, with the
  system's input method at the prompt. The assistant answers in your
  language too.
- **Screen readers:** VoiceOver, Narrator and Orca read the terminal,
  Settings and the assistant's panel.
- **For programs:** a program can set off Flow's effects and sounds, change
  its settings (`flow-settings`) and draw pictures and models, from Rust, C
  or Python with [Flow's SDK](https://github.com/arcanii/Flow-SDK).

### More screenshots

<table>
  <tr>
    <td><img src="images/settings.png" alt="The Settings menu"></td>
    <td><img src="images/settings-apps.png" alt="Settings' Apps"></td>
  </tr>
  <tr>
    <td>Settings: the look, the font, the assistant and the rest</td>
    <td><b>Settings → Apps</b>: what <code>flowapp</code> does, with buttons</td>
  </tr>
  <tr>
    <td><img src="images/theme-gallery.png" alt="The Theme gallery"></td>
    <td><img src="images/new-tab.png" alt="The new-tab picker"></td>
  </tr>
  <tr>
    <td>The <b>Theme gallery</b>, previewing a package of themes</td>
    <td>A new tab: its shell and its theme, side by side</td>
  </tr>
  <tr>
    <td><img src="images/key.png" alt="Adding an API key"></td>
    <td><img src="images/about.png" alt="The About card"></td>
  </tr>
  <tr>
    <td>Adding the assistant's API key</td>
    <td>About, with a check for updates</td>
  </tr>
</table>

## Download

### macOS

Get **Flow-&lt;version&gt;-macos.dmg** from the
[macOS release](https://github.com/arcanii/Flow-releases/releases/tag/v0.1.48-macos),
open it, and drag Flow to Applications. It runs on Macs with Apple silicon and
macOS 11 or later.

- Flow for macOS is signed and notarized, so it opens without a warning.
- It updates itself. Flow asks once whether to check automatically, and
  **Flow → Check for Updates…** checks on demand.
- `SHA256SUMS-macos.txt` in each macOS release lists the checksum.

### Windows

Get **Flow-&lt;version&gt;-setup.exe** from the
[latest release](https://github.com/arcanii/Flow-releases/releases/latest) and
run it. It runs on Windows 10 and 11, x64 (and on Arm through Windows' x64
emulation).

- The installer isn't code-signed yet, so SmartScreen may say "Windows
  protected your PC". Choose **More info → Run anyway**.
- Installed copies update themselves. Flow asks once whether to check
  automatically, and **About → Check for Updates…** checks on demand.
- Prefer not to install? Use the portable zip. Portable copies don't update
  themselves.
- `SHA256SUMS.txt` in each release lists the files' checksums.

### Linux

From the [Linux release](https://github.com/arcanii/Flow-releases/releases/tag/v0.1.48-linux),
for x86-64 Linux with glibc 2.31 or newer (Ubuntu 20.04, Debian 11 and
everything since), on Wayland or X11, with a Vulkan driver:

- **Ubuntu, Debian and others with apt:** get
  **Flow-&lt;version&gt;-linux-amd64.deb** and run
  `sudo apt install ./Flow-<version>-linux-amd64.deb`. `sudo apt remove
  flow-terminal` takes it away. Flow updates itself through apt: **About →
  Install Update** downloads and checks the new .deb, then runs apt in a tab
  of its own, where you type your password, and offers to restart.
- **Any Linux, no root needed:** get **Flow-&lt;version&gt;-linux-x86_64.tar.gz**,
  unpack it and run `./flow-<version>/install.sh`, which puts Flow in
  `~/.local` and in your applications (`--uninstall` takes it away). Installed
  this way, Flow installs its own updates.
- Flow asks once whether to check for updates daily, and **About → Check for
  Updates…** checks on demand.
- Each file's `.sha256` beside it has its checksum.

Every update Flow installs, on every system, carries an Ed25519 signature
that Flow checks before using it, and it refuses any that doesn't verify.

## What this repo holds

- The [releases](https://github.com/arcanii/Flow-releases/releases): Flow's
  Windows installers and portable zips (with the source of the BusyBox they
  bundle, free software under the GPL, version 2), its macOS disk images in
  the releases tagged `-macos`, and its Linux tarballs and .debs in those
  tagged `-linux`; and each app's downloads, in releases tagged
  `<app>-v<version>`.
- `appcast.xml`, `appcast-macos.xml` and `appcast-linux-x86_64.xml`, the
  update feeds that installed copies of Flow read on Windows, macOS and
  Linux, and `apps.json`, the catalog `flowapp` reads.

Something not right? Please [open an
issue](https://github.com/arcanii/Flow-Terminal/issues), or report a
security hole privately through its **Security** tab.

Flow is open source: its source is at
[arcanii/Flow-Terminal](https://github.com/arcanii/Flow-Terminal), under the
MIT License. Flow's name, icon and startup logo aren't covered by that
license ([Flow's brand
license](https://github.com/arcanii/Flow-Terminal/blob/master/docs/brand/LICENSE-brand.txt)).

<sub>Intel, AMD, Sun Microsystems and its emblem, SGI and its cube, Amiga and
its Boing Ball (with Kickstart, Workbench and Topaz), Apple and Windows are
trademarks of their respective owners. Flow shows their logos only as a
historical showcase of the computers of their time, and is not related to
them or endorsed by them. Ultima V is a trademark of Electronic Arts; Flow
Rogue carries none of its tiles.</sub>
