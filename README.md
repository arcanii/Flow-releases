<p align="center">
  <img src="images/icon.png" width="128" height="128" alt="The Flow icon: a terminal prompt over swirling liquid">
</p>

<h1 align="center">Flow</h1>

<p align="center">
  A terminal for Windows and macOS with a liquid-glass look and an AI assistant built in.<br>
  <a href="https://github.com/arcanii/Flow-releases/releases/latest"><b>Download for Windows</b></a> ·
  <a href="https://github.com/arcanii/Flow-releases/releases/tag/v0.1.10-macos"><b>Download for macOS</b></a>
</p>

Type commands as usual, or describe what you want in plain English. The
assistant suggests the steps or runs them in your shell, and asks first before
anything risky. It's Anthropic's Claude, OpenAI's GPT or Google's Gemini,
whichever you prefer.

Flow runs the shells you already have. On Windows that's cmd, PowerShell and
bash; if you don't have Git Bash, MSYS2 or WSL, Flow brings its own bash:
BusyBox, a small POSIX shell with the usual Unix tools. On the Mac it's zsh and
bash, with a menu bar, a right-click menu and the keys you're used to from
Terminal.

![Flow with the assistant panel open](images/main.png)

## Tabs

One window holds as many terminals as you like, each in a tab running the shell
you pick. **⌘T** (**Ctrl+Shift+T** on Windows) opens a tab with your default
shell, in the folder of the tab in front, and the **+** after the tabs opens one
with any other shell. **⌘W** (**Ctrl+Shift+W**) closes a tab, **⌘1** to **⌘9**
(**Ctrl+Shift+1** to **9**) jump to one, and **⇧⌘]** and **⇧⌘[** (**Ctrl+Tab**
and **Ctrl+Shift+Tab**) step through them. The assistant works in the tab in
front.

Tabs came to the Mac in Flow 0.1.7 and to Windows in 0.1.8.

## Liquid glass

The glass is a live fluid simulation, and your cursor and typing stir it up.
Pick a style in Settings, and slow it down if you like:

<table>
  <tr>
    <td><img src="images/clouds.webp" alt="Clouds with lightning"></td>
    <td><img src="images/water-above.webp" alt="Water seen from above"></td>
  </tr>
  <tr>
    <td><b>Clouds</b>, with optional lightning</td>
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
    <td><b>Rain</b> on a fogged window: drops run down and grow, and your cursor wipes the glass</td>
    <td><b>None</b>: plain tinted glass with nothing moving behind it</td>
  </tr>
</table>

In Settings you can also pick the terminal's font from the monospaced fonts on
your computer. Since 0.1.8, **Text color** and **Cursor color**
offer a row of swatches (any other color works as `#RRGGBB` in the config
file), and **Glow** turns the glow around the cursor, tabs and buttons down to
nothing or up to 200%.

On the Mac, since 0.1.9, each color also shows as its `#RRGGBB` value, which
opens a color picker: drag for saturation and brightness, pick the hue on a
bar, or type or paste a hex value. A third color, **Background**, tints the
glass behind the terminal under any liquid style.

## The glass reacts

Whatever the style, the glass also shows what your terminal is up to:

- **Commands:** when one finishes, a ring spreads from the prompt (red if it
  failed, wider after a long run), and the liquid splashes in its own way, with
  bursts of cloud, ripples, bubbles or running drops.
- **Progress:** programs that report how far along they are, such as Cargo,
  fill the glass from the bottom like a tank.
- **The assistant:** while it thinks, the liquid leans toward its panel. Each
  step it takes splashes, and a finished task blooms.
- **Tabs:** when a long command finishes in a tab you aren't looking at, that
  tab glows green, or red if the command failed.

Prefer a calm window? Turn off **Reactions** in Settings. The reactions came to
the Mac in Flow 0.1.7 and to Windows in 0.1.8.

## Download

### Windows

Get **Flow-&lt;version&gt;-setup.exe** from the
[latest release](https://github.com/arcanii/Flow-releases/releases/latest) and run it.

- The installer isn't code-signed yet, so SmartScreen may say "Windows
  protected your PC". Choose **More info → Run anyway**.
- Installed copies update themselves. Flow asks once whether to check
  automatically, and **About → Check for Updates…** checks on demand.
- Prefer not to install? Use the portable zip. Portable copies don't update
  themselves.
- `SHA256SUMS.txt` in each release lists the files' checksums.

### macOS

Get **Flow-&lt;version&gt;-macos.dmg** from the
[macOS release](https://github.com/arcanii/Flow-releases/releases/tag/v0.1.10-macos),
open it, and drag Flow to Applications. It runs on Macs with Apple silicon and
macOS 11 or later.

- Flow for macOS is signed and notarized, so it opens without a warning.
- It updates itself. Flow asks once whether to check automatically, and
  **Flow → Check for Updates…** checks on demand.
- `SHA256SUMS-macos.txt` in each macOS release lists the checksum.

## The assistant

The assistant needs an API key from its provider. Flow works as a terminal
without one and never asks for it on its own. Open Settings (`Ctrl+,`, or `⌘,`
on the Mac), pick the **Provider** under Assistant (Claude, GPT or Gemini), and
add that provider's key under **API key**. Each provider keeps its own key, in
Windows Credential Manager or the macOS Keychain. GPT and Gemini are new in
Flow, so expect some rough edges.

![Adding an API key](images/key.png)

## More screenshots

<table>
  <tr>
    <td><img src="images/settings.png" alt="The settings menu"></td>
    <td><img src="images/about.png" alt="The About dialog"></td>
  </tr>
  <tr>
    <td>Settings: the look, the font, the assistant and its provider, a token cap</td>
    <td>About, with a check for updates</td>
  </tr>
</table>

## What this repo holds

- The [releases](https://github.com/arcanii/Flow-releases/releases): the Windows
  installers, and the macOS disk images in the releases tagged `-macos`. Since
  0.1.1, each Windows release also carries the source of the BusyBox it
  bundles, which is free software under the GPL, version 2.
- `appcast.xml` and `appcast-macos.xml`, the update feeds that installed copies
  of Flow read on Windows and on macOS. Every update in them carries an EdDSA
  signature, and Flow refuses updates that don't verify.

Flow's source code isn't public yet, but I do plan to make it OpenSource when more mature.
This is also testing a release repo.
