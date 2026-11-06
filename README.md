# Aneris

Aneris is an AI-powered desktop companion that brings AI assistance, voice interaction, and screenshot-based
context into one lightweight Windows overlay — helping you stay productive without constantly switching
between tools.

This repository ships the **built app only**. The source code is kept private; releases are published here.

## Requirements

- Windows 10 (version 2004 or newer) or Windows 11, 64-bit
- [Claude Code](https://claude.com/claude-code) installed and signed in (`claude` once, then `/login`),
  and/or the Codex CLI signed in with `codex login` — Aneris answers through your own account, no API key
- About 70 MB free for the one-time local speech-recognition download

## Install

1. Go to the [Releases page](../../releases) and download the latest `Aneris_x64-setup.exe`.
2. Run it. Windows SmartScreen may warn "Windows protected your PC" because the installer isn't
   code-signed — click **More info**, then **Run anyway**.
3. Start **Aneris** from the Start menu. A tray icon near the clock (click the `^` arrow if it's hidden)
   confirms it's running — there's no taskbar button.

Aneris checks for new versions automatically and can update itself in place; you won't need to
re-download the installer for future releases.

## Using Aneris

| Keys | Action |
|---|---|
| Ctrl+Shift+L | Manual listening: start recording, press again to stop and send |
| Ctrl+Shift+Space | Add a screenshot to the tray (nothing sends until you ask a question) |
| Ctrl+Shift+H | Show or hide the window |
| Ctrl+Shift+K | Turn click-through on or off |
| Ctrl+Shift+C | Start a new chat |

- **Listening:** pick **Manual** (you control when it records) or **Automatic** (sends once the other
  person stops talking) from the panel above the question box.
- **Model:** choose Haiku, Sonnet, or Opus at any time next to the send button.
- **Interview mode:** the header's Interview button sets up role, company, resume, answer length and
  style once, then every answer follows it until you end the interview.
- **Chats:** every conversation is saved with its own memory; reopen or delete past chats from the
  history panel.
- **Settings:** audio sources, speech accuracy, answer format and length, your own answer rules, and more.

## Privacy

- Aneris's window is excluded from screen capture and recording (Windows' own
  `WDA_EXCLUDEFROMCAPTURE`), so it doesn't appear in Zoom, Teams, Discord, or OBS screen shares. This
  does not hide it from a camera pointed at your screen, a second person in the room, or OS-level
  monitoring software with elevated access — follow the rules of any meeting, interview, or exam you're
  in.
- Audio and speech recognition run entirely on your PC; nothing is sent anywhere except what you
  explicitly ask the AI.

## Support

This is a built-release repository; please open an [issue](../../issues) for bugs or requests.
