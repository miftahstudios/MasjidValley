**MASJID VALLEY**

**Decisions Brief — Phaser (In-Browser) Variant**

*Every decision made up to 25 November 2026, in one self-contained handoff.
Copy this document and give it to the Muse who will build the game.*

This is the Phaser variant. The main project chose Godot 4 (see Section 16), but this brief overrides the engine for this variant only: build in Phaser, in the browser. Every other decision in this brief applies unchanged to the Phaser build.

How to use this brief: read Sections 1 and 2 first — they are the rules every change must respect. Work through the build phases in Section 17 in order. Use Section 15 for starting numbers, Section 13 for art, and Section 16 for the Phaser architecture. Where a later decision overrides an earlier document, this brief already states the final version — the Decisions Log in Section 19 shows what was overridden and why. Do not invent Islamic content: Section 18 lists everything that stays a placeholder until Hannah supplies it from her authentic sources.

**Kickoff prompt — copy this to the builder Muse:**

*"You are helping Hannah build Masjid Valley, a cozy Stardew-style game about restoring a masjid. Read this brief in full. Follow Section 2 as hard rules. This variant is built in Phaser for the browser (Section 16). Start with Phase A in Section 17. Before writing any content with Islamic teaching, stop and ask Hannah for the source. Show me the style sheet and the Phase A plan first, then build. Do not copy any Stardew Valley assets, music, UI art, or layouts."*

# 1. How to use this brief

This document is self-contained. The builder does not need the earlier outline, the production brief, or the chat history — everything decided is in here, stated in its final form.

- **Start with the style sheet and the Phase A plan. **Show both to Hannah before building (see Sections 13 and 17).

- **Rules win over features. **When a change conflicts with a rule in Section 2, the rule wins. Flag the conflict to Hannah instead of choosing silently.

- **Numbers are starting values. **Section 15 values come from Stardew’s feel. Tune them in playtests; do not treat them as lore.

- **Placeholders stay placeholders. **Section 18 content is never written from general knowledge. Leave a clearly marked placeholder and ask Hannah.

- **Data-driven throughout. **People, likes, schedules, scenes, projects, crops, recipes, fish, forage tables, and festivals live in config files (Section 16), so the cast and later years can grow without rewriting the engine.

# 2. Non-negotiable rules

These rules govern every system, scene, and asset. They come from the outline and the production brief, with one explicit override by Hannah on 25 November 2026, marked below.

- **No chance. **No random crop quality, drops, loot, or gacha. Every minigame is skill. Istikhara and a child’s arrival are written story beats, never dice rolls presented as chance.

- **Halal economy only. **Honest trade and donations. No gambling, loans, or interest — including for the mahr, the house, and every expansion.

- **Authentic sources only. **Every dua, dhikr, ruling, and teaching line taught by the imam or shaykh comes from Hannah’s Google Drive / AICP sources. Never invent it (see Section 18).

- **Modest relationships. **No dating or living together before the nikah. Courtship runs through trust, counsel, istikhara, and family. Never a scene of a couple alone together before the nikah.

- **Cozy, always — with one override. **No fail state and no child-care meters. Time passing never punishes the player. OVERRIDE (Hannah, 2026-11-25): the former rule of “no trust decay for absence” no longer applies. If the player ignores a character for about one week, that relationship deteriorates by a very small percentage (see Section 5). The exact percentage is a tuning value to be set in playtest, not a fixed number. Apart from this one gentle effect, absence is never punished.

- **Modesty in art. **Women in hijab and abaya with the face visible. Men in kufi and thobe. A range of skin tones. No immodest outfits in the creator, the shops, or any festival scene.

- **Pixel faces are allowed in this game only. **Stardew-style pixel sprites include simple faces for everyone, at every age. This is Hannah’s deliberate exception for this pixelated format, following the Maliki position that drawing them is permissible here. It does not carry into any other Miftah material, which keeps its existing no-faces rule.

- **Clean screen. **Everything that is information rather than play lives behind the single settings (gear) icon and menu (see Section 6).

- **Inspired-by, never copied. **Do not trace, copy, or extract Stardew Valley’s sprites, tiles, portraits, UI art, music, sound effects, fonts, or map layouts. Do not mirror its story beat for beat or reuse its names and invented terms. Genre mechanics, the 16-pixel grid, the top-down 3/4 view, and the hearts-and-gifts structure are fair game; the masjid, family, counsel, and halal-economy scenes lead.

# 3. Concept and story

A cozy Stardew-style farming game about restoring a rundown masjid and bringing its community back to life over one Hijri year — and then living in that community for as many years as the player wants. The masjid is the community center. The loop is Stardew’s loop, recentred: work, earn, give, restore, belong.

## Premise

You return to your grandmother’s neighborhood after years away. The masjid where you grew up is falling apart — the prayer hall carpet is worn thin, the minaret needs repair, the wudu area leaks, the library shelves are empty, and the garden is a tangle of weeds. The community has drifted away. Your grandmother leaves you the keys and one request: bring the masjid back to life.

## The year — five acts

- **Act 1 — Arrival (Muharram–Safar). **A quiet, dusty masjid. Imam Yusuf hands you the keys and the first job: clear the courtyard and fix the garden wall. You learn the basics — till, plant, water, harvest. The masjid cat appears on the second day and decides you belong here. The neighborhood is polite but distant.

- **Act 2 — The Community Wakes (Rabi al-Awwal–Jumada). **People come back. You restore the wudu area and the library shelves. Umm Maryam reopens the children’s classes. The shaykh’s house opens — advice, rulings, and duas. The hunting grounds open and the shaykh teaches zabiha. Hassan opens the community kitchen and teaches the cooking minigame. The first communal meal happens in the courtyard.

- **Act 3 — Preparing for Ramadan (Rajab–Sha’ban). **The big push: restore the prayer hall carpet and repair the minaret. Trust deepens and personal quest lines resolve — the two neighbors arguing over the garden make peace with the shaykh’s help; the market trader offers a shady deal and you turn it down. The neighborhood plans the Ramadan iftars together.

- **Act 4 — Ramadan. **The masjid is full every night. You cook iftar in the kitchen each evening, Taraweeh fills the prayer hall, and Laylat al-Qadr is a special quiet night event. The final big restoration — the dome — completes during the last ten nights. The masjid glows.

- **Act 5 — Eid and After (Shawwal–Dhul-Hijjah). **Eid al-Fitr in the courtyard with everyone you helped. Then Hajj season — some neighbors leave for Hajj and send letters. Eid al-Adha brings the qurbani, tying together everything learned about zabiha. The last restoration finishes.

## The ending — and why it is not the end

There is no fail state. The Year One ending triggers when every main restoration project is complete (or at the end of the Hijri year): Fajr on the final day, the prayer hall full, the garden green, the cat asleep on the new carpet. The player gets a closing scene and a summary — rooms restored, hearts earned, iftars cooked, duas learned, closest friends — and then the game keeps going. The ending unlocks Year Two and beyond (Section 12), the marriage and family path if it has not happened yet (Section 11), and legacy projects. Nothing is taken away, no timer starts, and no one is forced to marry, move, or finish anything by a deadline. A save that finishes Year One unmarried must be able to marry, move, and raise children entirely within Year Two content.

# 4. World and places

Every place has a person attached to it, a prayer-time rhythm, and a visible change when it is restored or when trust grows. Shops keep honest hours — closed at prayer times, open between them — so the world itself teaches the day’s rhythm. Travel is on foot. Paths clear as you restore them, and shortcuts open between the masjid, the market, and the homes once the garden wall is complete (see Section 9).

The world is a real walkable map, not menus or button panels (see Section 6). In Slice 1 the layout is: the masjid with its dome and minarets at the top, the stone courtyard in the middle, Abu Khalid’s market stall on the right, and the fenced garden at the bottom left, joined by dirt paths, trees, and flowers. The full game grows that same layout outward into the neighborhood, the market, the kitchen, the library, and the homes.

| **Place** | **What happens there** | **How it changes** |
| --- | --- | --- |
| The masjid | Prayer, main restoration quests, classes, iftars, Taraweeh, nikah and Eid gatherings | Carpet, wudu area, library, minaret, dome, and tiles restored room by room |
| Your yard and house | Your home from day one: bed, mailbox, yard to clear and shape; later the married home (Section 11) | Debris cleared; house upgrades in place; second building (guest house) on the same plot |
| Courtyard and masjid garden | Farming, communal meals, Eid celebration, children’s play | Weeds to green plots, flower beds, benches, string lights for Ramadan nights |
| Community kitchen | Cooking minigame, iftar prep, walimah feast, Hassan’s quests | Cold and empty to busy; stoves, shelves, and recipes unlock with trust |
| The market | Buy seeds and honest goods, sell harvest, trader storylines | Stalls multiply as the community returns; farmers’ row opens in Year Two |
| Shaykh’s house | Counsel: advice, religious judgments, dhikr and duaa | Opens in Act 2; study and guest bench added as trust grows |
| Imam’s house | Story quests, letters, Hajj-season farewells | Noticeboard for community needs appears outside |
| Neighborhood homes | Visiting, gifts, trust events, family life | Homes gain gardens, lights, and repairs as stories resolve |
| Library | Children’s classes, study, book donations, quiet events | Empty shelves fill; children’s corner and reading circle open |
| River, woods, and old cistern | Fishing with Salim, foraging, hunting grounds, stone/clay/lime gathering (Section 8) | Hunting grounds open in Act 2 after zabiha is learned |
| Guest house and youth space (Year 2+) | Visitors, youth activities, new neighbors arriving | Legacy projects built after the main story (Section 12) |

# 5. People — roster, trust, and community life

Stardew Valley’s staying power is its people, and Masjid Valley is built the same way: 24 named townspeople, each with a home, a job, a daily schedule, favourite gifts, dislikes, a known day (the birthday equivalent), and at least one personal quest line. No one is a generic shopkeeper. Everyone can be befriended, and everyone shows up somewhere different depending on the prayer block, the day, and the season. Schedules, likes, scenes, and projects are data in config files, not hard-coded.

## Trust (hearts) — how relationships work

- **Hearts. **250 points per heart, 10 hearts per person (2,500 points), with extra hearts available for a spouse. Talking gives about +20 once per day per person.

- **Gifts. **Two gifts per person per week. Values are fixed and discoverable: loved about +80, liked about +45, neutral about +20. Disliked and hated gifts give nothing — there are no negative gift points; the person simply says so kindly. A gift on someone’s known day is worth double.

- **Scenes. **Trust milestones unlock personal scenes (heart events): scripted camera pans and NPC movement, with choices that change dialogue but never cause failure.

- **No punishment for a busy day — one gentle exception. **Missing a day, a birthday, or a conversation never costs trust by itself. The single exception is Hannah’s override below.

**Trust deterioration for neglect — Hannah’s decision, 2026-11-25 (explicit override):**

If the player ignores a character for about one week — no conversation, gift, quest help, or other interaction with that person for roughly seven in-game days — that relationship deteriorates by a very small percentage. This directly overrides the “no trust decay for absence” rule as originally written in the production brief’s Section 1 and in the outline. Implement it exactly as a gentle nudge, in the cozy spirit of Section 2: the loss is small, it never applies before the roughly one-week threshold, and any interaction with the character resets the neglect clock. The exact percentage is a tuning value to be set in playtest — do not hard-code a large or punitive figure, and do not present the placeholder percentage as a decided number. Record the chosen playtest value in config so it can be tuned without code changes.

Design intent: relationships need a little tending, just as the garden does — but the game stays cozy. A player who returns after a long absence should find slightly cooler friendships to warm up again, never lost friends, locked scenes, or a fail state.

## The roster — 24 townspeople plus the cat

| **Name** | **Role** | **Usually found** | **Candidate?** |
| --- | --- | --- | --- |
| Imam Yusuf | Imam; main restoration quests; teaches duas | Masjid, before Fajr daily | No — elder / guide |
| Shaykh Abdullah | Shaykh; counsel, fatwa, dhikr and duaa | Shaykh’s house | No — elder / guide |
| Hajja Safiyyah | Elder; storytelling evenings, duaa circle, founders’ history | Her home, masjid | No |
| Umm Maryam | Teacher; library and children’s classes | Library, schoolroom | No |
| Abu Khalid | Gardener; teaches farming, sells seeds | Market stall, his garden | No |
| Hassan | Cook; community kitchen, cooking minigame | Kitchen, market | No |
| Bilal | Carpenter; restoration building work, tool upgrades | Workshop, masjid projects | Yes |
| Hamza | Caretaker’s son; repairs and tile work | Masjid, workshop | Yes |
| Omar | Market assistant; honest-trade storyline | Market, his uncle’s stall | Yes |
| Fatimah | Herbalist; remedies, teas, rosewater still | Herb garden, market | Yes |
| Aisha | Librarian’s assistant; book restoration; Archive | Library | Yes |
| Khadijah | Kitchen assistant; baker; bread oven | Kitchen, courtyard | Yes |
| Karim | Trader; the shady-deal storyline, Year Two redemption | Market | No |
| Tariq | Orchard keeper; young father | Orchard, his home | No |
| Sakina | Tariq’s wife; preserves and jam making | Her home, kitchen | No |
| Idris | Student of knowledge; study circle; Archive | Library, shaykh’s house | No |
| Salim | Fisherman and hunting-grounds guide | River, hunting grounds, market | No |
| Zaynab | Midwife and nurse; family storylines | Her home, visiting rounds | No |
| Nura | Newcomer seamstress; arrives in Act 2 | Guest rooms, market | No |
| Umm Layla | Sewing and Eid clothes | Her home, market | No |
| Abu Omar | Elder neighbor; garden-argument storyline | His home and garden | No |
| Layla | Neighborhood child; flowers and the cat | Courtyard, garden | No — child |
| Maryam (young) | Layla’s older sister; youth classes and youth space | Library, youth space | No — youth |
| Yusuf (young) | Teen helper; wants to learn carpentry | Workshop, masjid | No — youth |

Key storylines to preserve: Imam Yusuf’s quiet trust events (opening the masjid at dawn, handing over the old keys); Shaykh Abdullah’s students who drifted away and return one by one in Acts 2–5; Hajja Safiyyah giving the neighborhood’s history one trust level at a time; Umm Maryam’s multi-season children’s lesson-book quest; Hassan’s line from communal meal to iftars to walimah-scale feasts; Omar caught between easy money and honest trade, where the player’s choice changes how his story ends; Karim’s redemption arc in Year Two at high community trust; Tariq and Sakina’s young-family storyline as a gentle preview of the player’s own family path; Nura welcomed in Act 2 and hosting a newcomer herself in Year Two; Layla’s drawing for the library wall that stays there for the rest of the game.

## Noticeboard and gatherings

The masjid noticeboard posts requests every few days: a crop for the kitchen, cloth for Umm Layla, herbs for Fatimah, books for the library, help carrying, help cooking. Each request names who asked, what they need, and a fair reward in coins, trust, or a recipe. Requests let a farming-focused player still build every relationship, and a people-focused player still use the garden. In Year Two the board gains community projects — larger, multi-person requests that take a season and change the neighborhood visibly. The noticeboard also carries the weather forecast (Section 10) and, each new year, the player’s chosen focus.

| **Gathering** | **When** | **What it does** |
| --- | --- | --- |
| Communal courtyard meal | First in Act 2, then monthly | Cook together; small trust with everyone who attends |
| Ramadan iftars | Every evening in Ramadan | The heart of the year; cooking, gathering, Taraweeh |
| Eid al-Fitr celebration | 1 Shawwal | Everyone helped is there; known-day gifts and sweets |
| Eid al-Adha and qurbani | 10 Dhul-Hijjah | Shared zabiha; meat divided for the neighborhood and families in need |
| Mawlid gathering | Rabi al-Awwal | Remembrance and food at the masjid; elders’ storylines advance |
| Storytelling evenings | Monthly, Hajja Safiyyah’s home | Neighborhood history; children’s and elders’ trust |
| Market day | Weekly | Best prices, special requests, trader storylines advance |

# 6. How you play — opening, creator, map, dialogue, controls, clean screen

## The opening — a scenic introduction

The game opens on a full-screen scenic introduction: a pixel dawn over the valley — hills, the masjid dome, and the minarets — with a short three-paragraph story introduction setting the premise in Section 3. At the foot of the intro a blinking prompt reads “Press X to start.” Pressing X (or tapping the Begin button on touch screens) moves to the character creator, and only after the creator is finished does the walkable game begin. Nothing behind the intro accepts input before then. Note: earlier builds said “Press E to start”; the final decision moves start to X for consistency, so E means menu everywhere (see Controls below).

## The character creator

- **Your name. **The name every townsperson uses with you, in greetings, thank-yous, and wherever it is natural in speech (see Dialogue below).

- **Boy or girl. **Then style the outfit with a live pixel preview that updates as each option changes: qamis colour and kufi style (plain, gold band, embroidered) for a boy; abaya colour and hijab style (classic wrap, soft drape, gold pin — face visible, hair covered) for a girl. Skin tones and simple pixel face options (eyes, expression, face shape in chunky pixels) are chosen alongside.

- **Your masjid cat. **Choose one of the three cats below at the same menu. The choice is permanent for that save: it sets the cat’s colours, its name in the journal and in prompts, and the cat that follows you and, once the carpet is restored, sleeps on it.

| **Cat** | **Look** | **Character** |
| --- | --- | --- |
| Amber | Orange tabby | Warm and visible everywhere; the classic courtyard cat |
| Layl | Black night cat | Dark coat, easy to miss until Isha lantern light catches her eyes |
| Bayda | White patched cat | White with patches; stands out against the stone courtyard |

The cat is part of the map, not a panel: she wanders the courtyard, follows you once her affection is high enough, and sleeps on the new prayer hall carpet once it is restored. All NPCs follow the same modesty rule — every woman wears hijab and abaya, every man wears kufi and thobe. A spouse keeps their own style after marriage, and children are dressed by the same direction as they grow.

## A walkable map, not a text game

Play happens by walking. Your character moves around a top-down Stardew-style pixel map and interacts with what — and who — is in front of them. Walking up to a plot, a person, the market stall, the masjid doorway, or the cat shows a prompt; pressing the interact key does the thing: plant, water, and harvest at plots, talk or hand over task crops, sell at Abu Khalid’s stall, work on restoration at the doorway, pet or feed the cat. WASD or arrow keys, an on-screen D-pad, and tap-to-walk on touch screens all move the same character at the same speed, with a walking animation. Collision is real: buildings, fences, garden plots, trees, and people block movement. Light follows the prayer blocks and the clock: the sky and scene change from Fajr to Isha, and lanterns come on at Isha.

## Talking — dialogue portraits and your name

Talking to any townsperson opens a Stardew-style dialogue box at the bottom of the map: the text on the left, a framed pixel portrait of the speaker on the right, and their name on a name plate under the portrait. Portraits use the same faces as the overworld sprites, larger and more expressive (64×64, several expressions — see Section 13). Dialogue advances with X, E, or a tap, and movement pauses while a dialogue box is open. Task hand-ins, thank-yous, and story lines all play through the same portrait box — there is no separate text-panel mode for talking.

Your character’s name appears inside other people’s speech where it is natural — a greeting, a thank-you, being called across the courtyard — and is left out of lines where it would sound forced. Not every line uses the name.

## Controls — final version, copied from Stardew Valley

One key, one job, everywhere. This table is final: it resolves the earlier conflict where E did two jobs, and it moves the intro start prompt to X to match. The full list also lives inside the game, in the Controls panel of the settings menu.

| **Action** | **Keys** |
| --- | --- |
| Move up / left / down / right | W / A / S / D (arrow keys also work) |
| Run | LeftShift |
| Check / Do Action (talk, interact); also Start on the intro | X or Right-Click |
| Use Tool | C or Left-Click |
| Access Menu | E or Escape |
| Access Journal (task list) | F — and I in Masjid Valley |
| Access Map | M |
| Inventory / hotbar | Number keys 1–0, Minus, Plus (12 slots); mouse wheel; Q cycles in Slice 1 |

On touch screens the same actions are buttons on the map itself: the D-pad to move, an Interact button, and tap-to-walk — tapping a reachable place walks your character there.

## A clean screen — everything extra folds into a settings icon and menu

The game screen stays clean. Around the map the player sees only what is needed while walking and working: the map, the clock with day, date, and coins (top right), the energy bar (bottom right), the hotbar (bottom centre), and a single gear icon that opens the menu. Everything else is folded away behind that one gear icon and opens only when the player asks for it. The task list is the clearest example: it is never pinned to the screen; it lives in the journal, hidden until the player opens it with I or F (or the Tasks button), and closes again with Esc. Opening the menu, the journal, the map, or a dialogue box pauses movement. Rule for every future feature: if a new item is information rather than play, it goes in the settings menu first; it only earns a permanent place on the screen if the player needs it while walking or working.

| **In the settings menu** | **What it holds** |
| --- | --- |
| Journal / Tasks | The hidden task list: current tasks, who asked, what is still owed, and rewards — opened with I or F, closed with Esc |
| Map | The valley map panel (M): the masjid, courtyard, garden, market, and homes, and where people are |
| Controls | The full control list above, Stardew-style, with each action and its key |
| Community | Every townsperson, their trust hearts, discovered likes, and whether you have spoken today |
| Book of duas | Duas and dhikr learned from the imam and the shaykh (Section 8; content from Hannah’s sources only) |
| Garden journal | The day-by-day log of planting, harvests, tasks, and the cat; also the fish and forage guides |
| Settings | Sound and music, display, and accessibility options; save and return to the title / intro |

# 7. Day, clock, and calendar

## The day — prayer blocks plus a visible clock

Fajr to Isha sets the rhythm of the day. Work happens between prayers, and the community gathers at prayer times. The day is divided into prayer-to-prayer blocks, and NPC schedules, shop hours, quest timing, and counsel visits are all counted in prayer blocks: a visit to the shaykh costs one block, cooking an iftar takes the Maghrib block, and nothing important is ever scheduled against a prayer.

On top of the blocks, the day runs on a visible in-game clock (production brief 4.2). The five prayers are fixed points on that clock, with times that shift by season. The clock starts the day at Fajr and allows play until a soft cap after Isha — roughly 14 real minutes for a full day (about seven real seconds per ten in-game minutes) as a starting value. Praying on time gives barakah — a small blessing that makes the day go better (energy lasts longer, crops grow a little faster). Sleeping ends the day and triggers the end-of-day ledger (Section 10). Running out of energy or staying out too late is a soft scene with no penalty — for example, waking on the garden bench under a blanket.

## The year — 28-day Hijri months, and Ramadan drifts

The year runs on Hijri months mapped to Stardew’s rhythm: 28-day months, 12 months per year, a 336-day game year, grouped into four seasons of three months. Birthdays (known days) and festivals appear on a calendar the player can open. Crops change with the season.

**Calendar decision (walkthrough 4.10): Ramadan drifts over the years.**

Do not lock Ramadan to one fixed season. As the years pass, Ramadan moves through the seasons, as the real Hijri year drifts through the solar seasons — so fasting length and iftar timing change over the years, and later years feel different from the first. The outline’s earlier wording that “the calendar repeats every year” is superseded on this point: months, crops, and festivals cycle, but Ramadan’s seasonal position drifts. What changes in later years is therefore the people, the projects, the player’s household — and Ramadan itself.

| **Month(s)** | **Season feel** | **Community life** |
| --- | --- | --- |
| Muharram | Quiet fresh start | New year; arrival in Year One; goal-setting on the noticeboard in later years |
| Safar | Settling in | Garden basics; first requests; the cat arrives (Year One) |
| Rabi al-Awwal | Warming up | Mawlid gathering; wudu and library restoration (Year One) |
| Rabi al-Thani – Jumada | Community wakes | Children’s classes reopen; kitchen and hunting open |
| Rajab – Sha’ban | The big push | Carpet and minaret; iftars planned; shady-deal storyline resolves |
| Ramadan | The heart of the year | Night life: iftar cooking, Taraweeh, Laylat al-Qadr, the dome completes |
| Shawwal | Celebration | Eid al-Fitr in the courtyard; Eid clothes; sweets and visiting |
| Dhul-Qa’dah | Breathing out | Visiting rounds; orchard and market in full swing |
| Dhul-Hijjah | Farewells and sacrifice | Neighbors leave for Hajj and send letters; Eid al-Adha and the qurbani |

Note on the table: the month-to-season groupings describe Year One’s feel. Because Ramadan drifts (above), do not hard-code Ramadan to a single season’s weather, daylight, or crop set for all years — compute its seasonal context from the drift.

# 8. Core systems

## Your own plot — grandmother’s yard

Your grandmother’s house and its overgrown yard are your Year One starting plot (production brief 4.1). It starts with weeds, stones, branches, and fallen limbs to clear. A free-placement grid allows beds, paths, fences, irrigation, and decorations. The masjid garden stays the communal garden, run on the same farming system. Acceptance: a new player can clear debris, till, plant, water, and rearrange their yard in the first in-game week, and sleep in their own bed. The decision for what this plot becomes after marriage is in Section 11: the yard grows into the married home.

## Farming

Till plots, plant, water, harvest — in the masjid garden and, at larger scale, in your own yard and later home garden. Produce feeds the community kitchen and sells at the market. Yields are fixed per crop and care: a well-watered crop always gives its full yield. Crop quality stars are earned from care — watering streaks and fertilizer type — deterministically, and shown in the crop guide. A spouse and older children can help with watering (Section 11). The glasshouse (Section 9) gives year-round crops once restored.

## Tools, energy, and the hotbar

Tools are used on the tile the player faces: hoe, watering can, axe, chisel/pickaxe, scythe, and fishing rod. They sit on a 12-slot hotbar, with inventory growing in steps (12, then 24, then 36 slots). Upgrade tiers are basic, copper, steel, gold, then a final tier — five in all — costing materials plus a few in-game days at Bilal’s workshop. Each tool use costs energy; energy starts near 270 and is extended by upgrades and meals. Eating restores energy, and praying on time gives the barakah effect above. Acceptance: the player feels the pressure of “one more thing before Maghrib” without ever being punished for missing it.

## Fishing, foraging, and the old cistern

- **Fishing. **A skill minigame at the river with Salim. Fish availability is fixed by season, time, and weather, and listed in a journal guide. No random bite luck. Whether fish need any ruling step is an open placeholder for Hannah’s sources (Section 18); the zabiha system applies to land animals.

- **Foraging. **Seasonal wild herbs, dates, and similar, from fixed spawn tables that are visible in the journal, per location, season, and weather.

- **The old cistern — decided. **The gathering area with depth is the old cistern, not a quarry or mine (walkthrough 4.3). It yields stone, clay, and lime for restoration, on a published rotation the player can look up in the journal — never random generation or random drops.

- **Hunting. **The zabiha-gated system below sits beside fishing, not in place of it.

Acceptance: at least three distinct gathering activities feed the restoration and kitchen loops.

## Animals and the artisan chain

Both goats and sheep — decided (walkthrough 4.4) — plus chickens and bees. Each animal has its own friendship meter and a pen or hive the player builds. Sheep and goats can be offered in the Eid al-Adha qurbani; the conditions for suitable animals come from Hannah’s sources only and stay a placeholder (Section 18).

Artisan machines each turn a crop into a fixed-value good that specific people love — grow it, process it, gift it or sell it: preserves jar (with Sakina), bread oven (with Khadijah), rosewater still (with Fatimah), plus a honey extractor, date dehydrator, and olive press. Exclude any alcohol-producing machine, ever. Acceptance: a full chain exists — grow, process, gift or sell — with a named NPC reacting.

## Cooking and tile minigames

Cooking for the community kitchen is a timing-based minigame — stir at the right moment, flip at the right time. Skill, not luck. Good cooking feeds more people and earns more trust. Recipes are earned from people, not bought: Hassan, Khadijah, Sakina, and your spouse each teach dishes at trust milestones. Restoring the masjid’s tiles is a calm pattern-and-timing minigame — place the tiles in the right order — and Hamza’s storyline runs through it, from apprentice work to restoring his grandfather’s tiles in the prayer hall.

## Hunting and zabiha

You can hunt in the woods — rabbits, deer, birds — through a simple skill minigame (sneak and aim, timing-based). If you want to kill an animal to cook it, you must do zabiha, the correct slaughter. The shaykh teaches the method first, and you cannot hunt for food until you have learned it from him. Build the zabiha as a calm, respectful step-by-step sequence engine; the exact sequence wording and steps are supplied by Hannah from her sources and stay placeholders until then (Section 18) — do not write them from general knowledge. Done correctly, the meat is halal and goes to the kitchen; skipped or done wrong, the meat cannot be used. The same rules carry into the Eid al-Adha qurbani.

## The shaykh — counsel system

Visit the shaykh’s house between prayers. Visiting costs one prayer block, so the player chooses when counsel matters most.

- **Ask for advice. **Guidance on a quest or a community problem — for example, how to settle the neighbors’ argument over the garden, or how to organize the iftars. Good advice unlocks the next step of a quest.

- **Ask for a religious judgment (fatwa). **For example, whether a trade is allowed, or how to do zabiha correctly. The answer comes from authentic sources only and unlocks the correct way to do things. This is also where questions about marriage are first brought (Section 11). All answer text is Hannah-supplied placeholder content (Section 18).

- **Learn a dhikr or duaa. **The shaykh (and the imam) teach a dhikr or duaa from authentic sources, which goes into the Book of duas. Reciting it gives a small blessing for the day. All dua text is Hannah-supplied (Section 18).

## The halal economy

Coins come from selling produce at the market and from donations as trust grows. No gambling, no loans, no interest. The player can also give sadaqah — donate coins or produce — which raises community trust and barakah. A shady trader (Karim) offers a dishonest deal once in the story, and turning it down is the right choice. In family life the same economy grows up: a household budget, a bigger garden, and home expansions paid honestly from work and trade.

## Skills with professions

Five skills — Farming, Foraging, Fishing, Cooking, and Restoration — with ten levels each and fixed, known requirements. At levels 5 and 10 the player picks one of two deterministic bonuses (professions): for example, a Farming choice between faster growth and higher sell value. Every skill has two profession forks and no random effects. Knowledge (duas learned and study-circle questions answered) and Community (hearts earned) stay as they are in the outline, tracked alongside the five skills. In post-story play these become the mastery tracks (Section 12).

## Readable rules instead of randomness

Crop quality stars come from care (watering streaks, fertilizer) and are shown in the crop guide. Fishing is skill only, with the guide listing exactly when and where each fish appears. Gathering runs on published tables per location, season, and weather, and the cistern runs on a published rotation. Gift values are fixed and discoverable. Nothing in this section uses hidden randomness.

# 9. Restoration — bundles with choice and unlocks

Restoration is no longer donation-only. Every project becomes a set of bundles — for example, any 4 of 6 items per bundle — so there is more than one way to finish each room. Donate materials and coins, work alongside Bilal and Hamza, and the room visibly changes the moment it is finished: new carpet appears, the minaret is repaired, the shelves fill with books. As rooms complete, real neighborhood volunteers — kids, aunties, neighbors — appear working in the background. Never use spirit-like or fantasy creatures as helpers.

| **Finished project** | **Gameplay unlock** |
| --- | --- |
| Garden wall | Shortcuts open between the masjid, market, and homes |
| Wudu area and library | Recipes and skill books |
| Prayer hall carpet and tiles | Taraweeh and gathering scenes |
| Minaret | A lookout showing the valley map and where people are |
| Glasshouse (kept — see below) | Year-round crops |
| Dome | The Ramadan finale |

Glasshouse — kept (walkthrough 4.5). The glasshouse is in the game: a restored growing space that gives year-round crops, outside the normal seasonal limits.

**The carpet is a bundle, not a single purchase.**

In Slice 1 the prayer hall carpet was a single 120-coin purchase. That is superseded: in this design the carpet is set up as a restoration bundle with a choice of items, like every other project. Do not implement it as a one-price shop purchase. Acceptance for this section: each room has multiple valid ways to finish it and one new thing the player can now do.

# 10. The small loops

- **Mailbox. **Each morning at your house: letters, recipes, and small gifts arrive. This is also where Hajj letters land.

- **Weather. **Rain, wind, heat, and storms. A forecast is posted on the noticeboard (the TV equivalent). Rain waters the crops. Weather changes NPC schedules.

- **End-of-day ledger. **After sleeping, a screen shows earnings and the day’s results by category.

- **Playable festivals. **Each festival has a skill-based activity. Examples to design: an Eid sweets bake-off, lantern-making night, date-harvest fair, Hajj send-off, and qurbani distribution. Which activities are appropriate to play as minigames is Hannah’s call and stays open (Section 18); festival practices themselves come from her sources.

- **Masjid Archive. **The museum equivalent. Aisha and Idris catalogue donated heritage items — old photos, tile fragments, letters. Donations unlock rewards.

- **Secrets. **A few hidden things, such as the founders’ letters through Hajja Safiyyah, or a sealed room in the minaret.

- **Cutscenes and polish. **Heart events use scripted camera pans and NPC movement, with choices that change dialogue but never cause failure. Add emotes above heads, an area-name pop-up when entering a map, fade transitions between maps, and NPCs actually walking (pathfinding) between buildings on their schedules.

# 11. Marriage and family — a halal path to nikah

Masjid Valley keeps Stardew’s wish — to choose a person, build a life, and settle down — and changes the path completely: no dating, no living together before marriage, no casual romance mechanics. Interest is shown through respect, family, and counsel, and the whole neighborhood is part of it. A candidate is eligible regardless of the player’s path through the story — what matters is trust, not speed. A player may also never marry: the game never treats that as an unfinished ending, and every other system, including Year Two content, is fully available either way.

| **Candidate** | **Who they are** | **Where their story lives** | **Loved gifts** |
| --- | --- | --- | --- |
| Bilal | Carpenter; quiet, exact, kind | Workshop and restoration projects | Cooked meals, fine wood, strong tea |
| Hamza | Tile restorer; earnest, wants to prove himself | Masjid tiles, prayer hall | Tile patterns, books on craft, dates |
| Omar | Market assistant; funny, torn over honest trade | Market, his uncle’s stall | Honest-trade goods, cooked food, flowers for his mother |
| Fatimah | Herbalist; calm, knowledgeable | Herb garden, market | Rare herbs, honey, gardening tools |
| Aisha | Book restorer; thoughtful, bookish | Library | Pressed flowers, restored books, paper and cloth |
| Khadijah | Baker; warm, ambitious | Kitchen, courtyard | Baking ingredients, new recipes, flowers |

## The path, step by step

- **1. Trust first. **Reach 8 trust hearts with a candidate through gifts, quests, conversation, and working alongside them. At 8 hearts their personal storyline makes clear, modestly and without a romance scene, that they hold you in high regard and that their family knows your character from the community.

- **2. Counsel and istikhara. **Visit Shaykh Abdullah and choose “Ask for advice” about marriage. He asks who, asks about readiness and means, and advises istikhara. A short sequence follows over the next days: you pray istikhara, and the path either feels opened — the candidate’s family welcomes an approach — or you are gently guided to wait. Waiting is never a failure; trust can keep growing. Scene wording comes from Hannah’s sources (Section 18).

- **3. Approach through family. **With the shaykh’s or Imam Yusuf’s help, your interest is conveyed to the candidate’s family (their wali). A family meeting scene follows — tea, questions, honesty about work, home, and intentions — held with family present, never alone together. The candidate may accept, or may ask for more time, in which case the door stays open and friendship is unharmed.

- **4. The mahr. **Once the family agrees, prepare a mahr — a meaningful gift for the bride, chosen and earned, never bought with a loan: in game terms, a crafted or saved-for item of real value (for example, a restored book, a crafted chest, or saved coins), prepared through play. For a female player, the candidate prepares the mahr for her, and the player chooses what she would value from a short list.

- **5. The nikah. **Held at the restored masjid, with the wali, witnesses, the imam, and the whole community you have befriended — attendance reflects your trust hearts, so a well-loved player marries in a full hall. It is the game’s biggest gathering scene before Eid.

- **6. The walimah. **Hassan, Khadijah, and the kitchen host the walimah feast in the courtyard. The player helps cook it through the cooking minigame — feeding the neighborhood that fed this story is the point of the scene.

Design rule: there is no dating stage, no bouquet or pendant item bought from a shop as a shortcut, and no scene of the couple alone together before the nikah.

## A home of your own — the yard grows into the married home

**Decision (walkthrough 4.1): the yard grows into the married home. There is no separate married-home street.**

After the nikah, the couple’s home is an expansion of the player’s own plot from Section 8 — not a move to a separate site. The house upgrades in place through Bilal’s workshop (or Hamza leads if Bilal is the spouse): a larger kitchen, a guest room, a study, and the nursery, each a restoration-style project with materials and coins, never loans, done together with community help. The home garden grows with it — larger than the masjid plots, with room for an orchard row, herb beds, and flower beds — running on the same fixed-yield farming system as the household’s own income and kitchen supply, separate from the masjid garden the player still tends for the community. The guest-house legacy project becomes a second building on the same plot (it is not a separate street either), so visitors and newcomers stay properly and grandmother’s house ties the family story back to the premise. This supersedes the outline’s earlier “house plot on the quiet street beyond the masjid garden” wording.

## Life with a spouse

Your spouse keeps their job and their people: a married Bilal still works the workshop, a married Aisha still restores books — they leave after Fajr, work their block, and come home. Marriage adds a household; it does not remove a townsperson from the town. A spouse helps in small, visible ways — watering part of the home garden on some mornings, cooking a dish for the house, mending, or leaving a short note — as a kindness with a pattern the player can learn, never a random bonus. You share the prayer-block day at home too: meals together in the evening block, a shared duaa from the Book of duas, and spouse dialogue that changes with the seasons, Ramadan, your projects, and your children. Each spouse has married-life scenes at new trust milestones beyond the original 10 hearts — settling in, the first Ramadan as a household, hosting the elders, supporting each other’s work. Gifts and conversation still matter, and a spouse keeps their own likes, known day, and place on the Community page, now marked as your household.

## Up to two children

Once the home has the nursery expansion and the household has settled (a season of married life), the couple may have a child. Zaynab, the midwife, is part of the arrival, and the whole neighborhood visits with food. The game supports up to two children, spaced naturally by the family’s story. A second child requires the children’s room project first — home, then family, then a bigger home, the household version of the masjid restoration loop. Children have names chosen by the player from a warm list (or typed), simple likes, and a personality note — one may love the garden, the other the library. Children never create a fail state, a cost spiral, or a chore checklist: feeding, playing, and teaching are scenes and choices, not meters. With two children, sibling scenes appear, and the older child visibly looks out for the younger in gatherings. Children are modestly dressed like everyone else, in the same pixel art with simple pixel faces.

| **Stage** | **Roughly** | **What changes** |
| --- | --- | --- |
| Baby | First months | Nursery life; Zaynab visits; neighbors bring meals; parents’ work blocks are shorter, kindly, with no penalty |
| Toddler | Year after arrival | First steps around the house and courtyard; the masjid cat adopts the child; short, sweet home scenes |
| Child | From about age four in game years | Attends Umm Maryam’s classes, learns duas from your book, helps carry (never farm labour), befriends Layla and the neighborhood children |
| Older child | Year Three onward | Small errands, own known day, helps in the home garden, joins youth activities as the youth space grows |

# 12. Life after Year One — the game continues

Finishing the five acts ends the restoration story, not the game. From Shawwal of Year One onward — and in full from Muharram of Year Two — the game becomes an open life in a place the player has already changed. The Hijri year cycles forever (with Ramadan drifting, Section 7). Crops, months, Ramadan, and the Eids return, but dialogue, requests, and gatherings are written for “a masjid that is alive now”: iftars you host rather than rescue, classes you support rather than reopen, newcomers who arrive because the neighborhood has a name for welcoming people. Each Eid al-Fitr, the closing summary returns as a yearly reflection, and the player chooses a focus for the new year on the noticeboard — the garden, the library, the youth, guests, or family. It sets which community projects appear most; it locks nothing away.

| **Legacy project** | **What it adds** |
| --- | --- |
| Community hall | Weddings, walimahs, large classes, and gatherings move indoors in winter months; new group scenes |
| Youth space | Maryam’s project: youth helpers, study nights, and a new generation of quests as children grow |
| Guest house (second building on your plot) | Visitors and newcomers stay properly; a new arrival storyline most years |
| Orchard expansion | Tariq teaches grafting; multi-year trees that mature across several Hijri years |
| Library second room | A full catalogue quest: one donated book per townsperson, including your spouse and, later, your children |
| Market farmers’ row | Khadijah’s bakery stall, Fatimah’s herb stall, and the player’s own stall on market day |
| Masjid endowment garden | A sadaqah garden whose fixed yield feeds families on Zaynab’s list every week — the halal economy’s endgame |

- **Generational change. **Yusuf the teenager becomes Bilal’s apprentice, then a carpenter. Layla grows from child to class helper. Tariq and Sakina’s baby becomes a toddler alongside the player’s own children. Elders’ storylines conclude gently and their roles are carried by the next generation — Hajja Safiyyah’s storytelling evenings are hosted, in time, by Maryam.

- **New neighbors. **Roughly one household arrives each year (through the guest house storyline), with its own trust arc, likes, and requests.

- **Old friends deepen. **Every townsperson gains post-story dialogue and at least one Year Two quest line — Karim’s redemption at the market, Nura hosting a newcomer herself, Omar running an honest stall of his own.

- **Mastery and player-chosen goals. **Skill mastery, earned only by doing, with five levels per skill and fixed, known requirements — no random drops — unlocking recipes, crop varieties, tile patterns, and home and garden upgrades. A personal goals board at home tracks optional goals: grow every crop, cook every recipe, learn every duaa, reach max trust with everyone, complete the library catalogue, raise the endowment garden. None are required; all are tracked.

- **Completion of Care. **Perfection, Stardew-style, renamed: a single quiet page showing how much of the valley you have tended — restorations, legacy projects, hearts, recipes, duas, family milestones. Reaching it triggers one final optional scene: Fajr in a full masjid, your family beside you, the cat asleep on the carpet. Play continues afterwards, unchanged.

# 13. Art direction and art bible

The same pixelated style as Stardew Valley — chunky, warm, top-down pixel art, with small tiled maps, cozy interiors, seasonal palettes, and little character sprites you can read at a glance — recoloured for this world, with the masjid and garden in soft greens and golds. Faces are included (see Section 2): sprites have simple pixel faces — eyes, nose, mouth, and expressions — for the player, townspeople, a spouse, and children, in portraits and in the overworld. Modesty shapes every sprite: women in hijab and abaya with the face visible, men in kufi and thobe, a range of skin tones. The masjid is the visual centerpiece and visibly comes back to life as you restore it; homes follow the same rule, growing from a frame, to a home, to a family home with a nursery and children’s room.

**Masjid architectural reference — DECIDED (Hannah, 2026-11-25): Ottoman.**

The masjid’s architectural reference is Ottoman: cascading grey-blue domes, tall pencil-thin minarets with conical caps, and light stone. Keep this reference consistent across every building in the game — the masjid, homes, market, and all later buildings draw from the same Ottoman vocabulary of domes, minarets, arches, and light stone, so the valley reads as one place. This resolves the former open item “masjid architectural style”; it is decided, not open (see Sections 18 and 19). Do not substitute a different regional style for individual buildings.

## Technical rules

- 16×16 tiles. Characters 16×32 with four directions and about four walk frames. Portraits 64×64 with several expressions.

- Draw at native size and scale up by whole numbers only (3× or 4×), using nearest-neighbor. Never mix pixel sizes. Never rotate or scale sprites.

- 3/4 top-down view: building fronts and roofs are visible. Walls are two to three tiles tall. Sprites sort by Y so players walk behind objects (in Phaser this is hand-built — see Section 16).

- A soft oval shadow under every sprite and object.

## Color, texture, and animation

- Pick one palette of 30–50 colors before drawing anything. Warm, saturated, slightly muted. No pure black or white. Lospec has good starting palettes.

- Characters and objects get a dark desaturated brown or navy outline. Terrain stays mostly outline-free. Shadows shift toward blue or purple; highlights shift toward yellow. One light source from the top left everywhere. Seasons are recolors of the same tileset.

- Grass uses two or three base tiles with sparse tufts and flowers; avoid noisy dithering. Paths and water edges use autotiling. Crops have four to five growth stages with a clear ready state.

- Add swaying grass and trees, water shimmer, chimney smoke, cat idle animations (sit, groom, sleep), tool swing animations, and emote bubbles above heads.

## Lighting

Day to night is a multiply-tint overlay running Fajr to Isha. Lanterns are additive glow. Rain is particles with a darker tint. Interiors get their own lighting.

## Characters

At 16×32 a face is only a few pixels: carry personality through silhouette, hijab and kufi shape, color, and posture; portraits carry the expression. Build characters in layers with a shared frame layout — body, outfit, hijab or kufi, accessory — and use indexed-color palette swapping for outfit colors and skin tones, which also gives the creator its live preview cheaply. Hijab styles: classic wrap, soft drape, gold pin. Kufi styles: plain, gold band, embroidered. Abaya and qamis/thobe in varied colors. Children and teens use the same system at smaller sizes.

## UI and identity

Warm brown wooden frames with cream parchment inside, beveled pixel borders, and small drop shadows. Use a bitmap pixel font under an open license — verify the license. Test Arabic text early: most pixel fonts have no Arabic, so duas need a tested solution before dialogue content is written (still open — Section 18). Islamic geometry suits pixel grids: use it for tile patterns, screens, and arches, tied to the tile restoration minigame, with teal and turquoise zellige-style accents against the greens and golds — within the Ottoman reference above.

## Production workflow

- Build a style sheet first: ten tiles, one tree, one building, one NPC, one portrait, one UI frame. Approve it at 1× before producing more.

- Draw in Aseprite, LibreSprite, or Pixelorama. Build maps in Tiled.

- Starter packs from itch.io (for example Sprout Lands) can serve prototypes — check that the license allows commercial use and modification. The masjid and all key scenes need custom art.

- Do not use AI image generators for sprites. They break pixel-grid consistency.

- If commissioning an artist, give them the style sheet and use Stardew screenshots for mood only. Ask for original work.

# 14. Audio rules — decided

- **Music: duff or percussion-only. **Rhythmic tracks with duff or percussion only; no melodic instruments. Nature ambience (birds, wind, rain, footsteps) sits alongside it. This was Hannah’s choice among nature-ambience-only, vocal-only, and duff/percussion-only.

- **The adhan: a ding and a visual, never the actual adhan. **When a prayer time arrives in-game, play a simple ding and show a visual cue (banner / prayer-time change). Do not play a recording or rendition of the actual adhan.

- **Recitation: dedicated listening scenes only. **Qur’an recitation plays only in a dedicated listening scene — for example, sitting in the prayer hall to listen. It never plays as background audio while the player is farming, cooking, hunting, or doing other gameplay.

- **Sound effects needed regardless: **footsteps by surface, tool hits, watering, harvest, UI clicks, birds, wind, rain, and character dialogue blips.

# 15. Reference numbers — starting values, tune in playtest

| **System** | **Starting value** |
| --- | --- |
| Day length | Clock runs about 7 real seconds per 10 in-game minutes; a Fajr-to-after-Isha day is roughly 14 real minutes |
| Friendship | 250 points per heart; 10 hearts per person (2,500 points); extra hearts for a spouse |
| Gift values | Loved about +80, liked about +45, neutral about +20; disliked / hated give nothing (no negative points); known-day gift is doubled |
| Talking | About +20, once per day per person |
| Gifts per week | 2 per person |
| Trust deterioration for neglect (Hannah, 2026-11-25) | After about 1 week of no interaction with a character, that relationship deteriorates by a very small percentage. Exact percentage is a playtest tuning value in config — not a fixed decided number |
| Energy | Starts near 270; upgrades and meals extend it |
| Inventory | 12 slots, expanding to 24, then 36 |
| Skills | 10 levels each; professions at levels 5 and 10 |
| Tool tiers | 5 (basic, copper, steel, gold, final tier) |
| Month length | 28 days; 12 months; 336-day year |

# 16. Phaser build notes — this variant’s engine

**Engine for THIS variant: Phaser (in-browser JavaScript). This overrides the production brief’s Section 8 engine choice for this variant only.**

Be explicit with the builder: the main project’s walkthrough chose Godot 4 as its engine, and that Godot decision still stands for the main project. This brief exists so Hannah can also have a Phaser, in-browser version built from the same decisions. For this variant, Phaser wins wherever the two conflict — browser delivery, browser saves, and hand-built engine features below. Do not build this variant in Godot, and do not treat the Godot choice as a reason to change any design decision in Sections 2–15.

- **What Phaser gives you, and what you hand-build. **Phaser provides the browser game loop, scenes, input, cameras, tilemaps, and physics. Y-sorting (depth by Y position), autotiling beyond Phaser’s basics, and the Fajr-to-Isha lighting (tint overlays, lantern glow, interior lighting) must be hand-built deliberately — budget for them in Phase A rather than discovering them in Phase C.

- **Data-driven config. **People, likes, schedules, scenes, projects, crops, recipes, fish, forage tables, festivals, bundle contents, and unlocks live in config files / data objects, so the cast and Year Two content can grow without rewriting the engine. Zabiha and counsel scenes are step-by-step sequences: build the sequence engine first and fill in Hannah-verified content later.

- **Core systems to build. **Tile grid and free placement, tool use and energy, time and clock with prayer markers, save/load, NPC pathfinding and schedules, dialogue and portrait box, cutscene scripting, inventory and hotbar, shop and shipping/selling, quest and noticeboard, minigame framework (cooking, tile, fishing, zabiha), weather, and lighting.

- **Saves in the browser. **Saves live in the browser (for example localStorage / IndexedDB). Save compatibility matters: a save that finishes Year One unmarried must be able to marry, move (expand the home plot), and raise children entirely in Year Two content. Version the save format from Phase A.

- **Cozy Farm Starter — verify or build from scratch. **The outline names Cozy Farm Starter, a tiny farming game/template in plain JavaScript with one HTML file and a config for map, crops, prices, and texts, as a possible clean starting point. Verify its MIT license in its own repository before touching any of its code. If the license does not check out, build the slice from scratch instead. The same verify-first rule applies to any starter pack or third-party code.

- **No Stardew assets. **Nothing is copied from Stardew Valley — no sprites, tiles, portraits, UI art, music, sound, fonts, or map layouts (Section 2). Inspired-by only.

# 17. Build phases and acceptance tests

Build in this order. Show Hannah the style sheet and the Phase A plan first, then build Phase A.

## Phase A — Slice 1.5, the playable test

Scenic intro (Press X to start), character creator (name, boy or girl, outfit styles, cat choice of Amber, Layl, or Bayda). Your own yard with debris to clear, six tillable plots, three crops (mint, tomatoes, melons — all fixed yields), a hoe and a watering can, an energy bar, and a ticking clock with the five prayers marked. A Fajr-to-Isha day with lighting changes, an end-of-day ledger, and sleeping in your own bed. The masjid courtyard map (Ottoman reference, Section 13), the cat, and Imam Yusuf, Umm Maryam, and Abu Khalid with portrait dialogue and natural use of the player’s name. The task list hidden in the journal; everything extra behind the single gear menu. One restoration project — the prayer hall carpet — set up as a bundle (Section 9), not a single purchase.

*Pass if: a new player goes from intro to a first harvest, a sale, and a restored carpet in one sitting and understands every control.*

## Phase B — the prototype

Add fishing, foraging, the old cistern, a Ramadan week, trust hearts with six townspeople (including the neglect rule in Section 5, with its percentage as a config tuning value), gift likes, the kitchen cooking minigame, shaykh counsel, hunting with zabiha, three restoration bundles with unlocks, the noticeboard, mailbox, and weather.

*Pass if: one in-game month feels like Stardew’s first month — always something new to do before dusk.*

## Phase C — Year One

The full Hijri year with Ramadan drifting by year, all five acts, the full 24-person roster with schedules, likes, known days, and heart scenes, animals and artisan machines, festivals, the Masjid Archive, skills with professions, the qurbani, and the ending.

## Phase D — family and beyond

The marriage path with all six candidates, the home expanding on the player’s own plot with nursery and children’s room, up to two children with growth stages, legacy projects, generational change, mastery, the goals board, and Completion of Care.

# 18. Open items and placeholders — never invent

The builder leaves clear placeholders for everything in this section and never writes it from general knowledge. When a system needs this content, build the system and mark the content as awaiting Hannah’s source.

- **Every dua and dhikr **in the Book of duas.

- **The zabiha sequence wording **and the qurbani conditions, including which animals are suitable.

- **All shaykh counsel, **fatwa-style answers, and istikhara scene wording.

- **The marriage path scene details: **wali, mahr, nikah, and walimah wording beyond the structure in Section 11.

- **Festival practices **and the Ramadan, Laylat al-Qadr, and Hajj-season scene content.

- **Any ruling about trade, animals, or food **that a quest depends on — including whether fish need any ruling step in the shaykh’s lessons (production brief 4.3).

- **Which festival activities are playable minigames. **Examples are listed in Section 10, but Hannah decides which are appropriate to play.

- **The Arabic font solution for duas. **Most pixel fonts have no Arabic; this needs testing early, before dialogue content is written.

- **The trust-deterioration percentage. **Decided in principle (Section 5) but the exact figure is a playtest tuning value, not yet a number.

Decided — no longer open: the masjid architectural style. It is Ottoman (Section 13), decided by Hannah on 25 November 2026. Do not list it as open and do not ask Hannah to re-decide it.

Content rule for all of the above: every dua, ruling, recipe-with-ruling, and teaching line comes from Hannah’s Drive / AICP sources. If it is not in her sources, it stays a placeholder and the builder says so plainly.

# 19. Decisions log — what was decided, and where it came from

Use this log to audit the brief. “Final form in this brief” is what the builder implements; earlier wordings that conflict are superseded and should not be rebuilt.

| **Topic** | **Decision (final form)** | **Source** |
| --- | --- | --- |
| Art format and faces | Stardew-style pixel art; simple pixel faces included for everyone — Maliki-based exception for this pixel format only; other Miftah material keeps no-faces | Hannah feedback 2026-11-24; outline §§13–14 |
| World presentation | Full walkable top-down map with collision and walking animation — not a text game or button panels | Hannah feedback 2026-11-24; outline §§3, 12 |
| Opening | Scenic intro, then character creator, then the walkable game | Hannah request 2026-11-25; outline §12 |
| Intro start key | Press X to start (moved from E for consistency) | Walkthrough 4.9 decision |
| Character creator | Name, boy/girl, abaya/qamis + hijab/kufi styling, skin tones, pixel face options, live preview | Hannah request 2026-11-25; outline §§8, 12 |
| Masjid cats | Choose 1 of 3 at the creator: Amber, Layl, Bayda; choice is permanent per save | Hannah request 2026-11-25; outline §12 |
| Player name in dialogue | Townspeople use the player name where natural; not forced into every line | Hannah request 2026-11-25; outline §12 |
| Dialogue | Stardew-style box with speaker portrait (64×64) and name plate; movement pauses | Hannah request with Stardew screenshots 2026-11-25; outline §12 |
| Task list | Hidden in the journal; opened with I or F, closed with Esc — never pinned to the screen | Hannah request 2026-11-25; outline §12 |
| Controls | Final Stardew layout: X interact/start, C tool, E menu, F journal (I also opens journal), M map, WASD/arrows, Shift run | Hannah request 2026-11-25 + walkthrough 4.9 fix |
| Screen layout | Clean screen; everything extra folds into one gear (settings) icon and menu | Hannah request 2026-11-25; outline §12 |
| Own plot (4.1) | Grandmother’s yard is the Year One plot: clear, till, plant, rearrange in week one; sleep in own bed | Production brief 4.1, adopted in walkthrough |
| Married home (4.1) | The yard grows into the married home; upgrades in place via Bilal; guest house is a second building on the same plot — no separate street | Walkthrough 4.1 decision (Hannah) |
| Tools, energy, clock (4.2) | 6 tools, 12-slot hotbar, 5 upgrade tiers at Bilal’s, energy per use, barakah for on-time prayer, visible clock with prayers marked, sleep + ledger, soft no-penalty late scene | Production brief 4.2, adopted as written |
| Gathering area (4.3) | The old cistern (not a quarry): stone, clay, lime on a published rotation | Walkthrough 4.3 decision (Hannah) |
| Fishing and foraging (4.3) | Fishing skill minigame with Salim, fixed by season/time/weather in journal guide; foraging from fixed published tables | Production brief 4.3, adopted as written |
| Animals (4.4) | Both goats and sheep, plus chickens and bees; each with friendship meter and pen/hive | Walkthrough 4.4 decision (Hannah) |
| Artisan chain (4.4) | Preserves (Sakina), bread oven (Khadijah), rosewater still (Fatimah), honey extractor, date dehydrator, olive press; no alcohol machine ever | Production brief 4.4, adopted as written |
| Restoration (4.5) | Bundles with choice (e.g. any 4 of 6); each room unlocks a feature; real volunteers in background, no spirit creatures | Production brief 4.5, adopted as written |
| Glasshouse (4.5) | Kept: year-round crops | Walkthrough 4.5 decision (Hannah) |
| Carpet | A restoration bundle, not a single 120-coin purchase (Slice 1 form superseded) | Production brief 4.5 / Phase A |
| Small loops (4.6) | Mailbox, weather + forecast, end-of-day ledger, playable festivals, Masjid Archive (Aisha + Idris), secrets, cutscene/polish set — all in | Production brief 4.6, adopted as written |
| Skills (4.7) | Farming, Foraging, Fishing, Cooking, Restoration: 10 levels, professions at 5 and 10; Knowledge + Community stay as outline | Production brief 4.7, adopted as written |
| Determinism (4.8) | Quality from care, fishing skill-only with guide, gathering on published tables, gift values fixed and discoverable | Production brief 4.8, adopted as written |
| Calendar (4.10) | 28-day Hijri months, 336-day year, known days + festivals on calendar; Ramadan drifts through seasons over the years | Walkthrough 4.10 decision (Hannah) |
| Music (§7) | Duff or percussion-only | Walkthrough §7 decision (Hannah) |
| Adhan and recitation (§7) | Adhan = ding + visual, never the actual adhan; recitation only in a dedicated listening scene | Walkthrough §7 decisions (Hannah) |
| Engine — main project (§8) | Godot 4 for the main project | Walkthrough §8 decision (Hannah) |
| Engine — this variant (§8) | Phaser, in-browser — variant-specific override of the Godot choice; all other decisions unchanged | Hannah request for this brief 2026-11-25 |
| Trust deterioration for neglect | Ignoring a character for about 1 week deteriorates that relationship by a very small percentage; exact % is a playtest tuning value. Explicitly overrides “no trust decay for absence” | Hannah decision 2026-11-25 |
| Masjid architectural style | Ottoman: cascading grey-blue domes, tall pencil-thin minarets with conical caps, light stone — consistent across every building. Resolves the former open item | Hannah decision 2026-11-25 |
| Reference numbers (§5) | Day ~14 min, 250 pts/heart, gifts +80/+45/+20 (known day double), talk +20/day, 2 gifts/week, energy ~270, inventory 12→24→36, 10 skill levels, 5 tool tiers, 28-day months | Production brief §5 |
| Art bible (§6) | 16×16 tiles, 16×32 characters, 64×64 portraits, whole-number scaling, Y-sorting, 30–50 color palette, Islamic geometry + zellige accents, style sheet first, no AI sprites | Production brief §6 |
| Build order (§9) | Phases A (Slice 1.5) → B (prototype) → C (Year One) → D (family and beyond), style sheet + Phase A plan first | Production brief §9 |

End of brief. If anything in Sections 2–18 conflicts with this log, follow Sections 2–18 — they already state the final form — and flag the conflict to Hannah.
