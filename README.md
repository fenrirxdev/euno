<p align="center">
  <img src="images/icon.png" width="128" height="128" alt="euno">
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="images/euno-en-dark.gif">
    <img src="images/euno-en-light.gif" width="720" alt="Typing /euno cx in Claude reads Codex's review and carries on">
  </picture>
</p>

# euno

[日本語](README.ja.md) · [Product page](https://euno.fenrirx.dev/)

euno is a macOS menu bar app that bridges chats in Claude, Codex and Cursor, so an AI can read the conversation in the chat on the other side when it needs to.

This repository is where euno is distributed and where bugs are reported. The source code is not public.

euno is an unofficial app made by an individual developer. It is not affiliated with Anthropic, OpenAI or Anysphere.

## Requirements

- macOS 15 (Sequoia) or later
- A Mac with Apple silicon
- At least two of these apps:
  - Claude (Code mode in the desktop app, or Claude Code)
  - Codex
  - Cursor
- To register the MCP server, euno uses each app's CLI for Claude and Codex (`claude`, `codex`). To install the skill, it uses `npx` (Node).

## Install

1. [Download euno.dmg](https://github.com/fenrirxdev/euno/releases/latest/download/euno.dmg).
2. Open the DMG and drag euno to the Applications folder.
3. Open euno from the Applications folder.

euno cannot register its MCP server while it runs from inside the DMG. Move it to the Applications folder before opening it.

## First run

1. **Allow Accessibility.** euno uses the Accessibility permission to tell which chat each app is showing, and to notice a double tap of the right ⌘ key. It never reads or records which keys you press.
2. **Register the apps.** In euno's settings, under Integrations, register the MCP server and the skill for each app you use. Chats started before registering cannot use euno, so start a new chat afterwards. Codex also needs to be restarted.
3. **Make a bridge.** Double-tap the right ⌘ key to open the panel, and pick the chats to bridge.

Inside a chat, `/euno` in Claude and Cursor, or `$euno` in Codex, brings in the chat on the other side.

## Updates

euno can check for new versions automatically. It asks whether to on the second launch, and you can change this later in settings. To check by hand, open Settings → General → Check for Updates.

## Privacy

- euno reads the chat history each app stores on your Mac, read-only. It never changes that history.
- It reads only the chats you bridged.
- Your bridges, and a record of which AI read which chat, are kept in `~/Library/Application Support/euno`.
- euno connects to the network to check for and download updates, and to install or update the skill. It does not send message text, read records, or usage data to external services.

See [Privacy](PRIVACY.md#privacy) for what euno reads, writes, and sends. When you ask AI to name a bridge, euno passes chat titles and repository names to the CLI you choose.

## Uninstall

1. In euno's settings, under Integrations, unregister the MCP server and uninstall the skill for each app. For Cursor, delete the `euno` entry from `~/.cursor/mcp.json`.
2. Quit euno and delete it from the Applications folder.
3. To remove its settings and records too, delete `~/Library/Application Support/euno`.

## Reporting bugs

Report bugs in [Issues](https://github.com/fenrirxdev/euno/issues/new/choose). Issues are public, so do not include conversation text, names or tokens.

Report a Problem… in euno's menu opens an issue form with version, permission, and integration information filled in. It contains no message text. Check the contents before submitting.

## Compatibility

The apps may change how they store chat history without notice, and euno may then be unable to read conversations. euno is currently in beta. Changes and limitations are listed in each release's notes.

## License

Copyright © 2026 fenrirxdev. All rights reserved.
