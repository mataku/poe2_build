# poe2_build

A personal workspace for thinking through Path of Exile 2 (PoE2) builds. This is not a repository for application source code — it is where build ideas, passive trees, skill setups, and gear notes are collected as raw material for thinking.

Files sitting in this repository are work-in-progress fragments and do not describe the repository's purpose. Unless told otherwise, there is no need to read them.

## Assumptions

- Target is **Season 0.5 "Runes of Aldur"**. Reason from this season's mechanics and balance
- Purpose is **endgame**. Not league start or leveling — builds are meant for running maps and endgame content

## My characters

Background on the characters played this season lives under `runes_of_aldur/`, one directory per character. There is no need to read these every session; read the relevant `README.md` when that character comes up.

- Chronomancer → `runes_of_aldur/chronomancer/README.md`
- Spirit Walker → `runes_of_aldur/spiritwalker/README.md`

Open decisions — "is this weapon worth buying", gear shortlists, budget splits — go in `runes_of_aldur/{character}/considering/`. That directory is gitignored and stays local, because those notes carry prices and budgets that go stale as soon as something is bought. Write new deliberation notes there, not next to the `README.md`. When a decision lands, fold the conclusion into the character's `README.md`.

## What happens in this repository

- Comparing and evaluating build ideas (skills, support gems, ascendancies, passive tree routing)
- Working out gear and mod setups, and balancing required stats / resistance caps
- Reading build data pulled from poe.ninja or Path of Building (PoB)
- Notes from investigating in-game mechanics

Writing code is essentially never the task. What is wanted is research, calculation, comparison, and recommendations.

## Use the PoE2 MCP first

This session has the `mcp__poe2__*` MCP tools connected. For any question about PoE2 game data (skill/support gems, passive nodes, keystones, base items, mods, formulas, mechanics, trade prices, etc.), **always verify with the MCP tools** rather than relying on memory or web search. PoE2 changes frequently — treat training data as outdated.

Commonly used:

- Research: `explain_mechanic`, `get_formula`, `inspect_spell_gem`, `inspect_support_gem`, `inspect_passive_node`, `inspect_keystone`, `inspect_mod`, `inspect_base_item`
- Discovery: `list_all_*`, `search_mods_by_stat`, `find_stat_sources`, `search_items`, `search_trade_items`
- Builds: `import_pob`, `export_pob`, `import_poe_ninja_url`, `analyze_character`, `analyze_passive_tree`, `calculate_character_dps`, `validate_build_constraints`, `validate_support_combination`, `compare_to_top_players`
- Data freshness: if a number looks wrong, check `check_tree_freshness` / `check_for_updates`

When presenting numbers (damage, resistances, ES/life, resistance caps, etc.), state explicitly whether the value came from the MCP or is an estimate. Never invent numbers.

## How to work

- Respond in Japanese. In-game terminology mixes Japanese client wording with English, so pairing them on first mention — e.g. 「アイスノヴァ (Ice Nova)」 — reads better
- For build proposals, be concise and ordered: conclusion (what to take) → reasoning → trade-offs. Prefer giving one recommendation and then touching on alternatives, over enumerating every option
- If budget or playstyle assumptions are unknown and would change the conclusion, ask. Otherwise proceed on reasonable assumptions and state them explicitly
