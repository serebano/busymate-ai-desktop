# Changelog

All notable changes to the Busymate AI desktop app are documented here. Versions follow
`<version> (build <build>)` as shown in the app's About panel.

## 1.1.0 (build 11) — 2026-09-24

- Sign-in links from your browser now open the app reliably, even when the link is what launches it: a link that arrives while the app is starting, reloading or offline is no longer lost.
- The app now declares the 14 languages the Console speaks, so macOS lists it under each of them.
- The app also registers its own link address, ai.busymate.console://, beside busymate-ai://.

**Download:** [`v1.1.0-build11`](https://github.com/serebano/busymate-ai-desktop/releases/tag/v1.1.0-build11)

## 0.2.7 (build 10) — 2026-09-13

- Automatic updates on launch and every few hours; Check for Updates… with a native dialog; the minimal About panel; one menu-bar icon.

**Download:** [`v0.2.7-build10`](https://github.com/serebano/busymate-ai-desktop/releases/tag/v0.2.7-build10)

## 0.2.6 (build 9) — 2026-09-13

- Maintenance release: the same app as 0.2.5, published so the automatic updater has a newer build to install — this release is the live proof of Check for Updates › Install & relaunch.

**Download:** [`v0.2.6-build9`](https://github.com/serebano/busymate-ai-desktop/releases/tag/v0.2.6-build9)

## 0.2.5 (build 8) — 2026-09-13

- Update prompts now appear. "Check for Updates…" shows a native dialog with what changed and an Install & relaunch button — or tells you you're up to date.
- Automatic updates on launch and every few hours, one click to install.
- A cleaner About panel — name, version and build, build date, and a link to busymate.ai.

**Download:** [`v0.2.5-build8`](https://github.com/serebano/busymate-ai-desktop/releases/tag/v0.2.5-build8)

## 0.2.4 (build 7) — 2026-09-13

- Automatic updates. Busymate AI checks for a newer build on launch and every few hours, and installs it with one click — no reinstalling from the website.
- A cleaner About panel — just the name, the version and build, the build date, and a link to busymate.ai.
- One menu-bar icon, and a signed-out launch that lands on the sign-in screen.

**Download:** [`v0.2.4-build7`](https://github.com/serebano/busymate-ai-desktop/releases/tag/v0.2.4-build7)

## 0.2.3 (build 6) — 2026-09-12

- Automatic updates. Busymate AI now checks for a newer build on launch and every few hours, and installs it with one click — no reinstalling from the website.
- Signed-out launch fix. Opening the app while signed out now lands on the sign-in screen instead of an error page.
- One menu-bar icon. The menu bar shows a single Busymate AI icon.
- A cleaner About panel — name, version, build date, and a link to busymate.ai.

**Download:** [`v0.2.3-build6`](https://github.com/serebano/busymate-ai-desktop/releases/tag/v0.2.3-build6)

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
