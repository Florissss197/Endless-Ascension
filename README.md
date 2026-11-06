[README.md](https://github.com/user-attachments/files/34497027/README.md)
# Endless Ascension — Setup Guide

Endless Ascension is a community-made mod project for **Sanctum 2**, by **UltimateWeener**.

> **This is a development preview, not a stable release.** The installer was checked against an isolated copy, but gameplay and LAN co-op have not been runtime-tested. Share the preview only through a **private GitHub repository** with people who own Sanctum 2.

## What is included?

- A Windows launcher with **Install & Launch**, **Launch Installed**, and **Uninstall** buttons.
- One fixed Challenge profile: enemy count ×1 and resilience ×1.
- Verification of required Sanctum 2 files before installation.
- Backup and restore support for the game file changed by the installer.

This preview does not include configurable Sandbox mode or the in-game shop.

## Set up GitHub

1. Create a **private repository** on GitHub.
2. Upload the contents of the `Repository` folder to the repository root. Upload the files inside `Repository`, not just the folder itself.
3. Open **Releases** and select **Create a new release**.
4. Set the tag and release name to `0.2.0-dev.1`.
5. Attach `EndlessAscension-Dev-0.2CI-Preview.zip` from `GitHub-Release-Assets` to the release.
6. Publish the release in the private repository and invite your friend to the repository.

Keep the preview ZIP private: it contains a modified Sanctum 2 game package. Do not upload it to a public repository or public release.

## Install and launch

Each player must do these steps on their own Windows PC:

1. Install Sanctum 2 through Steam, then close the game.
2. Download `EndlessAscension-Dev-0.2CI-Preview.zip` from the GitHub Release.
3. Extract the entire ZIP to a normal folder. Do not run the EXE from the ZIP preview.
4. Open `EndlessAscensionLauncher.exe`.
5. Select your own Sanctum 2 installation folder, the one containing `Binaries` and `SanctumGame`.
6. Click **INSTALL & LAUNCH** and accept the development-preview notice.

The installer checks that the game files match the required base version. If the check fails, it stops without changing the file. Do not use a different or manually modified game build.

## Uninstall

1. Close Sanctum 2 completely.
2. Open `EndlessAscensionLauncher.exe` again.
3. Click **UNINSTALL**.

The uninstaller restores the backup created during installation. Do not delete that backup before uninstalling the mod.

## Co-op / LAN

Every player needs their own Sanctum 2 installation and must install the same release. This preview has not been tested on two PCs, so LAN/co-op is not guaranteed.

## Troubleshooting

- **The launcher cannot find the game:** browse to the folder containing `Binaries` and `SanctumGame`.
- **Base-file verification fails:** verify Sanctum 2 files through Steam and retry with the unmodified required game version.
- **The game is running:** close Sanctum 2 before installing or uninstalling.
- **Installation fails:** use **UNINSTALL** if available, then check the launcher log in `SanctumGame\Logs` inside the selected game folder.

## Repository contents

- `EndlessAscension-installer/` — installer, checker, uninstaller, and release builder.
- `EndlessAscensionLauncher.cs` — Windows launcher source.
- `Build-Launcher.cmd` — Windows build script for the launcher.
- `Project-Preview.html` — project overview and roadmap.

