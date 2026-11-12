# Start here: art brief for the image AI

You are making the artwork for **Pixel Alibi**, a cozy pixel-art murder-mystery logic puzzle book. The puzzles are finished. Your job is only the pictures: 226 images in one consistent style, plus an optional cover (227 prompts in all).

## What to make

| Images | What | Size |
|---|---|---|
| 14 | Map objects (chair, sink, oven…), one per image, transparent background | 512×512 |
| 4 | Seamless floor textures | 512×512 |
| 208 | Character portraits, head and shoulders | 1024×1024 |
| 1 | Book cover (optional) | portrait, 8.5×11 ratio |

## How to work

1. Open [art/prompts/batch-01.md](art/prompts/batch-01.md). Every image already has a complete prompt, including the style block, and the exact file name to save it as.
2. Make the images in that batch one at a time, using each prompt as written.
3. Give each image back with its file name (for example `art/tiles/chair.png`) so it can be saved in the right place.
4. Move on to the next batch. Each batch file links to the next one. The full list is in [art/prompts/README.md](art/prompts/README.md).

Do batch 01 (objects and floors) first. Those images appear in every puzzle, and the rules below matter most there.

## Rules that must not be broken

Readers solve the puzzles by recognising objects on a grid, so a confusing drawing can make a puzzle wrong.

- **Same style every time.** Crisp hard-edged pixel art, dark plum outline, the pastel palette in the style block. No blur, no text, no letters, no watermark, no signature.
- **Only sinks, windows and glass may be blue.** No blue screens, cushions or trim on anything else.
- **Stool:** round, wooden, on visible legs, no back, never pink.
- **Chair:** visible back and a pink cushion.
- **Table:** square, white tablecloth, small vase. Not round, not pink, no cake.
- **Counter:** always the same: wood front, grey cash register with a green screen. No cakes on counters.
- **Doormat:** flat brown woven mat seen from above. It must not look like a bench.
- **Display case:** glass case on legs with one gold treasure. It must not look like a bookshelf.
- **One camera for all objects:** three-quarter top-down view, like a cozy farming game, looking down at about 45° so the top and a little of the front show. Floors are straight down.
- **Objects stay inside their square** and fill about 80% of it.
- **Floors tile seamlessly** and stay low-contrast.
- **Nobody looks guilty.** Most characters are innocent in some cases and the killer in another, so every face is friendly and calm, victims included.
- **Portrait framing:** top of the hair about 1/8 down from the top edge, chin about 5/8 down, shoulders running off the bottom, head about half the image width. Same for everyone.
- **Glasses, hats and accessories only when the description mentions them.**
- **A character looks the same everywhere.** One portrait per character, used in every case they appear in.

## Reference

- [ART-PROMPTS.md](ART-PROMPTS.md): the master brief with every character description and object rule. The batch files are built from it.
- [art/CHECKLIST.md](art/CHECKLIST.md): every file that's needed and which ones are done.
