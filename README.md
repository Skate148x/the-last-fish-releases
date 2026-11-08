# The Last Fish — Blackwater Reservoir

Windows preview downloads and update metadata. Game source is maintained separately; this is a release distribution repository.

## First updater test

1. Close the old desktop game.
2. Install **0.4.23-beta.1**, choosing the suggested **C:\Games\The Last Fish** folder (or another dedicated folder named The Last Fish).
3. Launch with the new desktop shortcut. Existing progress is read from the same save folder.
4. The game checks for a newer preview shortly after launch. Download the **newest preview**, then pause and choose **Save & restart to update**.
5. Confirm that the game restarts, **Alt → Game → Check for updates** reports the new preview version, and your fish, money, upgrades, and settings are still present.

Updates never install during normal play or automatically on ordinary quit. The restart is blocked if the current shift cannot be saved. Offline update checks do not prevent playing.

## Imported-save preservation check

Preview **0.4.23-beta.3** is a version-only test update. On beta 2, import your browser save, note your money, fish remaining, backpack, upgrades and settings, then update through the game. Do not re-import afterward: confirm the existing desktop save loads unchanged.

## Display mode (beta 4 and later)

Open **Settings → Graphics & display → Display mode** to choose Fullscreen or Windowed. F11 and Alt+Enter switch the same saved setting. New installations default to fullscreen; later launches remember the chosen mode. Windowed size, position, and maximized state are retained, with recovery onto an available monitor if the old monitor is disconnected. Minimized state is never restored. Display preferences are separate from fishing saves and survive game updates and browser-save imports.

## Desktop controls — Playtest Build 005

The main menu has an **Exit game** button beside Settings. To leave a live shift, use **Save & return to title**, then **Exit game**. Failed live-shift saves block leaving, and title-screen exit preserves the stored player location.

Escape is routed through the desktop app so a second press can resume mouse-look without clicking the water. Pause still releases the cursor. This also applies when returning from Settings; native Windows capture behavior needs player verification.

Player-facing labels now use **Playtest Build 005, 006, …** for small updates. Internal semver and prerelease tags are retained for compatibility with existing updaters; those tags do not represent game-development milestones.

## Saves

Saves and rolling backups remain in `%APPDATA%\TheLastFish\Saves`, separately from the game files. **Alt → Game → Open save backups** opens this folder. Exporting a backup before the first update test is recommended.

The initial 0.4.22 LocalAppData game files are left intact as a fallback when moving to C:. Use the new shortcut; do not run the old folder's uninstaller after moving, because it can remove the new shortcuts. Do not manually move the installed EXE out of its folder.

## Preview status

These are unsigned Windows x64 previews. Windows may show an unknown-publisher notice. Automated tests cover game saves, update state transitions, and save-before-restart behavior; Windows installation and restart behavior still require player testing. Downloads are checked against their SHA-512 release metadata, which is not a publisher certificate. No Steam integration is included yet.

To install directly without testing the update path, use the newest beta installer from Releases.
