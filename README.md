<p align="center">
  <img src="images/icon.png" width="128" height="128" alt="The Flow icon: a terminal prompt over swirling liquid">
</p>

<h1 align="center">Flow</h1>

<p align="center">
  A terminal for Windows and macOS with a liquid-glass look and Claude built in.<br>
  <a href="https://github.com/arcanii/Flow-releases/releases/latest"><b>Download for Windows</b></a> ·
  <a href="https://github.com/arcanii/Flow-releases/releases/tag/v0.1.4-macos"><b>Download for macOS</b></a>
</p>

Type commands as usual, or describe what you want in plain English. The
assistant suggests the steps or runs them in your shell, and asks first before
anything risky.

On Windows, cmd, PowerShell and bash each get a tab. If you don't have Git
Bash, MSYS2 or WSL, Flow brings its own bash: BusyBox, a small POSIX shell with
the usual Unix tools. On the Mac, zsh and bash do, with a menu bar, a
right-click menu and the keys you're used to from Terminal.

![Flow with the assistant panel open](images/main.png)

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
</table>

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
[macOS release](https://github.com/arcanii/Flow-releases/releases/tag/v0.1.4-macos),
open it, and drag Flow to Applications. It runs on Macs with Apple silicon and
macOS 11 or later.

- Flow for macOS is signed and notarized, so it opens without a warning.
- It updates itself. Flow asks once whether to check automatically, and
  **Flow → Check for Updates…** checks on demand.
- `SHA256SUMS-macos.txt` in each macOS release lists the checksum.

The assistant needs an Anthropic API key. Flow asks for it on first start and
keeps it in Windows Credential Manager or the macOS Keychain.

![The first-run dialog that asks for an Anthropic API key](images/key.png)

## More screenshots

<table>
  <tr>
    <td><img src="images/settings.png" alt="The settings menu"></td>
    <td><img src="images/about.png" alt="The About dialog"></td>
  </tr>
  <tr>
    <td>Settings: the look, the assistant, a token cap</td>
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
