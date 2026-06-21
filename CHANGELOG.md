# Changelog

## 0.2.1 — 2026-06-21

- Added `setup/setup.sh` (first-run bootstrap): installs the marketplace update-notifier hook and auto-installs the Python deps (`pyperclip`, `playwright`) for the GPT-Pro web bridge. repomix still runs via `npx -y` (no preinstall); browser CDP launch + ChatGPT login stay in the command's interactive onboarding (Step 0.5).
- GitHub star is now opt-in via AskUserQuestion (네 / 아니요): asked once and recorded (`~/.gptaku-setup/insane-review.star.json`), never re-asked. The prompt is shown in the user's current language — falling back to the language detected from recent Claude sessions (else English) when there's no signal yet. No auto-star.

## 0.2.0

- GPT-5.5 Pro (web-only) bridge: repomix pack → subscription ChatGPT Pro via CDP → review retrieval. Standalone reviewer + agent-council web member.
