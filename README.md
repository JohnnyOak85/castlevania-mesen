# Castlevania Mesen

This repository contains re-usable templates to use as HD Packs for Castlevania on Mesen.

With this you can recolor or replace every sprite within the game.

## Image files

These are 256 × 256 blocks that contain the various sprites used in the game.

- `00.png`: Player and intractable objects in the first palette.
- `01.png`: Player and intractable objects in the second palette.
- `02.png`: Player and intractable objects in the third palette.
- `03.png`: Player and intractable objects in the fourth palette.
- `04.png`: Player in the fifth palette.
- `05.png`: Enemies in the second palette.
- `06.png`: Enemies in the third palette.
- `07.png`: Enemies in the fourth palette.

## Text file

The `hires.txt` file contains the tile information for each `.png` file included.

Work in progress, HUD is not done yet.

### Legend

```
<tile>0,3C3C3C38FCFCFC0024242428C484FC00,FF273707,16,8,1,N,3589879857,18
```

| Position                           | Meaning                                                   | Type        |
| ---------------------------------- | --------------------------------------------------------- | ----------- |
| `<tile>`                           | Identifying tag                                           | String      |
| `0`                                | Image index                                               | Integer     |
| `3C3C3C38FCFCFC0024242428C484FC00` | Tile ROM index                                            | Hexadecimal |
| `FF273707`                         | Palette used                                              | Hexadecimal |
| `16`                               | X coordinate, ranges from `0` to `120` in increments of 8 | Integer     |
| `8`                                | Y coordinate, ranges from `0` to `120` in increments of 8 | Integer     |
| `1`                                | Brightness, ranges from `0.0` to `1.0`                    | Decimal     |
| `N`                                | Default tile flag, either `Y` or `N`                      | String      |
| `3589879857`                       | Foreground or Background identifier                       | Integer     |
| `18`                               | Tile number, ranges from `0` to `255`                     | Integer     |

## TODO

- [x] Map all player sprites
- [x] Map all object sprites
- [x] Map all enemy sprites
- [ ] Map all HUD sprites
- [ ] Map stage tiles

## Further Reading

For more information, check the official documentation at https://www.mesen.ca/docs/hdpacks.html
