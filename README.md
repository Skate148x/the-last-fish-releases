# The Last Fish — Blackwater Reservoir

Windows preview downloads and update metadata. Game source is maintained separately; this is a release distribution repository.

## First updater test

1. Close the old desktop game.
2. Install **0.4.23-beta.1**, choosing the suggested **C:\Games\The Last Fish** folder (or another dedicated folder named The Last Fish).
3. Launch with the new desktop shortcut. Existing progress is read from the same save folder.
4. The game checks for a newer preview shortly after launch. Download **beta 2**, then pause and choose **Save & restart to update**.
5. Confirm that the game restarts, **Alt → Game → Check for updates** reports beta 2, and your fish, money, upgrades, and settings are still present.

Updates never install during normal play or automatically on ordinary quit. The restart is blocked if the current shift cannot be saved. Offline update checks do not prevent playing.

## Saves

Saves and rolling backups remain in `%APPDATA%\TheLastFish\Saves`, separately from the game files. **Alt → Game → Open save backups** opens this folder. Exporting a backup before the first update test is recommended.

The initial 0.4.22 LocalAppData game files are left intact as a fallback when moving to C:. Use the new shortcut; do not run the old folder's uninstaller after moving, because it can remove the new shortcuts. Do not manually move the installed EXE out of its folder.

## Preview status

These are unsigned Windows x64 previews. Windows may show an unknown-publisher notice. Automated tests cover game saves, update state transitions, and save-before-restart behavior; Windows installation and restart behavior still require player testing. Downloads are checked against their SHA-512 release metadata, which is not a publisher certificate. No Steam integration is included yet.

To install directly without testing the update path, use the newest beta installer from Releases.
