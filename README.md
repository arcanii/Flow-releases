# Flow

Flow is a terminal for Windows with a liquid-glass look and Claude built in.
Type commands as usual, or describe what you want in plain English. The
assistant suggests the steps or runs them in your shell, and asks first before
anything risky.

## Download

Get **Flow-&lt;version&gt;-setup.exe** from the
[latest release](https://github.com/arcanii/Flow-releases/releases/latest) and run it.

- The installer isn't code-signed yet, so SmartScreen may say "Windows
  protected your PC". Choose **More info → Run anyway**.
- Installed copies update themselves. Flow asks once whether to check
  automatically, and **About → Check for Updates…** checks on demand.
- Prefer not to install? Use the portable zip. Portable copies don't update
  themselves.
- `SHA256SUMS.txt` in each release lists the files' checksums.

The assistant needs an Anthropic API key. Flow asks for it on first start and
keeps it in Windows Credential Manager.

## What this repo holds

- The [releases](https://github.com/arcanii/Flow-releases/releases) with the
  installers.
- `appcast.xml`, the update feed that installed copies of Flow read. Every
  update in it carries an EdDSA signature, and Flow refuses updates that don't
  verify.

Flow's source code isn't public.
