# Chronomancer — matachro

Cold CoC Comet, Chaos Inoculation / Energy Shield. Season 0.5 "Runes of Aldur", endgame mapping.

- Character: `matachro` (Sorceress / Chronomancer)
- Profile: https://poe.ninja/poe2/profile/matakuchan-0487/runesofaldur/character/matachro

## Core concept

Crit-fishing with cheap, fast cold projectile spells to drive **Cast on Critical → Comet** as the real damage source. Frostbolt and Frost Darts are the trigger layer, not the payload; Comet does the killing. Ice Nova is the secondary cold layer (cast on Frostbolt projectiles). Defence is pure ES under CI — no life at all, so all mitigation and recovery decisions run through ES recharge rather than leech or regen.

**Single weapon set, all cold (2026-08).** The Pain Mast swap and the Spark layer it carried are dropped. That simplifies the build, at the cost of Sigil of Power — see Open points.

## Axis

| Axis | Choice |
| --- | --- |
| Payload | Comet (via Cast on Critical) |
| Trigger | Frostbolt, Frost Darts |
| Secondary | Ice Nova |
| Defence | Chaos Inoculation + Energy Shield |
| Damage scaling | Spell crit → cold damage → crit damage bonus |
| Ascendancy | Chronomancer (Time Freeze / Time Snap / cooldown manipulation) |

## Key skill setups

- **Cast on Critical** — Comet + Elemental Focus + Rapid Casting + Living Bomb
- **Frostbolt** — Projectile Acceleration + Multishot + Cold Attunement + Rapid Casting + Cold Mastery
- **Frost Darts** — Considered Casting + Elemental Focus + Rapid Casting + Trickster's Shard + Deliberation
- **Ice Nova** — Rapid Casting + Magnified Area + Ice Bite + Deep Freeze + Cold Mastery
- **Comet (self-cast)** — Rapid Casting + Spell Echo + Elemental Focus + Unleash + Cold Mastery
- Utility: Frost Bomb, Elemental Weakness (Ritualistic Curse), Mana Remnants

## Passive tree

Keystone: **Chaos Inoculation** (max life 1, immune to chaos and bleed).

Ascendancy notables taken: **Ultimate Command** (grants Time Freeze), **Unbound Encore** (grants Time Snap), **Now and Again** (33% chance to not consume a cooldown), **The Rapid River** (recoup over 4s).

Main clusters:

- **Crit** — Controlling Magic, Critical Overload, Sudden Escalation, Careful Assassin, Critical Exploit, True Strike
- **ES** — Melding, Pure Energy, Dampening Shield, Insightfulness, Rapid Recharge, Refocus
- **Cold / elemental** — Glaciation, Endless Blizzard, Elemental Force, Raw Power, Turn the Clock Forward
- **Mana sustain** — Efficient Casting, Open Mind, Mana Blessing, Arcane Blossom

Mana sustain is a real tree investment, not an afterthought — the CoC loop is cast-speed bound and mana hungry.

## Gear axis

- **Empyrean Song** (Ashen Staff, bought 2026-08 for 480 div) — the main hand. Prefixes: **210% increased Spell Damage** (T8 *Runic*), Gain 53% as Extra Cold, Gain 56% as Extra Lightning. Suffixes: +7 to all Cold Spell Skills (capped), 101% spell crit (*of Unmaking*), 43% cast speed with 14% of Elemental Damage as Extra Cold. Implicit grants Level 18 Firebolt, which is not used. Two rune sockets, and it is worth **+12% mapping / +31% boss** over the Dusk Pole it replaced.

  The structural change from the Dusk Pole is trading a third gain-as-extra prefix for the T8 increased-spell-damage prefix. Base damage is still the larger multiplier, but at a 465% cold bucket that one prefix beats a fourth stacked gain-as-extra.

  Runes: socket 1 holds **Forged by the Breath of Aldur**, which is **socket-bound and cannot be removed** — it reads the staff's Extra Lightning prefix as Extra Cold while it stays socketed (x1.042, since cold also collects the cold-specific bucket). Socket 2 holds **+1 to Level of all Spell Skills** and should stay there; see the damage model below for why a projectile rune loses to it.

- **Maligaro's Virtuosity** — crit chance and cast speed on gloves. Its 87% increased Evasion Rating is dead weight here.
- **Lavianga's Spirits** — mana flask, permanent effect rather than on-use.
- **Doom Shroud** (Vile Robe, 1,130 ES) — about **61% of the whole energy shield pool**, once the ~320% global increased ES and Heart of the Well's body-armour-only 55% are applied. Corrupted, so it can never be improved, and one suffix ("58% reduced Duration of Bleeding on You") is dead under CI. Replace only as a strict upgrade.
- Rings/amulet carry mana, spell damage, cast speed, crit, and the resistance balance.
- Helm and boots are pure ES with hybrid defence runes.
- Retired: **Dusk Pole** (Sanctified Staff) — three gain-as-extra prefixes (53% fire / 54% lightning / 51% cold) stacking the base hit to 2.58x, +7 to all Cold Spell Skills, 102% spell crit, 47% cast speed.

## Damage model

The numbers that keep coming back, so they do not have to be re-derived. All MCP-verified against `data-v0.5.0-r12`.

- **Gem levels are the dominant multiplier.** Measured with `calculate_character_dps` on Comet, holding everything else fixed: level 30 -> 3,963 base damage, level 31 -> 4,567.5. That is **x1.1525 per level**, and it does not decelerate much past the gem's natural max of 20. The staff's `+7 to all Cold Spell Skills` alone is therefore about **x2.75**. Comet's effective level is around 30 — gem 19, +7 staff, +3 amulet, +1 rune.
- **Gain as Extra multiplies, increased dilutes.** Gain-as-extra adds to base damage, so it scales the entire increased bucket — but each additional one is diluted by the ones already stacked. Increased Spell Damage is additive into a single bucket, currently ~465% generic with a further 100% cold-specific.
- **At this build's numbers those two cross over.** A T8 209–238% increased-spell-damage prefix beats a fourth stacked gain-as-extra roll. It did not at the Dusk Pole's numbers, which is why the old staff carried three gain-as-extra prefixes instead.
- **Projectiles are a mapping-only stat.** Cast on Critical gains energy per critical *hit* scaled by monster power (`cast_on_crit_gain_X_centienergy_per_monster_power_on_crit`), and triggers at maximum energy. More projectiles mean more crit hits against a pack and nothing against a single target, where the spread misses. Cast on Critical has no `spell` tag, so `+X to Level of all Spell Skills` does not raise it.
- **Two-hand roughly doubles every relevant mod cap** over one-hand: spell damage 209–238% vs 90–104%, gain-as-extra 55–60% vs 28–30%, cold skill levels +7 vs +5, spell crit 90–109% vs 60–73%. A wand plus focus lands around −20–30% and cannot carry a gain-as-extra prefix at staff magnitude.

## Snapshot (poe.ninja, level 89)

Values below come from the PoE2 MCP import of the profile, not from PoB.

- Life + ES pool: 8,831 (life is 1 under CI, so effectively all ES)
- Effective HP: 28,814
- Resistances: Fire 75% / Cold 75% / Lightning 75% / Chaos 100% (CI)
- DPS: not reported by the import — needs PoB for a real number

## Investigations

Working notes live under `considering/`, which is gitignored and local-only.

- `considering/weapons.md` — **closed.** What the Empyrean Song beat, what dropping weapon set 2 cost, and the reusable trade search spec.
- `considering/defence.md` — **the live decision.** Why T15 maps kill this character and what fixes it, in cost order.

## Open points

- **Storm Driven is one node away.** Taking it moves elemental-damage-to-ES recoup from 9% to 24% for a single passive point. There is no dead node to fund it from, so the point has to come from somewhere — the six Mana Regeneration smalls are the documented over-investment. Details in `considering/defence.md`.
- The respec that bought the three Energy Shield Recoup smalls paid for it with Rapid Recharge and an Energy Shield Delay small, so **faster start of Energy Shield Recharge went 40% -> 0%**. Buy it back on gear (*of Anticipation*, 51–55% on one suffix) rather than re-specing into it — the tree is the only dense source of recoup, and gear is the cheap source of delay reduction.
- **Sigil of Power is gone with the weapon swap, and it was large.** At gem level 19 it gives roughly 13–14% *more* spell damage per stage to a maximum of 4 stages — on the order of **x1.5 or better while standing in it**, which dwarfs the entire staff upgrade. Uptime was always partial while mapping (10s duration, 10s cooldown, a 30-radius circle, stages bought with mana) but near-full on a boss. The only way to keep it on one weapon set is a **Chiming Staff** main hand, whose implicit grants it. Worth deciding deliberately rather than by default.
- The tree's lightning nodes are dead now that Spark is gone, but **they do not turn into a spare point.** The weapon-set system only divides already-allocated passives between the two sets; there is no separate set-2 allotment to fold back into set 1.
- Crit chance on the trigger skills is the main lever for CoC uptime — worth checking whether Frost Darts or Frostbolt is actually driving more triggers.
- **Resolved:** an item-granted Sigil of Power *does* take support gems — it ran with Cooldown Recovery II and Magnified Area II off the Pain Mast implicit. So a Chiming Staff main hand would carry it fully supported.

## Working notes

- poe.ninja's import caps every item at **five displayed lines**, and rune lines eat that budget. Always use a PoB export for gear comparisons.
- Never hand-compute damage: use `calculate_character_dps`. A remembered Path of Exile 1 constant for gem-level scaling (x1.04 against the measured x1.1525) once reversed a rune recommendation.
- **The MCP's passive tree data cannot be trusted for identifying a specific node.** Its coordinates are group-level rather than per-node, the 2026-08-23 import reported 11 of 128 allocated nodes absent from `tree.json`, and it resolved node 54194 to a "Life Recoup" small that does not exist on this tree at all. Node names and stats need in-game confirmation before acting on them.
- There is no rune or soul-core data in the MCP at all. Every rune value here came from in-game text.
