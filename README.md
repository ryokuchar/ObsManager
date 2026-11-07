# ObsManager

ObsManager manages the OBS Replay Buffer for registered games on Windows 11 x64.

## Get started

1. Extract the entire release folder and run `ObsManager.exe`.
2. In OBS Studio, enable the WebSocket server and Replay Buffer. Enter the server address (usually `ws://127.0.0.1:4455`) and password in ObsManager.
3. Register the game and use the process name of the game itself. Save and restart ObsManager after changing a game's launch or monitoring settings.

Use the generated shortcut or `ObsManager.exe --game <game-id>` to start a registered game.

## Replay Buffer

ObsManager stops only a buffer it started during the current OBS connection, after all registered games have closed and the configured delay has elapsed. Use OBS controls or a hotkey configured in OBS to save replays.

## Update

Exit ObsManager from the system tray before opening the new release. Settings carry over for the same Windows user. Recreate shortcuts that point to the old folder.
