# Event lobbies

A plugin for the [Echo VR Launcher](https://github.com/marshmallow-mia/EchoVR_Launcher): play the
event builds (Halloween and Christmas 2017/2018, Summer 2019) together on a classic lobbies server
(EchoRelay).

- **Public matches** on the server, with Join. Who plays in them isn't shown.
- **Your match** and its id, to give to friends.
- **Join by id**, also a private match.
- **Request a game server**: your next Play goes there.
- **Your account** there: the launcher's classic lobbies account, or one of its own.

The plugin is only its `plugin.json`: the launcher draws the page and runs its actions
(the format: the launcher's `docs/plugins/pages.md`). It needs a classic lobbies server
with the matches API (`/api/matches`, `/api/matches/join`, `/api/matches/current`).

## Trying it

Put this folder into the launcher's data folder as `plugins/event-lobbies/`
(`%LOCALAPPDATA%\EchoVR_Launcher` on Windows, `~/.local/share/EchoVR_Launcher` on Linux)
and start the launcher: it has an Event lobbies tab.

## Releasing

Zip `plugin.json` (at the zip's root), put it on release.echovr.de, and add its entry with
the zip's `sha256` and the new `version` to the launcher's plugins catalogue.
