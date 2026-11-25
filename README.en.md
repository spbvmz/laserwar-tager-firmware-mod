# LaserWar tager — ZOMBIE firmware mod

[Русская версия](README.md)

Unofficial modification of LaserWar tager firmwares **V9.02.76.3** and **V9.02.82** for lasertag. Adds control of the zombie transformation time and tager ID change **without entering configuration mode**.

## Files

| File | Based on |
|------|----------|
| V9.02.76.3-rus_ZOMBIE.bin | official V9.02.76.3 (RU) |
| V9.02.82-rus_ZOMBIE.bin | official V9.02.82 (RU) |

## What is added

- **Zombie transformation time** — command C5: sets the full time from death to becoming a zombie (0…60 s). Phrase and growl follow the stock schedule. From the remote: **Devices → Zombie → Time**.
- **Tager ID change** — command C6: writes the player ID (0…125) to RAM and EEPROM without configuration mode. From the remote: **Devices → Tager ID**.

Stock game modes and the rest of the tager logic are intentionally unchanged (except for these commands).

## Control from the remote

Requires the modified **Smart PRO Remote v.1** firmware:

https://github.com/spbvmz/laserwar-smart-remote-pro-v1-mod

Without that remote, C5/C6 can still be sent by another MilesTag IR transmitter, but the menu is built for this mod.

## Official firmwares

Official tager firmwares are available from the manufacturer:

https://laserwar.ru/firmware-for-hardware/

This repository contains **no** original LaserWar files — only ready-made modified .bin images.

## Flashing

1. Flash the tager with the modified .bin the same way you normally update LaserWar firmware (configurator / stock update procedure).
2. To control Zombie time and ID, flash the remote with the mod from the repository above (build with zombie/ID menu / current release that includes those items).
3. To restore the official tager firmware, flash the original from https://laserwar.ru/firmware-for-hardware/

## Disclaimer

This is an unofficial project and is **not affiliated** with Laserwar. The firmwares are free and come **without any warranty**; install at your own risk. This firmware is **not from the equipment manufacturer** and is **not supported by them**.

Official firmwares and the Laserwar trademark belong to their owner.

## Contacts

- Author: Telegram [@spbvmz](https://t.me/spbvmz)
- Support group: https://t.me/lasertagpult

Questions, bugs and ideas: the group or repository Issues.
