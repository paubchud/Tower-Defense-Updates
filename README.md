# Tower Defense PVP — Experimental playtests

Playable downloads, update notes and checksums. Unity source and Git history stay private; neither Unity nor source access is needed to play.

## Download and play

Current experimental Windows build: **[0.7.10](https://github.com/paubchud/Tower-Defense-Updates/releases/tag/v0.7.10)**. Download the Windows ZIP under **Assets** and extract the entire archive. GitHub's automatic source archives contain only public instructions/metadata. The latest paired macOS build remains the older [0.7.0 release](https://github.com/paubchud/Tower-Defense-Updates/releases/tag/v0.7.0).

- Windows: open `TowerDefense.exe` for guest play. Steam testing uses `Start-Private-Steam-Test.cmd` or the explicit startup option, with Steam running.
- macOS 0.7.0: open `TowerDefense.app`. Universal Intel/Apple Silicon, macOS 12+, unsigned/unnotarized. It is not compatible with Windows 0.7.10 rooms. If blocked, use the normal per-app macOS approval flow only if you trust the download. Real Mac execution/bot startup still needs testing.
- Choose Play as Guest for EOS internet rooms. Steam development App ID 480 is a separate pool, with no Steam/guest cross-play. All players need matching builds, separate Steam accounts/devices or independent guest identities. For same-machine testing use the local playtest, not duplicate online identities.
- Choose Warrior or Wizard, host a normal room and share its code. **Two humans can both Ready to start.** For four-player free-for-all, have all four join before readying. Three humans wait for a fourth. Empty seats remain empty; running matches reject late joins.
- Friend plus bots on Windows 0.7.10: with two fully joined humans, the host can choose Add 2 Bots; with three, the host can choose Add 1 Bot. Every human personally Readies after the selected bots arrive. Cancel/remove bots stays in the human room, and bot loss returns the room to a clean retry state.
- Solo: Play -> class -> LOCAL PLAYTEST / 3 BOTS -> Ready. This uses three background local clients and does not admit friends or fill internet rooms. Rematch waits for your vote and fresh Ready; Leave closes the bots.
- Keep the host running. Non-host departure resets the remaining lobby; host loss ends the session. Guest rooms are code-selected advertised lobbies. Queues, parties/teams, reconnect grace and host migration remain inactive.

## Controls and gameplay

WASD moves; middle-drag orbits the centered camera; wheel selects Weapon/Army/Quick tower upgrade. Left mouse uses the selected slot. Right-click land, towers and resources to manage them. I opens Equipment, G opens automation upgrades, and Esc opens Settings / Leave Game while the match continues. Settings includes separate player-interface and troop-menu opacity controls plus an option to hide button/key instructions.

Fresh matches and rematches begin with 0 Gold. Castles begin at 20 points and lose one per ordinary arriving troop. Sending costs 1 gold total, delivering one troop to each surviving participating enemy; weapon attacks gather visible wood/stone/iron/gold/diamond reserves to fund opening purchases. Both playable heroes can build the five selected towers and purchase their five stages; undefined WIP effects remain inactive. The main-menu Tower Catalog exposes 25 Primal/Mystic/Sadist/Holy/Fiendish inspection slots, but catalog-only WIP towers cannot be placed. Automation unlocks are per resource type; individual visited mines have separate material costs. See the versioned release notes for exact temporary costs and limits.

Normal hero death gives a timed own-side ghost with management but no attacks, collection or scouting. Castle elimination allows full-map camera viewing with no match actions; enemy wallets and private mining progress stay private. All participating rematch votes return to a fresh ready-up lobby. Progression is match-only; no permanent rewards or paid power are active.

## Feedback and recovery

Report version/platform/provider, host/client role, player count, steps, expected/actual behavior and redacted logs in [Issues](https://github.com/paubchud/Tower-Defense-Updates/issues). Never post credentials or private configuration.

These are experimental builds. The host can access full match authority; real-device internet, Mac execution, balance, long-soak, uncapped GPU and physical-wire checks remain open. Older fixed tags/ZIPs remain for rollback. Public Git contains only instructions, release notes and artifact checksums; playable binaries are Release assets. Each `releases/vVERSION.json` records ZIP sizes and SHA256.
