# Castlevania Mesen

This repository contains re-usable templates to use as HD Packs for Castlevania on Mesen.

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
Work in progress, enemies are not done yet.

### Legend

```
<tile>0,3C3C3C38FCFCFC0024242428C484FC00,FF273707,16,8,1,N,3589879857,18
```

| Position                         | Meaning                             | Type        |
| -------------------------------- | ----------------------------------- | ----------- |
| <tile>                           | Identifying tag                     | String      |
| 0                                | Image index                         | Integer     |
| 3C3C3C38FCFCFC0024242428C484FC00 | Tile ROM index                      | Hexadecimal |
| FF273707                         | Palette used                        | Hexadecimal |
| 16                               | X coordinate                        | Integer     |
| 8                                | Y coordinate                        | Integer     |
| 1                                | Brightness                          | Decimal     |
| N                                | Default tile flag                   | Y or N      |
| 3589879857                       | Foreground or Background identifier | Integer     |
| 18                               | Tile number                         | Integer     |

## TODO

- [x] Map all player sprites
- [x] Map all object sprites
- [ ] Map all enemy sprites
- [ ] Map stage tiles

## Further Reading

For more information, check the official documentation at https://www.mesen.ca/docs/hdpacks.html
