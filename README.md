# Tower Defense multiplayer playtests

This repository contains playable downloads, update notes and checksums. **The Unity source and its Git history are not included.** You do not need Unity or access to the source repository to play.

## Download and play

Current experimental build: **[0.6.1](https://github.com/paubchud/Tower-Defense-Updates/releases/tag/v0.6.1)**. Open **Assets**, download the Windows or macOS ZIP, and extract the entire archive. Do not download GitHub's automatic "Source code" archives: those contain only this repository's instructions and release metadata, not the game.

- Windows: open `TowerDefense.exe` for guest play. Steam testing uses `Start-Private-Steam-Test.cmd`, or the explicit startup option, with Steam already running.
- macOS: open `TowerDefense.app`. The Universal build targets Intel and Apple Silicon/macOS12+. It is unsigned/unnotarized and may be blocked by macOS. Approve only this app through macOS's normal per-app security flow if you trust the download; do not disable system security. A real Mac playtest is still required.
- Choose **Play as Guest** for EOS guest internet play without an Epic/Steam sign-in screen. Steam's explicit development App ID480 is also available. These are separate player pools, with no cross-play.
- For this update, **four matching-version players** select Warrior or Wizard. One hosts a room and shares its code with three friends; all four click Ready. Use separate accounts/devices for Steam and independent device identities for EOS guests. Two guests under one OS account can share an identity; use LAN/This PC for same-machine testing instead.
- Keep the host running. Guest rooms are code-selected advertised lobbies, not password-protected private rooms. Current non-host departure resets the remaining lobby; host loss ends the session. Random queues, parties/teams, reconnect grace and host migration are not active yet.

## Current prototype

1v1v1v1 on a blocky four-sector map. Send costs1gold total for one troop per surviving enemy castle; castles start at30points and lose1 per arrival. Defend, mine grey rocks for stone, buy plots/build towers, invade visible enemy nodes and fight living heroes. Hero-only Player XP and separate level points use temporary test values. Other wiki content remains planned; synergies/In-game Upgrades and non-rock resource mechanics are inactive.

WASD moves; right-drag orbits the hero-centered camera; wheel selects the hotbar. Left mouse attacks, E/pickaxe mines, T sends, U upgrades future troops, B manages land/towers, I shows equipment, G opens the inactive upgrade tab. Ghosts cannot attack, mine or scout. All four rematch votes return to fresh ready-up.

## Feedback and recovery

Report version, platform, provider, host/client role, reproduction steps and relevant Player.log excerpts in [Issues](https://github.com/paubchud/Tower-Defense-Updates/issues). Never post account credentials or private configuration. Test builds are experimental; real four-device internet play, balance, Mac execution and long-soak performance remain open gates.

Older published version tags and ZIPs stay fixed for rollback. Each `releases/vVERSION.json` lists the complete ZIP sizes and SHA256 checksums. This public repository holds **only instructions, release notes and checksums** in Git; game binaries are attached under Releases, not committed into its file history.
