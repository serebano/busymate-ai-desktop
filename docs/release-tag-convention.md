# Release tag convention

This repository is the release host for the Busymate AI desktop app. Automated publish pipelines
targeting this repo should follow this convention so releases stay consistent and discoverable.

## Tag format

```
v<version>-build<build>
```

Examples: `v0.2.2-build3`, `v0.2.3-build1`.

- `<version>` is the app's semantic version, as shown in the About panel (e.g. `0.2.2`).
- `<build>` is the integer build number for that version (e.g. `3`), also from the About panel.

## Release title

```
Busymate AI <version> (build <build>)
```

Example: `Busymate AI 0.2.2 (build 3)`.

## Release notes

The body of the GitHub Release should mirror the corresponding entry in
[`CHANGELOG.md`](../CHANGELOG.md), plus the SHA-256 checksum of the attached DMG.

## Assets

Each release should attach the signed, notarized, universal (Apple Silicon + Intel) `.dmg` for
macOS. As Windows/Linux builds become available, attach their signed installers to the same
release using clear per-platform filenames.

## What a future auto-publish pipeline should do, per build

1. Build, sign, and notarize the app (as already happens today).
2. Create a GitHub Release in **this repo** (`serebano/busymate-ai-desktop`) tagged
   `v<version>-build<build>`, titled `Busymate AI <version> (build <build>)`, with notes drawn
   from the changelog entry for that build and the DMG's SHA-256.
3. Attach the signed DMG (and future Windows/Linux installers) as release assets.
4. Update [`CHANGELOG.md`](../CHANGELOG.md) in this repo with the new entry (same content as the
   release notes).
5. Point `busymate.ai/desktop`'s "latest release" data at this GitHub Release (via the API or a
   generated manifest) so the download page and the in-app updater manifest both reflect the same
   build, and include a **"Report an issue"** link on `busymate.ai/desktop` back to
   [this repo's issue tracker](https://github.com/serebano/busymate-ai-desktop/issues).

This repo does not contain the app's source — only release artifacts, issues, and docs — so the
pipeline only needs `gh release create` (or the equivalent REST/GraphQL calls) against this repo,
not a source push.
