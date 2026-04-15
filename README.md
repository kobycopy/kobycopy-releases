# KobyCopy Releases

Public installer downloads for [KobyCopy](https://kobycopy.com), the desktop copywriting assistant.

This repo hosts only compiled installers as release assets. The source code lives in a private repository.

## Latest: v0.1.0

- **macOS (Apple Silicon, M1+)** — `CopyWriter_0.1.0_aarch64.dmg`
- **macOS (Intel)** — `CopyWriter_0.1.0_x64.dmg`
- **Windows (x64)** — `CopyWriter_0.1.0_x64-setup.exe`

Download from the [Releases page](https://github.com/kobycopy/kobycopy-releases/releases).

## For maintainers: publishing a release

1. Build installers into this repo's working directory (`.dmg`, `.exe` files are gitignored so they won't accidentally be committed).
2. Create and push a tag:
   ```
   git tag v0.1.0
   git push origin v0.1.0
   ```
3. On GitHub, go to **Releases → Draft a new release**, pick the tag, and drag the installer files in as assets.
4. Publish. Download URLs follow the pattern:
   ```
   https://github.com/kobycopy/kobycopy-releases/releases/download/v0.1.0/CopyWriter_0.1.0_aarch64.dmg
   ```
