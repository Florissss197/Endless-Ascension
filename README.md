[Project-Preview.html](https://github.com/user-attachments/files/34497037/Project-Preview.html)
[README.md](https://github.com/user-attachments/files/34497027/README.md)
# Endless Ascension — Setup Guide

Endless Ascension is a community-made mod project for **Sanctum 2**, by **UltimateWeener**.

> **This is a development preview, not a stable release.** The installer was checked against an isolated copy, but gameplay and LAN co-op have not been runtime-tested. Share the preview only through a **private GitHub repository** with people who own Sanctum 2.

## What is included?
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="color-scheme" content="dark">
  <title>Endless Ascension — Project Preview</title>
  <style>
    :root { --bg:#07121b; --panel:#102433; --panel2:#132d3e; --line:#24516a; --text:#e8f3f8; --muted:#aac0cc; --cyan:#42d6ff; --gold:#ffc36b; --green:#7ce0ae; }
    * { box-sizing:border-box; }
    body { margin:0; color:var(--text); background:radial-gradient(ellipse at 75% -20%,#174263 0,transparent 45%),var(--bg); font:16px/1.6 "Segoe UI",Arial,sans-serif; }
    main { width:min(1080px,calc(100% - 36px)); margin:0 auto; padding:54px 0 72px; }
    .eyebrow { color:var(--cyan); font-size:.78rem; font-weight:700; letter-spacing:.2em; text-transform:uppercase; }
    h1 { margin:.35rem 0 .3rem; font-size:clamp(2.2rem,6vw,4.5rem); line-height:1.02; letter-spacing:.035em; }
    .byline { color:var(--muted); margin:0 0 26px; }
    .intro { max-width:800px; color:#d1e4ec; font-size:1.12rem; }
    .status { display:inline-flex; align-items:center; gap:9px; border:1px solid #71542d; background:#30271b; color:#ffd591; border-radius:999px; padding:6px 13px; font-size:.86rem; font-weight:700; }
    .dot { width:8px;height:8px;border-radius:50%;background:var(--gold);box-shadow:0 0 12px var(--gold); }
    section { margin-top:42px; }
    h2 { margin:0 0 14px; font-size:1.42rem; }
    .grid { display:grid; grid-template-columns:repeat(2,minmax(0,1fr)); gap:16px; }
    .card { border:1px solid var(--line); border-radius:14px; padding:22px; background:linear-gradient(145deg,var(--panel2),var(--panel)); box-shadow:0 18px 50px #0003; }
    .card h3 { margin:0 0 8px; color:var(--cyan); font-size:1.15rem; }
    .card p { margin:.45rem 0; color:var(--muted); }
    .tiers { display:grid; grid-template-columns:repeat(4,1fr); gap:8px; margin:16px 0 6px; }
    .tier { padding:10px 7px; text-align:center; border:1px solid #28617b; border-radius:9px; color:#d8f4ff; background:#0a1a25; font-size:.9rem; }
    .tier b { display:block; color:var(--cyan); font-size:1.1rem; }
    ul { margin:8px 0 0; padding-left:20px; color:var(--muted); }
    li { margin:.4rem 0; }
    .roadmap { display:grid; grid-template-columns:repeat(3,minmax(0,1fr)); gap:14px; }
    .roadmap .card { padding:18px; }
    .tag { color:var(--green); text-transform:uppercase; font-size:.72rem; font-weight:700; letter-spacing:.14em; }
    .note { margin-top:22px; border-left:3px solid var(--gold); padding:12px 16px; background:#211d18; color:#eadcc8; }
    footer { margin-top:42px; padding-top:18px; border-top:1px solid var(--line); color:#8fa8b5; font-size:.9rem; }
    @media(max-width:700px){.grid,.roadmap{grid-template-columns:1fr}.tiers{grid-template-columns:repeat(2,1fr)}main{padding-top:34px}}
  </style>
</head>
<body>
<main>
  <div class="eyebrow">A community-made Sanctum 2 mod project</div>
  <h1>ENDLESS<br>ASCENSION</h1>
  <p class="byline">A co-op survival challenge by UltimateWeener</p>
  <span class="status"><span class="dot"></span> Development preview — stability work in progress</span>
  <p class="intro">Endless Ascension turns survival into a replayable, configurable challenge. We are shaping it to feel like a game mode with clear difficulty choices, while keeping a separate sandbox for players who want to tune every detail.</p>

  <section>
    <h2>Two ways to play</h2>
    <div class="grid">
      <article class="card">
        <h3>Challenge Mode</h3>
        <p>Pick readable difficulty grades instead of guessing at a collection of unrelated sliders. Enemy numbers and enemy resilience can be chosen independently.</p>
        <strong>Enemy numbers</strong>
        <div class="tiers"><div class="tier">Standard<b>×1</b></div><div class="tier">Large<b>×2</b></div><div class="tier">Massive<b>×3</b></div><div class="tier">Insane<b>×4</b></div></div>
        <strong>Enemy resilience</strong>
        <div class="tiers"><div class="tier">Standard<b>×1 health</b></div><div class="tier">Tough<b>×2</b></div><div class="tier">Extreme<b>×3</b></div><div class="tier">Insane<b>×4</b></div></div>
        <p>An optional reward setting scales <em>starting resources</em> with the enemy-number grade only. Health difficulty does not grant extra resources. Challenge runs use a mixed, repeating wave set and exclude boss waves.</p>
      </article>
      <article class="card">
        <h3>Sandbox Mode</h3>
        <p>For custom runs, tune each of the 11 repeating wave slots yourself.</p>
        <ul>
          <li>Choose regular enemy types and group sizes</li>
          <li>Set enemy health and movement speed</li>
          <li>Adjust spawn pacing and the alive-enemy cap</li>
          <li>Choose a preset or edit the wave table directly</li>
        </ul>
        <p>The normal build phase remains enabled. Wave 1 and later build timers are separate settings.</p>
      </article>
    </div>
  </section>

  <section>
    <h2>Opening the launcher</h2>
    <div class="card">
      <p>On the development PC, double-click <strong>START-Endless-Ascension.cmd</strong> in the test-game folder. The launcher opens first; choose Challenge or Sandbox, set the options, then click <strong>BUILD LAUNCH</strong>.</p>
      <p>Each player needs their own legitimate Sanctum 2 install. The current launcher still targets this development copy, so a friend-ready installer and portable Steam-game detection are part of the remaining work.</p>
    </div>
  </section>

  <section>
    <h2>What is working toward the preview</h2>
    <div class="roadmap">
      <article class="card"><div class="tag">In the current launcher work</div><ul><li>Challenge and Sandbox paths</li><li>Clear four-step count and resilience grades</li><li>Count-linked starting-resource option</li><li>Loadout choices and base-game build phase</li></ul></article>
      <article class="card"><div class="tag">Being stabilized</div><ul><li>Reliable game startup and wave transitions</li><li>Smoother enemy arrival without spawn pile-ups</li><li>Repeatable balance across the 11-wave cycle</li><li>Safe install and restore behavior for each player</li></ul></article>
      <article class="card"><div class="tag">Planned next</div><ul><li>Single-player playthrough and two-player LAN verification</li><li>Finalize Challenge grade balance and reward values</li><li>Prepare a compact installer, uninstaller, and quick-start guide</li><li>Revisit the in-game upgrade shop after input and purchase fixes</li></ul></article>
    </div>
    <div class="note"><strong>Preview note:</strong> this is not yet a certified stable release. The in-game upgrade shop is intentionally disabled in the share preview until its controls and purchases are reliable. Enemy spawn pacing and LAN behavior still need playtesting before we label a build stable.</div>
  </section>

  <section>
    <h2>What we would love feedback on</h2>
    <div class="card">
      <ul>
        <li>Do the four enemy-number grades feel distinct and easy to understand?</li>
        <li>Are the four resilience grades challenging without making waves drag?</li>
        <li>Does Challenge Mode feel like a designed game mode, with Sandbox clearly separate?</li>
        <li>Which regular enemies or wave patterns make the best co-op moments?</li>
      </ul>
    </div>
  </section>
  <footer>Endless Ascension is a community mod project and requires a legitimate Sanctum 2 installation for each player. This page describes the development direction; it does not promise unverified features.</footer>
</main>
</body>
</html>

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

