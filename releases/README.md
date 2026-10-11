# Releases

How GhostGirl Softmod releases work.

---

## What Goes in a Release

Each release attaches one asset:

| Asset | Purpose |
|---|---|
| `GhostGirlRepack.zip` | The softmod package |

The zip contains the folder `GhostGirlRepack` with all the softmod files inside.

---

## Why the Softmod Is a Release Asset

The softmod contains binary files (`.xex`, payloads, etc.) that
would bloat the repo.

- ✅ Keeps the repo small
- ✅ GitHub Releases has dedicated storage
- ✅ Users download from one place
- ✅ Each release is versioned and immutable

**Don't commit softmod files to the repo.** Always attach them to a release.

---

## Release Workflow

1. Assemble the `GhostGirlRepack` folder locally.
2. Test on real hardware (Trinity + Corona, ABadUpdate + ABadAvatar).
3. Zip it: `zip -r GhostGirlRepack.zip GhostGirlRepack/`
4. Go to **Releases** → **Draft a new release**.
5. Tag it (e.g. `v1.3.9`).
6. Title it `GhostGirlRepack v1.3.9`.
7. Attach `GhostGirlRepack.zip`.
8. Write release notes (see template below).
9. Publish.

---

## Release Notes Template

```markdown
# 👻 GhostGirlRepack v1.3.9

## ⚠️ READ THE INSTALLATION GUIDE FIRST

Before you do anything else, read the full installation guide.

📖 → docs/INSTALL.md

The softmod will NOT work if you skip the setup steps.

## 📥 Download

**Asset:** `GhostGirlRepack.zip`

Extract it, then look for the folder named `GhostGirlRepack`.
Copy the files INSIDE it — not the folder itself — to the root of a
FAT32 USB stick.

## ✨ What's New in v1.3.9

- Early access release
- ABadUpdate support
- ABadAvatar support
- Install guide included in the folder
- Stability improvements
- Minor bug fixes

## ⚠️ Permanent Softmod Warning

Permanent softmod is **NOT recommended** at the moment.
Use the temporary USB method for now.

## 🚀 Quick Start

1. Download and extract `GhostGirlRepack.zip`
2. Open the `GhostGirlRepack` folder
3. Copy the files INSIDE to the root of a FAT32 USB stick
4. Turn off Wi-Fi and Auto Sign-In on your console
5. Power off, wait 30 seconds, insert USB into the port nearest the power button
6. Wait 5 seconds, then power on
7. Sign in to the `abadavatar` profile

Full guide → docs/INSTALL.md

## 📋 Requirements

- Jailbreakable Xbox 360
- USB stick formatted to FAT32
- A PC to prepare the USB stick

## 🔗 Links

- [Project Ghost Girl](https://github.com/Ghost-Girl-Jailbreak/Project-Ghost-Girl)
- [Discord](https://discord.gg/2YFyMqP6Te)
```

---

## Version Naming

| Release Type | Tag Example |
|---|---|
| Bug fix only | `v1.3.10` |
| New feature | `v1.4.0` |
| Breaking change | `v2.0.0` |

---

## Related

- [docs/INSTALL.md](../docs/INSTALL.md) — install guide
- [docs/FILE_LAYOUT.md](../docs/FILE_LAYOUT.md) — USB structure
- [CHANGELOG.md](../CHANGELOG.md) — changelog
