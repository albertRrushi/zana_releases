# Changelog

## 0.3.0

- New Voice view: offline text-to-speech reads assistant replies aloud through a Listen button under each reply; voices download on demand and work fully offline afterwards.
- Optional auto-read: when enabled in Voice defaults, the last reply is read aloud automatically when a task you are viewing finishes, and when the assistant chat finishes responding. Background completions stay silent.
- Voice defaults (voice, speed, speaker, auto-read) are edited locally with explicit Save/Reset buttons.
- New Dictation section in the Voice view: offline speech-to-text with downloadable engine and models; includes a test pad with live transcription and copy.
- Mic button in chat inputs and the Add Task dialog: dictation transcribes live as you speak and inserts the text at the cursor; pausing auto-sends the message when auto-send is enabled, otherwise you press send yourself.
- Auto-send for dictation is a Voice-view setting (on by default); recordings are transcribed on the fly and never stored.

## 0.2.8

- Fixed OpenCode failing to start automatically on Windows after reboot.

## 0.2.3

- Removed Antigravity as a provider option.
- Replaced the per-project delete button with a settings gear that spins on hover; it opens a Project settings popup showing the project name as read-only, with deletion moved into a confirming Danger zone.
- Project settings now allow renaming the alias, and memory distillation plus permission auto-approval can each follow the global Settings or be overridden per project — leaving override off follows the global value including future changes, while turning it on reveals the per-project choice.
- The Add Project dialog offers the same follow-global-or-override choices at creation time.
- Toned the settings gear to a muted color that turns primary on hover.

## 0.2.0

- Migrates the OpenCode provider to OpenCode 2.0-only (`@opencode/client` 2.x, shared service model). OpenCode 1.x is no longer supported — users must have OpenCode CLI 2.0+ installed.
