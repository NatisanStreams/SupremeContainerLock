# SCL - Supreme Container Lock

A lightweight Skript-based container protection system. Players lock their chests, barrels, furnaces, blast furnaces and smokers in a single click and manage everything from a clean GUI - no commands to memorise. Ownership is stored directly on the block using persistent data, so locks survive restarts, chunk reloads and server migrations without any external database.

## Features

- **One-click locking** - claim any supported container as yours instantly
- **GUI management** - lock, unlock, trust, untrust, list and clear from one menu
- **Trust system** - grant specific players access to your container
- **Full protection** - blocks access, breaking, hopper transfers and explosions for non-owners
- **Chat-based player selection** - type a username to trust or untrust, with a 30 second timeout
- **Admin tools** - force unlock and inspect any locked container
- **Persistent storage** - ownership lives on the block via persistent data, no external database
- **Tab completion** - clean, permission-aware command suggestions

## Supported Containers

- Chest
- Barrel
- Furnace
- Blast Furnace
- Smoker

## Commands & Permissions

| Command | Description | Permission |
|---------|-------------|------------|
| `/scl manage` | Open the management GUI for the container you're looking at | `scl.use` |
| `/scl force_unlock` | Forcefully unlock a container | `scl.admin` |
| `/scl force_list_trusted` | View a container's owner and trusted list | `scl.admin` |

Players with `scl.admin` bypass all container protection.

## Dependencies

- [Skript](https://github.com/SkriptLang/Skript) `2.15.0+`
- [SkBee](https://modrinth.com/plugin/skbee/versions) `3.25.0+`
- [Skript-GUI](https://github.com/APickledWalrus/skript-gui)

## Installation

1. Install all dependencies above on a Paper server.
2. Drop the `.sk` file into `/plugins/Skript/scripts/`.
3. Run `/sk reload scl` (or restart the server).
4. Lock a container with `/scl manage` while looking at it.

## License

Released under the MIT License. See [LICENSE](LICENSE) for details.
