# Stormweaver — matites

Multi-element self-cast Sorceress, Energy Shield + life hybrid. Season 0.5.5 "Forbidden Rites", aimed at endgame mapping.

**Work in progress (last synced 2026-09-16, level 83).** The build is still being assembled — Comet (cold) and Arc (lightning) are both carrying damage supports, and the plan as of 2026-09-16 is to run them from separate weapon sets with an element-specific staff each. Nothing below is a settled plan; it is a record of where things stand so the next session can start from it.

- Character: `matites` (Sorceress / Stormweaver)
- Profile: https://poe.ninja/poe2/profile/matakuchan-0487/forbiddenrites/character/matites
- PoB: not stored — a PoB code goes stale with every gear swap or level-up, so ask for a fresh export each session instead of reading a saved one. Prefer it over the poe.ninja import for gear — poe.ninja caps every item at five displayed lines and rune lines eat that budget.

## Current state

What is observably true from the level 76 PoB export and the 2026-09-16 poe.ninja import:

| Axis | Now | Decided? |
| --- | --- | --- |
| Damage skills | Comet (Unleash + Spell Echo) and Arc (Unleash + Living Lightning) self-cast, Ice Nova secondary | Two mains, split by weapon set |
| Element | Cold (Comet, Ice Nova) on set 2, lightning (Arc) on set 1; staff Extra Fire rides on both | Yes, as of 2026-09-16 |
| Damage scaling | Spell crit chance (tree + Maligaro's) → spell damage → +8 spell levels (staff +5, amulet +3) | Partly |
| Defence | ES + life hybrid today; target is Chaos Inoculation + pure ES | Yes, as of 2026-09-16 |
| Ascendancy | Stormweaver (see Passive tree for the reported nodes) | Yes |

## Skill setups (poe.ninja, 2026-09-16)

- **Comet** (Lv17, 20% quality) — Elemental Focus + Rapid Casting II + Unleash + Spell Echo + Cold Mastery
- **Arc** (Lv16, 20%) — Unleash + Mana Flare + Rapid Casting II + Living Lightning II
- **Enervating Nova** (Lv17, from the staff implicit) — Lightning Mastery + Zenith I + Rapid Casting II. Electrocute tool, not a damage source.
- **Ice Nova** (Lv16) — Magnified Area II + Deep Freeze + Rapid Casting II + Freeze + Cold Mastery
- **Frost Bomb** (Lv16) — Magnified Area I + Cold Attunement + Cooldown Recovery I + Short Fuse I
- **Elemental Weakness** — Rapid Casting II + Burning Inscription
- **Orb of Storms** — Harmonic Remnants II
- **Siphon Elements** — Harmonic Remnants II
- **Mana Remnants** — Harmonic Remnants II + Mysticism II
- **Arctic Armour** — Freeze

No meta skill (Cast on Critical, Cast on Freeze, etc.) is slotted. The Honour Bliss jewel carries "Meta Skills gain 4% increased Energy" and "Triggered Spells deal 10% increased Spell Damage", which is the only hint of a trigger layer being planned.

## Passive tree

No keystone allocated.

Ascendancy nodes reported by the import — **unconfirmed**, because the MCP has no verifiable ascendancy data and `import_pob` returned an empty ascendancy list: **Constant Gale** (Arcane Surge), **Force of Will** (20% of damage taken from mana before life, Arcane Surge effect per missing mana), **Archon of the Storm** (Lightning Archon after spending 100% of maximum mana), **Refracted Infusion** (50% chance for a second Elemental Infusion).

Notables resolved by the import (119 points, 15 unresolved against the local tree):

- **Crit** — Controlling Magic, Critical Overload, Sudden Escalation
- **Spell / elemental** — Raw Power, Turn the Clock Forward, Elemental Force, Practiced Signs
- **Cold** — Glaciation, Endless Blizzard
- **Lightning** — Electric Amplification
- **ES** — Pure Energy, Patient Barrier
- **Mana** — Arcane Blossom, Open Mind, Ingenuity

Small nodes skew heavily toward mana regeneration (13 of them) and generic spell / elemental damage. Cold and lightning smalls are roughly even, which matches the undecided element. Two jewel sockets, both filled.

**Data caveat.** The local MCP tree is `data-v0.5.0-r12`. `check_tree_freshness` calls it current against poe.ninja's `PassiveTree-0.5` tag, but 15 of 119 allocated nodes did not resolve, the starting class came back as "Unknown", and the tree was reported as disconnected. Treat those as data artifacts of a 0.5.5 tree the local bundle predates, not as build problems, and confirm any specific node in game before acting on it.

## Gear (PoB for the level 76 items, poe.ninja for the 2026-09 changes)

Rune values below are from the PoB item text — the MCP has no rune or soul-core data.

- **Set 1 lightning staff** (Paralysing Staff, bought 2026-09-19, 35 div) — +7 to Level of all Lightning Spell Skills, 250% increased Spell Damage, 42% cast speed, Gain 56% as Extra Fire, 15% of Elemental as Extra Cold, +212 mana, 48% spell crit damage bonus (dead under Maligaro's). Rune socket holds a +1 to Level of all Spell Skills rune bonded with faster Archon cooldown. Implicit grants Level 18 Enervating Nova. About x2.29 on Arc over Kraken Goad; the cast speed carries most of that. Shopping rule that came out of it: levels, then gain-as-extra, then cast speed, then spell damage.
- **Kraken Goad** (Paralysing Staff, bought 2026-09-14, now the set 2 placeholder until the Chiming Staff is bought) — 166% increased Spell Damage, Gain 50% of Damage as Extra Fire, +5 to Level of all Spell Skills, 64% spell crit, +40 mana, 88% mana regen. Implicit grants Level 17 Enervating Nova. Two sockets filled, 60% increased Spell Damage from runes plus a dead Bonded armour-break line. Chosen over an otherwise equal +187-mana staff for the Extra Fire roll (about x1.13).
- Retired: **Corruption Chant** (Ashen Staff) — 164% spell damage, 46% Extra Lightning, +2 spell levels, 21% cast speed, Level 14 Firebolt implicit. The cast speed it carried was replaced by the two new rings.
- **Rift Cowl** (Skycrown Tiara, 296 ES) — +41 ES, 70% increased ES, +99 life, Fire 21% / Cold 32% / Lightning 28%. Rune: Greater Iron Rune (18% AES, bonded +20 life / +20 mana).
- **Kraken Shelter** (Vile Robe, 666 ES) — 103% and 40% increased ES, +28 ES, +82 life, Lightning 40% / Fire 32%, 27.8 life regen. Two Greater Iron Runes (36% AES, bonded +40 life / +40 mana).
- **Maligaro's Virtuosity** (Fine Bracers) — 27% increased Critical Hit Chance, Critical Damage Bonus fixed at 250%, crit chance cannot be rerolled. 69% evasion and attack speed are dead weight. Rune: Storm Rune (+14% Lightning Resistance).
- **Maelstrom Urge** (Luxurious Slippers, 202 ES) — 131% increased ES, +30 Intelligence, Cold 37% / Fire 34%, 20% movement speed, +71 stun threshold. Rune: Greater Glacial Rune (+18% Cold Resistance).
- **Mageblood** (bought 2026-10-07, 390 div, replaced Sorrow Locket) — two charm slots, 20% of flask recovery applied instantly, legacies Bismuth (+45% all elemental resistances), Sulphur (60% increased Damage, consecrated ground while stationary), Diamond (75% increased critical hit chance), Silver (30% increased Skill Speed), each 36% stronger per duplicate legacy. Legacies are always on (confirmed in game). Resistances stay capped without Sorrow Locket's 43 / 34 / 52 (Fire 107 / Cold 136 / Lightning 94, estimate). About x1.29–1.42 on Comet and x1.37 on Arc (estimate); loses Sorrow Locket's +65 mana, and Silver raises mana spend with cast rate. Mind Twirl's mana cost efficiency covers that: in game 904 mana and 292/s regeneration on the Gelid set, leaving roughly 86–103/s beyond Comet (estimate). Movement speed is to come from +30% boots instead of a Quicksilver legacy.
- **Rift Rosary** (Bloodstone Amulet) — +3 to Level of all Spell Skills, +32 life, 36% mana regen, +26 Strength. Replaced Hate Noose (+2 levels, +50 ES, 13% spell damage); poe.ninja shows five lines only, so the full mod list needs a PoB export.
- **Mind Twirl** (Topaz Ring, replaced Vortex Eye by 2026-10-07) — +22% Lightning Resistance (implicit), 33% spell damage, 24% cast speed, 82% mana regen, 26% spell mana cost efficiency (poe.ninja five-line view; check for hidden lines). With Woe Hold the spell mana cost efficiency total is 41%.
- **Woe Hold** (Sapphire Ring) — 21% spell damage, 21% cast speed, 60% mana regen, 15% mana cost efficiency, Cold 20%.
- Retired: Cataclysm Twirl and Pandemonium Gyre (leveling rings).
- Jewels: **Honour Bliss** (13% crit spell damage bonus, 14% faster start of ES recharge, meta skill energy, triggered spell damage) and **Soul Wisdom** (13% spell damage, 17% maximum ES, 4% cast speed, 22% chill duration).
- Flasks: Ultimate Life Flask, Transcendent Mana Flask. Charms: Antidote, Ruby, Staunching — all mana-recovery on trigger.

## Snapshot (poe.ninja, level 90, 2026-09-22)

Values below come from the PoE2 MCP import of the profile, not from PoB.

- Life + ES pool: 8,351
- Effective HP: 27,140 (18,463 at level 83, 15,724 at level 76)
- Resistances: Fire 75% / Cold 75% / Lightning 75% / **Chaos 7%**
- Passive points: 137 allocated, 15 unresolved against the local tree
- poe.ninja's own build score moved from C to A tier on this import
- Life + ES pool: not returned by this import
- DPS: not reported by the import — needs PoB for a real number

## Open points

- **Two-set staves.** Comet on a Chiming Staff (+7 cold, Sigil of Power) in set 2 and Arc on a +7 lightning staff in set 1 are under consideration.
- **Defence direction: Chaos Inoculation + pure ES, decided 2026-09-16.** Same shape as last season's Chronomancer. Current pool is roughly 2,900 ES (estimate), so the conversion is a multi-step project — ranked list: chest base first, then Melding / Ancient Aegis / a stun-threshold notable. CI-specific traps: life-based stun, ES-bypass nodes.
- **Chaos resistance is 7%** until CI lands; after that it is irrelevant and the Amethyst ring's suffix is freed.
- Belt, rings, body armour and amulet were all replaced during 2026-09. Nothing on the character is leveling-tier any more.
- **Trigger layer** hinted by the Honour Bliss jewel is not implemented — no meta gem slotted.
- **Mana regeneration: intentional or leftover?** The import reports 13 mana-regeneration smalls. Two reported ascendancy nodes reward spending and recovering mana fast (Archon of the Storm after spending 100% of maximum mana, Force of Will scaling with missing mana) and Arc runs Mana Flare, so this may be deliberate cycling fuel rather than leveling residue. Needs the user's confirmation before any respec is proposed.

## Working notes

- The MCP tree data cannot be trusted for identifying a specific node — see the caveat in Passive tree, and the same conclusions recorded in `runes_of_aldur/chronomancer/README.md`.
- Never hand-compute damage: use `calculate_character_dps`.
- `pob_status` reports PoB not installed and the bridge addon not deployed. Installing Path of Building 2 and running `pob_install_addon` would let `pob_get_calcs` return real DPS and pool numbers instead of the import's placeholders.
