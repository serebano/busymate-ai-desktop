# Changelog

All notable changes to the Busymate AI desktop app are documented here. Versions follow
`<version> (build <build>)` as shown in the app's About panel.

## 0.2.2 (build 5) — 2026-09-11

- Apple sign-in now completes fully in-window — the shell's navigation allowlist admits our own sign-in host (api.busymate.net) and Apple's (appleid.apple.com).
- Google sign-in opens in your default browser (Google refuses to run inside any embedded app window, by Google's own policy) and hands the finished session back to the app automatically.

**Download:** [`v0.2.2-build5`](https://github.com/serebano/busymate-ai-desktop/releases/tag/v0.2.2-build5)

## 0.2.2 (build 4) — 2026-09-11

- Menubar menu opens on left-click as well as right-click.

**Download:** [`v0.2.2-build4`](https://github.com/serebano/busymate-ai-desktop/releases/tag/v0.2.2-build4)

## 0.2.2 (build 3) — 2026-09-11

- Fixed in-app Apple sign-in — the sign-in flow now completes inside the app window instead of
  bouncing out to the system browser
- Consolidated to a single menu bar icon
- Fixed a titlebar gap that appeared in fullscreen
- Simplified the About panel to name, version, build date, and busymate.ai
- Added the brand boot/splash card shown on launch
- Signed with a Developer ID and notarized by Apple — installs with no Gatekeeper warning

**Download:** [`v0.2.2-build3`](https://github.com/serebano/busymate-ai-desktop/releases/tag/v0.2.2-build3)
