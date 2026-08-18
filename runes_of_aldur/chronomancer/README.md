# Chronomancer — matachro

Cold CoC Comet, Chaos Inoculation / Energy Shield. Season 0.5 "Runes of Aldur", endgame mapping.

- Character: `matachro` (Sorceress / Chronomancer)
- Profile: https://poe.ninja/poe2/profile/matakuchan-0487/runesofaldur/character/matachro

## Core concept

Crit-fishing with cheap, fast cold projectile spells to drive **Cast on Critical → Comet** as the real damage source. Frostbolt and Frost Darts are the trigger layer, not the payload; Comet does the killing. Ice Nova is the secondary cold layer (cast on Frostbolt projectiles). Defence is pure ES under CI — no life at all, so all mitigation and recovery decisions run through ES recharge rather than leech or regen.

## Axis

| Axis | Choice |
| --- | --- |
| Payload | Comet (via Cast on Critical) |
| Trigger | Frostbolt, Frost Darts |
| Secondary | Ice Nova, Spark |
| Defence | Chaos Inoculation + Energy Shield |
| Damage scaling | Spell crit → cold damage → crit damage bonus |
| Ascendancy | Chronomancer (Time Freeze / Time Snap / cooldown manipulation) |

## Key skill setups

- **Cast on Critical** — Comet + Elemental Focus + Rapid Casting + Living Bomb
- **Frostbolt** — Projectile Acceleration + Multishot + Cold Attunement + Rapid Casting + Cold Mastery
- **Frost Darts** — Considered Casting + Elemental Focus + Rapid Casting + Trickster's Shard + Deliberation
- **Ice Nova** — Rapid Casting + Magnified Area + Ice Bite + Deep Freeze + Cold Mastery
- **Comet (self-cast)** — Rapid Casting + Spell Echo + Elemental Focus + Unleash + Cold Mastery
- Utility: Sigil of Power (weapon-swap cast), Frost Bomb, Consecrate, Elemental Weakness (Ritualistic Curse), Mana Remnants, Spark

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

- **Dusk Pole** (Sanctified Staff) — three gain-as-extra prefixes (53% fire / 54% lightning / 51% cold) stack the base hit to 2.58x, on top of +7 to all Cold Spell Skills, 102% spell crit and 47% cast speed. Runes add +1 to all Spell Skills and 25% chance to fire 2 additional projectiles. Base damage and gem levels are the multipliers here, not increased damage.
- Weapon swap: **Pain Mast** (Chiming Staff) for casting Sigil of Power / buffs.
- **Maligaro's Virtuosity** — crit chance and cast speed on gloves.
- **Lavianga's Spirits** — mana flask, permanent effect rather than on-use.
- Rings/amulet carry mana, spell damage, cast speed, crit, and the resistance balance.
- Body/helm/boots are pure ES with hybrid defence runes.

## Snapshot (poe.ninja, level 89)

Values below come from the PoE2 MCP import of the profile, not from PoB.

- Life + ES pool: 8,831 (life is 1 under CI, so effectively all ES)
- Effective HP: 28,814
- Resistances: Fire 75% / Cold 75% / Lightning 75% / Chaos 100% (CI)
- DPS: not reported by the import — needs PoB for a real number

## Investigations

- [staff_upgrade.md](staff_upgrade.md) — weapon shortlist, per-slot marginal values, trade search spec, why one-hand does not compete
- [defence.md](defence.md) — why T15 maps kill this character, and the recoup fix

## Open points

- Crit chance on the trigger skills is the main lever for CoC uptime — worth checking whether Frost Darts or Frostbolt is actually driving more triggers.
- Cast on Critical gains energy per critical *hit*, scaled by monster power (`cast_on_crit_gain_X_centienergy_per_monster_power_on_crit`). That makes projectile count a mapping stat and near-worthless on single targets, where the spread misses. Worth measuring rather than assuming.
- Whether an item-granted Sigil of Power can still take support gems — decides if a Chiming Staff base can retire the Pain Mast weapon swap without losing Magnified Area.
- poe.ninja's import caps every item at five displayed lines. Always use a PoB export for gear comparisons.
