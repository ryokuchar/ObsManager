# ObsManager

ObsManager is a Windows 11 x64 tray app that manages the OBS Studio Replay Buffer for registered games. You can enable Replay Buffer integration per game and launch games from custom shortcuts.

## Download

Open **Releases** and download `ObsManager-v1.0.0-win-x64.zip` from **Assets**. Extract the entire ZIP and run `ObsManager.exe` from the extracted folder. The required .NET and Windows App SDK runtimes are bundled. Install OBS Studio separately.

This build is unsigned, so Windows SmartScreen may display a warning. The first public release does not support migrating settings from development builds.

## Set up

1. On first launch, choose a display language and review the distribution terms.
2. In OBS Studio, enable the WebSocket server and Replay Buffer. Enter the server address (usually `ws://127.0.0.1:4455`) and password in ObsManager.
3. Register a game's launch target and the process name of the game itself. Save and restart ObsManager after adding a game or changing its launch or monitoring settings.
4. Start the game from its generated shortcut or run `ObsManager.exe --game <game-id>`.

## How the Replay Buffer works

When a game with integration enabled starts, ObsManager starts the Replay Buffer if needed. It only stops a buffer it started during the current OBS connection. The stop delay begins once **all registered games** have closed, including those with integration disabled. To save a replay, use OBS Studio or a hotkey configured in OBS.

## License

ObsManager itself is licensed under MIT (Copyright © 2026 ryokuchar). Official builds are free to download. The source code is not published. Bundled components retain their own licenses. See `DISTRIBUTION-TERMS.txt` and `THIRD-PARTY-NOTICES.txt` in the release.
