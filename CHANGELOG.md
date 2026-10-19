# Changelog

## 0.2.3

- Removed Antigravity as a provider option.
- Replaced the per-project delete button with a settings gear that spins on hover; it opens a Project settings popup showing the project name as read-only, with deletion moved into a confirming Danger zone.
- Project settings now allow renaming the alias, and memory distillation plus permission auto-approval can each follow the global Settings or be overridden per project — leaving override off follows the global value including future changes, while turning it on reveals the per-project choice.
- The Add Project dialog offers the same follow-global-or-override choices at creation time.
- Toned the settings gear to a muted color that turns primary on hover.

## 0.2.0

- Migrates the OpenCode provider to OpenCode 2.0-only (`@opencode/client` 2.x, shared service model). OpenCode 1.x is no longer supported — users must have OpenCode CLI 2.0+ installed.
