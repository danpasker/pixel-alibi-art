# Art drop folder

Finished art from the outside image generator goes here.

| Folder | What goes in it | Size |
|---|---|---|
| `portraits/` | One head-and-shoulders portrait per character, named by character id (`lily.png`) | 1024×1024 |
| `tiles/` | One object per file, transparent background (`chair.png`) | 512×512 |
| `floors/` | Seamless floor textures (`plank.png`) | 512×512 |

1. Use the prompts and rules in [ART-PROMPTS.md](../ART-PROMPTS.md). Paste the style block before every prompt.
2. Save each PNG with the exact name from [CHECKLIST.md](CHECKLIST.md).
3. Run the art status script in the main project to tick off what's done and catch wrong names or sizes.

Do the 14 objects and 4 floors first: they appear in every case, and the legibility rules in ART-PROMPTS.md matter for the puzzles (only sinks, windows and glass may be blue; stools are round, wooden and never pink).
