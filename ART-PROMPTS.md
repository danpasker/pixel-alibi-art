# Pixel Alibi: art prompts

Prompts for the outside image generator (Grok, ChatGPT, etc.). Two jobs:

1. **Portraits**: 208 characters. Each person keeps one portrait for every case they appear in.
2. **Map art**: 14 objects and 4 floors. The book builds every room from these pieces.

Paste the **style block** at the start of every prompt, then add the line for the character or object you want.

---

## Why rooms are built from pieces

Don't ask the AI to draw whole rooms. Every puzzle depends on exactly which object sits in which square and where the walls are. An AI room picture won't line up with the grid. Even one wrong object can change the answer: in playtesting, a cash register that looked like a sink gave Case 11 a second solution.

So the AI draws **one object at a time**. The book places each object in its square and draws the walls, windows, doors and labels itself. A room's look comes from its floor and the objects in it.

---

## Style block (paste first, every time)

> Cozy pixel art in the style of a modern indie game. Crisp, hard pixel edges with no blur and no anti-aliasing, as if drawn on a 32×32 grid and scaled up. Dark plum outline (#2E1A47). Soft pastel palette built on cream #FFF7E8, lavender #E9D7FF, purple #6B3FA0, pink #FFC9D6, peach #FFDDB8, sky blue #D6EAFE, mint #DFF7E6, butter yellow #FFE38A and rose #E07A8F, with warm wood browns (#C98B55, #9C6439). Flat colors with 1–2 shading tones. No text, no letters, no watermark.

---

## 1. Portraits

### Format

- Square PNG, **1024×1024**, facing forward, centered.
- **Framing:** Head and shoulders: top of the hair about 1/8 of the way down from the top edge, chin about 5/8 of the way down, shoulders running off the bottom edge, head about half the image width. Same framing for every character.
- Glasses, hats and other accessories only when the character's description mentions them.
- Plain two-tone backdrop in the color listed for the character, with a dithered pixel band across the middle.
- Name the file by the character's **id**: `art/portraits/<id>.png` (e.g. `art/portraits/lily.png`).

### Portrait prompt template

> [Style block] Head-and-shoulders portrait of **[description]**. Friendly, calm expression with a small smile. Facing the viewer, centered, same framing as a trading card. Plain [backdrop] background with a dithered band. Cozy murder-mystery cast member.

**Important: nobody should look guilty.** Most characters are innocent in some cases and the killer in another, so every face has to stay friendly and neutral. Victims look normal too.

### Characters

| id | Name | Description for the prompt | Backdrop |
|---|---|---|---|
| honey | Mrs. Honey | kindly older woman, silver-lilac hair in a bun, round purple-framed glasses, purple cardigan over a white baker's apron | pink |
| marco | Chef Marco | cheerful man, tall white chef's hat, brown hair and thick brown mustache, red neckerchief | sky blue |
| lily | Lily | young woman, copper-orange hair with a yellow bow on one side, freckles, white blouse | mint |
| brooks | Mr. Brooks | middle-aged man, neat brown hair, round glasses, brown cardigan, orange tie | peach |
| dan | Dan | young delivery man, tan skin, short dark hair, blue cap with a yellow badge, blue work jacket | lavender |
| vale | Ms. Vale | elegant woman, deep brown skin, dark plum bob, purple blazer, gold earrings, red lipstick | lavender |
| rosa | Rosa | warm woman in her 50s, dark curly hair with a red rose tucked in, green apron | pink |
| basil | Basil | gentle gardener, sandy hair, straw sun hat, green overalls, a sprig of leaves in his pocket | mint |
| ivy | Ivy | teenage girl, black hair in two buns, green striped top, bright smile | mint |
| ash | Mr. Ash | slick landlord, grey slicked-back hair, charcoal suit, thin smile | peach |
| petra | Petra | young woman, blonde ponytail, pastel pink coat, tote bag strap | pink |
| agatha | Agatha | elderly woman, white hair in a bun, pearl necklace, lavender cardigan | lavender |
| hart | Colonel Hart | old military man, white handlebar mustache, tweed jacket, medal ribbon on chest | peach |
| nell | Nell | young waitress, auburn hair in a bun, black dress, white frilly apron | pink |
| felix | Felix | round-faced cook, rosy cheeks, ginger beard, white cook's cap, flour on his cheek | butter yellow |
| penny | Miss Penny | stylish woman, black bob, red beret, colorful feather brooch | sky blue |
| quill | Mr. Quill | thin old librarian, bald with white side hair, half-moon spectacles, bow tie | lavender |
| edith | Edith | elderly archivist, grey hair in a tight bun, cat-eye glasses on a chain, grey cardigan | peach |
| rory | Rory | scruffy student, messy brown hair, oversized green hoodie, backpack strap | butter yellow |
| page | Mrs. Page | bookish woman in her 60s, wavy grey hair, purple shawl, reading glasses on her head | pink |
| sloane | Dr. Sloane | professor, neat grey beard, tweed jacket with elbow patches, rolled map under his arm | peach |
| tess | Tess | young volunteer, deep brown skin, curly hair with a headband, yellow cardigan | lavender |
| victor | Victor Lane | hotel manager, slicked dark hair, burgundy suit, gold name badge | sky blue |
| bella | Bella | bartender, deep brown skin, braids tied up, black vest, white shirt | pink |
| otto | Otto | young bellhop, red pillbox hat, red uniform with gold buttons | butter yellow |
| finch | Mrs. Finch | small elderly woman, white curls, blue hat with a little feather, pearl earrings | sky blue |
| jules | Jules | young receptionist, dark side-parted hair, navy blazer, neat tie | lavender |
| sasha | Sasha | travel writer, light brown skin, long dark hair, round sunglasses pushed up, green scarf | mint |
| pell | Mr. Pell | postmaster, grey mustache, blue postal cap and blue uniform | sky blue |
| gina | Gina | young woman, East Asian, black hair in a high ponytail, red hoodie | pink |
| gus | Gus | jolly ice cream man, big belly, white paper hat, pink-and-white striped shirt | pink |
| leo | Leo | teenage boy, light brown skin, curly black hair, orange t-shirt | butter yellow |
| rook | Mr. Rook | antiques dealer, monocle, grey goatee, brown waistcoat with pocket-watch chain | peach |
| odette | Odette | mysterious woman, black hair in a long braid, dark green shawl, small brass key necklace | mint |
| mina | Mina | young woman, South Asian, black bob, big round glasses, lavender sweater | lavender |
| bert | Bert | barber, bald with a big black mustache, white barber's jacket, comb in his pocket | sky blue |
| earl | Earl | burly trucker, red trucker cap, bushy brown beard, plaid flannel shirt | peach |
| barnaby | Barnaby | stablehand, deep brown skin, short beard, flat cap, brown vest | mint |
| bramble | Mrs. Bramble | pet shop owner, grey curly hair, green apron, a small bird perched on her shoulder | mint |
| wren | Wren | traveling musician, light brown skin, wavy chestnut hair, mustard scarf, guitar strap | butter yellow |
| teo | Teo | friendly cleaner, Latino, short black hair, blue work shirt | sky blue |
| lark | Professor Lark | museum curator, short white hair, black turtleneck, gold brooch | lavender |
| hugo | Hugo | big gentle security guard, deep brown skin, shaved head, navy guard cap and uniform | sky blue |
| vance | Mr. Vance | wealthy collector, slicked silver hair, cravat, velvet jacket | lavender |
| pearl | Pearl | gift shop owner, blonde updo, pink cardigan, pearl necklace | pink |
| sal | Sal | diner owner, balding, black mustache, white t-shirt, paper diner hat | butter yellow |
| dot | Dot | veteran waitress, big red curly hair, pink uniform, pencil behind her ear | pink |
| ruby | Ruby | diner cook, dark hair in a red bandana, white cook's shirt | peach |
| pike | Mr. Pike | health inspector, thin, side-parted hair, grey suit, clipboard | sky blue |
| stern | Gordon Stern | CEO, grey hair, sharp black suit, red power tie | lavender |
| priya | Priya | accountant, South Asian, long black hair, rectangular glasses, teal blazer | mint |
| wes | Wes | IT guy, shaggy blond hair, headset around his neck, grey hoodie | sky blue |
| marge | Marge | receptionist, big grey perm, cat-eye glasses, pastel blue cardigan | sky blue |
| kit | Kit | saleswoman, sleek black bob, red blazer, confident smile | pink |
| vivian | Vivian Hale | painter, wild silver hair, paint smudge on her cheek, artist's smock | butter yellow |
| cobb | Stationmaster Cobb | stationmaster, white beard, navy conductor's cap with gold trim | sky blue |
| reginald | Sir Reginald | theatrical actor, swept-back silver hair, ruffled collar, velvet cape | lavender |
| lucille | Lucille | glamorous singer, deep brown skin, finger-waved black hair, sparkly purple gown, pearl earrings | lavender |
| coco | Coco Bellamy | chocolatier, brown bob, brown apron, chocolate smudge on her cheek | peach |
| raoul | Raoul | head chef, dark hair, thin black mustache, white double-breasted chef jacket | sky blue |
| grimsby | Headmaster Grimsby | stern headmaster, thin grey hair, black academic gown, small spectacles | lavender |
| clara | Clara | young housemaid, light brown hair under a white maid's cap, black dress | pink |
| thornbury | Mayor Thornbury | mayor, round face, grey mustache, gold mayoral chain over a dark suit | butter yellow |
| crane | Mr. Crane | thin accountant, slicked black hair, round glasses, grey vest, ledger in hand | peach |
| rex | Rex Rumble | radio DJ, pompadour hair, big headphones around his neck, loud Hawaiian shirt | butter yellow |
| duke | Duke | bartender, deep brown skin, neat beard, black vest, bow tie | peach |
| ashby | Lord Ashby | old aristocrat, white hair, white mustache, maroon smoking jacket | lavender |
| lady | Lady Ashby | aristocratic woman, silver updo, pearl choker, dark green gown | mint |
| graves | Mr. Graves | butler, slicked grey hair, long serious face (but polite), black tailcoat, white gloves | lavender |
| moss | Dr. Moss | family doctor, kind face, salt-and-pepper beard, stethoscope around his neck | mint |
| celeste | Celeste | young heiress, blonde waves, beret, Paris-chic striped top | pink |
| tom | Old Tom | old innkeeper, white bushy beard, red cheeks, brown apron | peach |
| maud | Maud | inn cook, grey bun, rosy cheeks, plain blue dress, apron | sky blue |
| silas | Silas | traveler, wide-brimmed hat, dark stubble, long brown coat | peach |
| montague | Mr. Montague | hotel owner, white hair, white mustache, gold-trimmed tuxedo | butter yellow |
| ingrid | Ingrid | spa owner, Scandinavian, platinum braid, white robe-style top | mint |
| fiona | Fiona | concierge, red hair in a French twist, navy uniform with gold keys pin | sky blue |
| gull | Captain Gull | lighthouse keeper, white beard, navy captain's hat, yellow raincoat | sky blue |
| sterling | Mr. Sterling | bank manager, neat grey hair, pinstripe suit, gold watch chain | butter yellow |
| horace | Old Horace | clockmaker, wispy white hair, jeweler's loupe on his eye, brown work apron | peach |
| rousseau | Madame Rousseau | French winemaker, silver bob, burgundy scarf, sun hat | pink |
| frost | Mr. Frost | lodge owner, icy white beard, red knit sweater with a snowflake | sky blue |
| bancroft | Mr. Bancroft | country club president, tan, white hair, green blazer with a crest | mint |
| orsino | Count Orsino | aristocrat, black hair, ornate gold Venetian mask pushed up on his forehead, black cape | lavender |
| thistle | Mrs. Thistle | elderly head gardener, white hair under a wide straw hat, green gardening apron, soil on her gloves | mint |
| beatrice | Beatrice | cheerful beekeeper, round face, golden curls, yellow-and-black striped scarf, a tiny bee on her shoulder | butter yellow |
| june | June | young florist, light brown skin, short black curls with a daisy tucked in, lavender apron | lavender |
| hattie | Hattie | retired schoolteacher, grey bob, red reading glasses on a chain, knitted cardigan | pink |
| lou | Big Lou | burly bowling alley owner, bald, big grin, red-and-white bowling shirt | pink |
| hank | Hank | mechanic, deep brown skin, grey stubble, oil-stained blue overalls, wrench in his pocket | sky blue |
| pip | Pip | freckled teenage paperboy, ginger hair, flat newsboy cap, satchel strap | butter yellow |
| ink | Mr. Ink | newspaper editor, rolled-up sleeves, green visor cap, pencil behind ear, grey mustache | mint |
| quinn | Quinn | photographer (they/them), short teal-dyed hair, round glasses, camera strap, black turtleneck | mint |
| arlo | Arlo | friendly mail carrier, Latino, short black hair, blue postal cap and satchel | sky blue |
| ned | Big Ned | fishmonger, big beard, yellow oilskin hat, rubber apron | sky blue |
| rufus | Rufus | weathered fisherman, grey beard, navy wool beanie, cable-knit sweater | sky blue |
| ezra | Ezra | carpenter, sandy hair, short beard, flannel shirt, pencil behind ear | peach |
| nora | Nora | new head librarian, East Asian, black hair in a neat bun, cat-eye glasses, burgundy cardigan | lavender |
| stellan | Dr. Stellan | astronomer, wild grey hair, star-patterned bow tie, tweed jacket | lavender |
| hollis | Mr. Hollis | miller, flour-dusted beard, flat cap, brown waistcoat | peach |
| greta | Greta | baker, blonde braids pinned up, rosy cheeks, white apron with flour handprints | pink |
| lenny | Lenny Fox | cinema owner, slicked-back hair, thin mustache, red velvet jacket | pink |
| desmond | Desmond | jazz pianist, deep brown skin, neat grey beard, burgundy waistcoat, bow tie | lavender |
| ophelia | Ophelia | fortune teller, long dark wavy hair, purple headscarf with coins, big hoop earrings | lavender |
| pocket | Mr. Pocket | toymaker, white beard, round spectacles, green waistcoat with a measuring tape | mint |
| mabel | Mabel | seamstress, silver bun with pins stuck in it, tape measure around her neck, pink blouse | pink |
| hargrove | Judge Hargrove | stern old judge, white wig, black robe | lavender |
| moreau | Captain Moreau | riverboat captain, grey mustache, white captain's hat, navy coat with brass buttons | sky blue |
| magnifico | Ringmaster Magnifico | ringmaster, curled black mustache, red tailcoat, top hat | butter yellow |
| ambrose | Brother Ambrose | elderly monk, bald crown with white fringe, brown habit | peach |
| whitcombe | Mr. Whitcombe | department store owner, silver hair, pinstripe suit, pocket square | lavender |
| kessler | Baron Kessler | music critic, monocle, sharp grey goatee, fur-collared coat | lavender |
| falcone | Signor Falcone | opera tenor, dark curly hair, dramatic ruffled shirt, red sash | pink |
| blackwood | Lord Blackwood | aristocrat, black hair with grey streak, dark velvet coat, signet ring | lavender |
| winters | Mrs. Winters | prim cake judge, white hair in a bun, pearl earrings, fur hat | sky blue |
| pembrook | Commodore Pembrook | ship commodore, white beard, white uniform with gold epaulettes | sky blue |
| gage | Sir Percival Gage | inventor, brass goggles on his forehead, frizzy white hair, leather apron | butter yellow |
| penrose | Mayor Penrose | mayor, round spectacles, silver hair, gold mayoral chain, dark suit | butter yellow |
| ferris | Mr. Ferris | old ticket seller, grey sideburns, navy waistcoat, ticket punch on a cord | sky blue |
| flynn | Flynn | friendly ferryman, curly brown hair, short beard, yellow rain jacket, rope over his shoulder | sky blue |
| cora | Cora | athletic swimmer, deep brown skin, short natural hair, red swimsuit strap under a striped towel | mint |
| hector | Hector | retired sailor, white captain's beard, navy peacoat, anchor tattoo, pipe in pocket | sky blue |
| primrose | Mrs. Primrose | salon owner, towering lilac bouffant, cat-eye glasses, pink smock | pink |
| kiki | Kiki | hairdresser, bright pink bob, scissors tucked behind her ear, black smock | pink |
| iris | Iris | young painter, East Asian, messy bun with a paintbrush stuck through it, paint-spattered overalls | lavender |
| molly | Molly | dairy farmer, freckles, red bandana, denim overalls, milk pail | butter yellow |
| petrov | Coach Petrov | skating coach, slicked silver hair, sharp cheekbones, fur-collared coat, whistle | sky blue |
| elsie | Elsie | figure skater, blonde hair in a tight bun, sparkly teal leotard, white earmuffs | mint |
| dex | Dex | skater teen, light brown skin, backwards red cap, hoodie, sticking plaster on his cheek | butter yellow |
| gwen | Gwen | gym teacher, short auburn hair, sporty headband, tracksuit, whistle around her neck | peach |
| jasper | Jasper | young magician, slicked black hair, thin mustache, purple velvet waistcoat, top hat | lavender |
| barker | Dr. Barker | kind vet, round glasses, grey curly hair, white coat with a paw-print badge | mint |
| ada | Ada | vet nurse, deep brown skin, braided bun, teal scrubs, stethoscope | mint |
| tilly | Tilly | girl scout, freckles, two brown pigtails, green scout scarf and badges | butter yellow |
| bram | Bram | burly blacksmith, bald, thick black beard, leather apron, soot on his cheek | peach |
| giles | Farmer Giles | old farmer, ruddy cheeks, flat cap, straw in his mouth, green wellies | mint |
| sid | Sid | taxi driver, middle-aged, bushy mustache, checkered flat cap, leather jacket | butter yellow |
| vera | Vera | retired detective, sharp grey bob, trench coat, magnifying glass on a chain, knowing smile | lavender |
| uly | Uly | old gardener, white stubble, straw hat, green apron, gentle smile | mint |
| wheeler | Mr. Wheeler | bus driver, round face, blue uniform cap, grey mustache | sky blue |
| nico | Nico | young barista, Italian, dark wavy hair, black apron, coffee cup | peach |
| olive | Olive | bookkeeper, neat brown bun, round glasses, olive-green cardigan, pencil behind ear | mint |
| zoltan | The Great Zoltan | grand old magician, pointed white beard, star-covered purple turban, cape | lavender |
| percy | Percy | butler, slicked silver hair, long face, black tailcoat, white gloves, polite | lavender |
| brawn | Coach Brawn | muscular gym owner, buzz cut, red tank top, sweatband | peach |
| lionel | Lionel | banker, slicked blond hair, pinstripe suit, gold tie pin | butter yellow |
| dewey | Mr. Dewey | bookseller, bald, white beard, half-moon glasses, brown cardigan | peach |
| walt | Walt | night janitor, middle-aged, grey cap, blue coveralls with a name patch, quiet smile | sky blue |
| roz | Roz | radio host, deep brown skin, big curly hair, headphones around her neck, red lipstick | pink |
| coalby | Mr. Coalby | old master blacksmith, white beard, leather cap, soot-streaked face | peach |
| brava | Señor Brava | coffee roaster, Latino, grey mustache, fedora, brown apron | peach |
| shelby | Mrs. Shelby | seaside hotel owner, sun hat, big sunglasses, striped blouse | sky blue |
| goldie | Mr. Goldie | pawnbroker, bald, gold monocle, green visor, gold tooth | butter yellow |
| volkova | Madame Volkova | ballet teacher, severe grey bun, black leotard, shawl, cane | lavender |
| gears | Mr. Gears | taxi firm owner, big belly, oil-stained shirt, chewed cigar (unlit) | butter yellow |
| laurent | Monsieur Laurent | famous French painter, curly grey hair, beret, neck scarf | lavender |
| marlin | Mr. Marlin | fishing lodge owner, tan, fishing hat covered in lures, khaki vest | mint |
| lavender | Lady Lavender | flower show judge, purple hat with flowers, pearls, lilac gloves | lavender |
| vasquez | Dr. Vasquez | head doctor, Latina, dark hair in a bun, white coat, stethoscope | sky blue |
| max | Max Kilobyte | arcade owner, spiky green-dyed hair, pixel-print t-shirt, headset | mint |
| ravenswood | Lady Ravenswood | 90-year-old aristocrat, white hair in an elaborate updo, black lace collar, cameo brooch | lavender |
| bramwell | Mr. Bramwell | zookeeper, safari hat, khaki shirt, kind weathered face | mint |
| calloway | Mrs. Calloway | hot springs owner, silver bob, white robe, towel around her neck | pink |
| gavel | Mr. Gavel | auctioneer, slicked-back hair, bow tie, pinstripe waistcoat | butter yellow |
| fairweather | Mayor Fairweather | new mayor, deep brown skin, silver locs, gold mayoral chain, rosette | butter yellow |
| agnes | Agnes | church organist, grey bun, round spectacles, lavender cardigan, sheet music | lavender |
| barty | Barty | street sweeper, flat cap, ginger sideburns, green work jacket, broom handle | mint |
| clem | Clem | young farmhand, sunburnt, straw-blond hair, checked shirt, braces | butter yellow |
| delphine | Delphine | elegant perfumer, French, black chignon, silk scarf, perfume bottle pendant | pink |
| edgar | Edgar | young undertaker, pale, slicked black hair, black suit, polite small smile | lavender |
| fern | Fern | park ranger, freckles, auburn braid, olive ranger hat and badge | mint |
| gideon | Gideon | pharmacist, neat dark hair, round glasses, white coat, pill bottle in pocket | sky blue |
| hazel | Hazel | candlemaker, chestnut curls, wax-stained apron, little flame earrings | peach |
| ivo | Ivo | accordion player, curly grey hair, red waistcoat, accordion strap | pink |
| jo | Jo | mechanic, short black hair, grease on her cheek, blue overalls, spanner | sky blue |
| kip | Kip | chimney sweep, soot-smudged face, black top hat, cheeky grin | lavender |
| lottie | Lottie | cake decorator, pink pigtails, sprinkles on her apron, piping bag | pink |
| monty | Monty | retired actor, silver pompadour, cravat, theatrical smile | lavender |
| opal | Opal | jeweler, sleek silver bob, loupe on a chain, opal earrings | mint |
| pru | Pru | postmistress, tight grey curls, red cardigan, postal badge | pink |
| quentin | Quentin | architect, tall, slicked brown hair, turtleneck, rolled blueprints | sky blue |
| saffron | Saffron | spice merchant, South Asian, long black braid, orange shawl, gold bangles | butter yellow |
| toby | Toby | baker's boy, freckles, flour on his nose, white cap, basket of bread | butter yellow |
| winnie | Winnie | knitting circle member, white curls, knitted beret, half-finished scarf | pink |
| wickham | Mr. Wickham | candlemaker, long grey beard, waistcoat, candle in hand | peach |
| ashdown | Reverend Ashdown | vicar, kind face, white clerical collar, thinning grey hair | lavender |
| pestle | Mr. Pestle | old pharmacist, bald, half-moon glasses, white coat | sky blue |
| fleur | Madame Fleur | perfumer, silver updo, pearls, lilac silk blouse | pink |
| oakes | Ranger Oakes | park ranger, grey beard, wide-brimmed ranger hat, green jacket | mint |
| mortimer | Mr. Mortimer | old undertaker, long thin face, black top hat, black coat | lavender |
| sugarman | Mrs. Sugarman | cake baker, round rosy face, white bun, frilly apron | pink |
| carat | Mr. Carat | jeweler, bald, monocle, velvet waistcoat, gold watch chain | butter yellow |
| brio | Maestro Brio | bandleader, wild white hair, tailcoat, baton | lavender |
| drummond | Mr. Drummond | property developer, slicked hair, sharp grey suit, gold cufflinks | butter yellow |
| dunmore | Mr. Dunmore | car dealer, loud checked jacket, big grin, car keys | peach |
| clove | Mr. Clove | spice trader, turban, grey beard, embroidered jacket | butter yellow |
| purl | Mrs. Purl | knitting circle head, grey bun with knitting needles in it, cardigan | pink |
| mortlake | Lord Mortlake | old aristocrat, gaunt, black cloak, silver-topped cane | lavender |
| pullman | Mr. Pullman | hotel owner, round face, bowler hat, railway-themed waistcoat | sky blue |
| featherstone | Lady Featherstone | aristocrat, huge feathered hat, pearls, garden-party dress | pink |
| ambleside | Bishop Ambleside | bishop, white hair, purple vestments, mitre | lavender |
| frostberg | Count Frostberg | icy aristocrat, white hair, fur collar, silver crown pin | sky blue |
| quarrel | Professor Quarrel | stern professor, bushy grey eyebrows, tweed jacket, bow tie | peach |
| kroft | Mr. Kroft | film director, beret, sunglasses, megaphone | butter yellow |
| rudd | Admiral Rudd | admiral, white mustache, navy blazer with gold buttons, captain's cap | sky blue |
| noel | Mr. Noel | market organizer, rosy cheeks, red scarf, white beard (not Santa — no hat) | pink |
| hollow | Lord Hollow | last of an old family, pale, dark velvet coat, family ring | lavender |
| vane | Mr. Vane | museum curator, neat black hair, round spectacles, tweed waistcoat | mint |

**Masquerade note (Case 30):** draw everyone normally. The book uses the same portraits.

---

## 2. Map art

### Format

- **Objects:** PNG with a transparent background, **512×512**, seen in three-quarter top-down view (see the camera rule below). Each object fills about 80% of the square and must never spill outside it.
- **Floors:** square PNG, **512×512**, **seamless** (tiles without visible joins), top-down, quiet and low-contrast so objects and people stand out.
- **Camera:** Same camera for every object: a three-quarter top-down view like a cozy farming game, looking down at about 45°, so you see the top surface and a little of the front. Floors are the only exception: straight down.
- File names: `art/tiles/<name>.png` and `art/floors/<name>.png`, using the names below.

### Object prompt template

> [Style block] A single **[object]**, in three-quarter top-down view (camera looking down at about 45°), centered, with a transparent background. Game sprite for a grid map. Must read clearly at 1 inch wide.

### Rules that matter for the puzzles

The puzzles depend on readers telling these apart at a glance:

- **Only sinks, windows and glass may be blue.** Nothing else gets a blue patch. (A blue cash-register screen created a second solution in playtesting.)
- **Chair vs stool vs table:** a chair has a visible back and a pink cushion; a stool is a round **wooden** seat with no back; a table is pink with a tablecloth and a cake. Never make a stool pink: a pink stool looked like a table in playtesting.
- **Rug vs doormat:** a rug is square, pink and decorative; a doormat is flat, brown and woven, and must never look like a bench.
- **Table vs desk vs worktable vs counter:** each needs its own shape and props (see below).
- **Boxes stay inside their square.**

### Objects (14)

| name | What to draw | People can stand on it? |
|---|---|---|
| `chair` | wooden chair with a clear back and a pink cushion | yes |
| `stool` | round wooden stool seat on short visible legs, seen from above, **no back**, not pink, must not look like a crate | yes |
| `rug` | square pink rug with a simple concentric pattern | yes |
| `mat` | flat brown woven doormat lying on the floor (a thin flat rectangle, no height), no slats or fringe (must not look like a bench) | yes |
| `table` | square table with a white tablecloth, pink trim and a small vase of flowers (not round, not pink, no cake) | no |
| `desk` | wooden office desk with drawers, a lamp and papers | no |
| `worktable` | sturdy butcher-block table with a rolling pin and flour dust | no |
| `counter` | shop counter, wood front, grey cash register with a **green** screen and a gold drawer. Every counter looks the same: no cakes on counters | no |
| `shelf` | tall wooden bookshelf with colorful books | no |
| `boxes` | two stacked cardboard boxes, inside the square | no |
| `oven` | cream-and-grey oven with an orange glowing window | no |
| `sink` | white sink with a **blue** water basin and a tap | no |
| `plant` | leafy green plant in a terracotta pot | no |
| `display` | glass display case on short legs holding one golden treasure (light blue glass allowed; must not look like a shelf of books) | no |

### Floors (4)

| name | What to draw |
|---|---|
| `tile` | cream and lavender checkerboard tiles |
| `checker` | cream and pink checkerboard tiles |
| `plank` | light honey-colored floorboards |
| `wood` | warm brown parquet / herringbone wood |

---

## 3. Optional: cover

> [Style block] Book cover illustration for "Pixel Alibi", a cozy murder-mystery puzzle book. A night-time pixel-art street in a small town called Hollowmere: a bakery, a library, a hotel and a lighthouse, with warm lit windows, a starry deep-purple sky, and a few silhouetted townsfolk. Leave the top third clear for a title. Portrait orientation, 8.5×11.

---

## Handing the files back

Put the PNGs in `art/portraits/`, `art/tiles/` and `art/floors/` using the names above. [art/CHECKLIST.md](art/CHECKLIST.md) lists all 226 files (the cover is optional and extra); run `node scripts/art-status.js` to tick them off and catch misspelled names or wrong sizes. The book and app then need a small update to use them in place of the current placeholder pixel art.
