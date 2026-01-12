# EKS Anti-Seat Shuffle

A lightweight FiveM client script that **prevents automatic seat shuffling** and only allows players to shuffle seats **on command or keybind** -> **adjacent seat only** and **only if it's empty**.

## Features
- Stops GTA's **auto seat shuffle** completely
- Allows shuffling **only** via:
  - `/shuffle`
  - Keybind (default: **B**)
- **Adjacent only (same row)**
  - Driver (-1) - Front Passenger (0)
  - Rear Left (1) - Rear Right (2)
- Can't shuffle from front to back (or back to front)
- Uses the **real shuffle animation** (no teleporting)
- If GTA tries to move the player anyway, they are **snapped back** unless they used `/shuffle`

## Commands
- `/shuffle` - Shuffle to the seat next to you (only if empty)

## Keybind
- Default: **B**
- Change it in: **Settings ? Key Bindings ? FiveM**

## Configuration
Edit `config.lua`:
- `Config.CommandName` - command name (default: `shuffle`)
- `Config.DefaultKey` - default keybind (default: `B`)
- `Config.ShuffleTimeoutMs` - max time to wait for shuffle animation to complete

## Installation
1. Put the folder in your server `resources` directory
2. Add this to your `server.cfg`:

## Support

For help or bug reports, join our Discord and open a support ticket:
https://discord.gg/busQ9w6dqa
