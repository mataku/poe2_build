# Stormweaver — matites

Multi-element self-cast Sorceress, Energy Shield + life hybrid. Season 0.5.5 "Forbidden Rites", aimed at endgame mapping.

**Work in progress (last synced 2026-10-07, level 94).** Comet (cold) and Arc (lightning) are the two damage skills, each cast from its own weapon set with an element-specific staff. The build is past leveling gear but not settled; this is a record of where things stand so the next session can start from it.

- Character: `matites` (Sorceress / Stormweaver)
- Profile: https://poe.ninja/poe2/profile/matakuchan-0487/forbiddenrites/character/matites
- PoB: not stored — a PoB code goes stale with every gear swap or level-up, so ask for a fresh export each session instead of reading a saved one. Prefer it over the poe.ninja import for gear — poe.ninja caps every item at five displayed lines and rune lines eat that budget. The user plays on macOS and cannot run PoB directly, so PoB numbers come only from the stats saved in the code.

## Current state

From the level 94 PoB export (2026-10-05) and the 2026-10-07 poe.ninja import:

| Axis | Now | Decided? |
| --- | --- | --- |
| Damage skills | Comet (Unleash + Spell Echo) on set 1, Arc (Unleash + Living Lightning) on set 2, Ice Nova secondary, Cast on Critical with Comet + Living Bomb | Yes |
| Element | Cold on set 1 (Gelid Staff), lightning on set 2 (Paralysing Staff); each set's weapon-set passive points follow its element | Yes |
| Damage scaling | Spell levels (Comet 31, Arc 29) → gain-as-extra → crit chance (Maligaro's 250% fixed bonus) → spell damage | Yes |
| Defence | ES + life hybrid (7,902 ES, 1,336 life on PoB); target is Chaos Inoculation + pure ES | Yes, as of 2026-09-16 |
| Ascendancy | Stormweaver (see Passive tree for the reported nodes) | Yes |

## Skill setups (poe.ninja, 2026-10-07)

- **Comet** (Lv19, 20% quality) — Elemental Focus + Rapid Casting II + Unleash + Spell Echo + Cold Mastery. PoB main skill.
- **Cast on Critical** (Lv19, 20%) — Comet (Lv18) + Living Bomb (Lv3) + Elemental Focus + Rapid Casting II + Spell Cascade
- **Arc** (Lv19, 20%) — Unleash + Projectile Acceleration III + Rapid Casting II + Living Lightning II + Lightning Mastery
- **Ice Nova** (Lv19, 20%) — Magnified Area II + Deep Freeze + Rapid Casting II + Freeze + Cold Mastery
- **Freezing Shards** (Lv18, Gelid Staff implicit) — Rapid Casting II + Mana Flare + Cold Mastery + Wildshards II
- **Enervating Nova** (Lv18, Paralysing Staff implicit) — Lightning Mastery + Zenith I + Rapid Casting II. Electrocute tool, not a damage source.
- **Frost Bomb** (Lv16, 20%) — Cooldown Recovery II + Cold Attunement + Magnified Area II + Short Fuse I + Rapid Casting II
- **Elemental Weakness** (Lv14, 20%) — Rapid Casting II + Burning Inscription
- **Orb of Storms** (Lv10, 20%) — Harmonic Remnants II
- **Mana Remnants** (Lv19, 20%) — Harmonic Remnants II
- **Arctic Armour** (Lv14, 20%) — Freeze

## Passive tree

No keystone allocated.

Ascendancy nodes reported by the import — **unconfirmed**, because the MCP has no verifiable ascendancy data and `import_pob` returned an empty ascendancy list: **Constant Gale** (Arcane Surge), **Force of Will** (20% of damage taken from mana before life, Arcane Surge effect per missing mana), **Archon of the Storm** (Lightning Archon after spending 100% of maximum mana), **Refracted Infusion** (50% chance for a second Elemental Infusion).

Notables resolved by the 2026-09 import (re-check against the current 143-point tree before relying on the list):

- **Crit** — Controlling Magic, Critical Overload, Sudden Escalation
- **Spell / elemental** — Raw Power, Turn the Clock Forward, Elemental Force, Practiced Signs
- **Cold** — Glaciation, Endless Blizzard (+1 to cold spell levels)
- **Lightning** — Electric Amplification
- **ES** — Pure Energy, Patient Barrier
- **Mana** — Arcane Blossom, Open Mind, Ingenuity

Small nodes skew heavily toward mana regeneration (13 of them) and generic spell / elemental damage. Three jewel sockets, all filled.

**Data caveat.** The local MCP tree is `data-v0.5.0-r12`. `check_tree_freshness` calls it current against poe.ninja's `PassiveTree-0.5` tag, but 15 of 143 allocated nodes do not resolve, the starting class comes back as "Unknown", and the tree is reported as disconnected. Treat those as data artifacts of a 0.5.5 tree the local bundle predates, not as build problems, and confirm any specific node in game before acting on it.

## Gear (PoB 2026-10-05 for item text, poe.ninja 2026-10-07 for later swaps)

Rune values below are from the PoB item text — the MCP has no rune or soul-core data.

- **Set 1: Miracle Song** (Gelid Staff, bought 2026-09-22, 37 div) — +7 to Level of all Cold Spell Skills, 128% + 85% increased Spell Damage, Gain 50% of Damage as Extra Cold, 36% cast speed, 50% mana regen, +79 mana. Runes: Hedgewitch Assandra's Rune of Wisdom (+1 to Level of all Spell Skills, bonded Archon recovery 30% faster) and Saqawal's Rune of the Sky (5% of Damage as Extra of all Elements, bonded 12% chance for a duplicate Elemental Infusion). Both runes are limited to one equipped. Implicit grants Level 18 Freezing Shards.
- **Set 2: Ghoul Weaver** (Paralysing Staff, bought 2026-09-19, 35 div) — +7 to Level of all Lightning Spell Skills, 250% increased Spell Damage, 42% cast speed, Gain 56% as Extra Fire, 15% of Elemental as Extra Cold, +212 mana, 48% spell crit damage bonus (dead under Maligaro's). Rune: Perfect Iron Rune (35% increased Spell Damage, bonded armour break). Implicit grants Level 18 Enervating Nova. No mana regen.
- Staff shopping rule (measured on Arc): levels first, then every gain-as-extra line, then cast speed, then spell damage. Mana regeneration on a staff matters less than it looks: total increased regen is around 700%, so a staff's 50% is under a tenth of it, while +100 maximum mana is worth about 11%.
- Retired staves: Kraken Goad (+5 all, 50% Extra Fire), Corruption Chant (Ashen Staff).
- **Beast Star** (Kamasan Tiara, 485 ES, corrupted) — +64 ES, 87% and 35% increased ES, +30 mana, Cold 40% / Lightning 32% / Fire 34%, 28% mana regen enchant. Rune: Perfect Iron Rune (20% AES, bonded +20 life / +20 mana).
- **Skull Shelter** (Vile Robe, 1,151 ES, corrupted) — 110% and 41% increased ES, +29 and +96 ES, Fire 36% / Lightning 35%, 26.4 life regen. Three Perfect Iron Runes (60% AES, bonded +60 life / +60 mana).
- **Maligaro's Virtuosity** (Fine Bracers) — 27% increased Critical Hit Chance, Critical Damage Bonus fixed at 250%, crit chance cannot be rerolled. Evasion, attack speed and Dexterity are dead weight. Rune: Greater Glacial Rune (+18% Cold Resistance).
- **Maelstrom Urge** (Luxurious Slippers, 202 ES) — 131% increased ES, +30 Intelligence, Cold 37% / Fire 34%, 20% movement speed, +71 stun threshold. Rune: Greater Glacial Rune (+18% Cold Resistance).
- **Mageblood** (Utility Belt, bought 2026-10-07, 390 div, replaced Sorrow Locket) — two charm slots, 20% of flask recovery applied instantly, legacies Bismuth (+45% all elemental resistances), Sulphur (60% increased Damage, consecrated ground while stationary), Diamond (75% increased critical hit chance), Silver (30% increased Skill Speed), each 36% stronger per duplicate legacy. Legacies are always on (confirmed in game). Resistances stay capped without Sorrow Locket's 43 / 34 / 52. About x1.29–1.42 on Comet and x1.37 on Arc over Sorrow Locket (estimate; Comet's range depends on whether its built-in +1 s cast time scales with cast speed). Loses Sorrow Locket's +65 mana. Movement speed is to come from +30% boots instead of a Quicksilver legacy.
- **Rift Rosary** (Bloodstone Amulet) — +3 to Level of all Spell Skills, 25% spell damage, 36% mana regen, 28% global defences, +32 life, +140 accuracy, +26 Strength.
- **Woe Hold** (Sapphire Ring) — Cold 20% (implicit), 21% spell damage, 21% cast speed, 60% mana regen, 15% spell mana cost efficiency, 7 mana per kill.
- **Mind Twirl** (Topaz Ring, replaced Vortex Eye by 2026-10-07) — Lightning 22% (implicit), 33% spell damage, 24% cast speed, 82% mana regen, 26% spell mana cost efficiency (poe.ninja five-line view; check for hidden lines). With Woe Hold the spell mana cost efficiency total is 41%.
- Jewels: **Heart of the Well** (unique Diamond: 10% of Damage as Extra Cold, 8% crit chance, 8% mana regen, 59% increased ES from body armour), **Honour Bliss** (13% crit spell damage bonus, 14% faster start of ES recharge, meta skill energy, triggered spell damage) and **Soul Wisdom** (13% spell damage, 17% maximum ES, 4% cast speed, 22% chill duration).
- Flasks: Ultimate Life Flask, Lavianga's Spirits (constant mana flask). Charms: Antidote, Staunching, Thawing.

## Snapshot

PoB, level 94, 2026-10-05 (Sorrow Locket and Vortex Eye still equipped, Gelid set):

- Comet: 123,316 DPS, 174,536 average hit, 32.89% crit, enemy at 50% resistances
- ES 7,902, life 1,336, PoB EHP 17,787 (poe.ninja reports 30,023)
- Mana 972 with 0% increased maximum mana, 305/s regeneration; Comet costs 711 per cast, 220/s
- Resistances: Fire 105 / Cold 125 / Lightning 101 before the cap, Chaos 7%

In game after Mageblood + Mind Twirl (2026-10-07): 904 mana and 292/s on the Gelid set, about 1,037 mana on the Ghoul Weaver set. With 41% spell mana cost efficiency, Comet leaves roughly 86–103/s for other skills (estimate). Resistances capped, Chaos 0%.

## Open points

- **Defence direction: Chaos Inoculation + pure ES, decided 2026-09-16.** Same shape as last season's Chronomancer. ES is already about 7,900, so CI is closer than when it was decided. Ranked list: chest base first, then Melding / Ancient Aegis / a stun-threshold notable. CI-specific traps: life-based stun, ES-bypass nodes. Chaos resistance is 0% until then.
- **Boots.** Replace Maelstrom Urge with +30% movement speed boots. Its Cold 37% / Fire 34% and the glacial rune's 18% cold go with it; the post-Mageblood buffer is about Fire +32 / Cold +61, so this fits.
- **One staff for both sets.** An empty weapon set uses the other set's weapon (per the user), so a single staff with +7 or more to all spell levels could replace both and keep the per-element passive split. Shopping for one stays open; mana regeneration on it is not required.
- **Arc's mana cost** is not in the PoB export (only the main skill's stats are), so Arc's sustain under Silver is unchecked. Read the mana cost and cast time from the in-game skill tooltip on weapon set 2.
- **Mana regeneration: intentional or leftover?** The import reports 13 mana-regeneration smalls. Two reported ascendancy nodes reward spending and recovering mana fast (Archon of the Storm after spending 100% of maximum mana, Force of Will scaling with missing mana) and Arc runs Mana Flare, so this may be deliberate cycling fuel rather than leveling residue. Needs the user's confirmation before any respec is proposed.

## Working notes

- The MCP tree data cannot be trusted for identifying a specific node — see the caveat in Passive tree, and the same conclusions recorded in `runes_of_aldur/chronomancer/README.md`.
- Never hand-compute damage: use `calculate_character_dps`. It does not model supports, infusions or Comet's flat +1 s cast time, so treat its output as ratios between gear options, not as a PoB-comparable DPS.
- `pob_status` reports PoB not installed and the bridge addon not deployed, and the user is on macOS, so `pob_get_calcs` is not an option.
