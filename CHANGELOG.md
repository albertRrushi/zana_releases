# Changelog

## 0.5.0

- New Gateway view that automatically sends each new task to the best provider, voice, and helper for the job, with a plain-language explanation of why that choice was made.
- Savings view showing projected cost savings from automatic routing, with totals across all routed tasks.
- Custom routing rules: pin specific kinds of work to a preferred provider, or narrow down the allowed choices, using flexible condition blocks (all / any / none logic, nested groups) that can skip questions already answered.
- Gateway test area to try routing rules and preview the chosen provider and reasoning before running a real task.
- Optional automatic decision helper behind Gateway routing that can be switched on or off; pinned rules keep working even when it is off.
- Per-provider reasoning strength control, available in settings, the assistant, new-task setup, and automatic routing.
- Claude Agent improvements: live model and helper lists with display names, a refresh button, a single default entry, and follow-up messages that steer the ongoing work directly in both task and assistant views.
- Smoother dictation and voice: microphone recording moved off the main thread for reliability, voice features now grouped behind one opt-in switch, listening and dictation buttons appear only when their feature is enabled.
- Clearer task flow: the Run button shows only for brand-new tasks and the first message starts the task; the Done list shows the last 2 days with older items behind a switch.
- API Server view: call history is now a terminal-style log with request and response previews, capped for size.

## 0.4.0

- New live progress for connected apps and integrations: you can now watch a running task as it happens, with text appearing as it's generated and a clear signal when the task finishes. Checking on a finished task works just as before, returning its saved details.
- Smoother follow-ups with Claude Agent tasks: messages you send while a task is still working now feed straight into the ongoing work, instead of piling up and arriving late.
- More reliable background work with Claude Agent tasks: tasks that kick off things in the background no longer fail or mix up their replies because of it.
- Security upkeep: updated core components to clear all reported vulnerabilities.

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
