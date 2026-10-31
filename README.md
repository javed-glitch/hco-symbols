# hco-symbols
The single list of symbols the HCO tools watch. Data only: no scripts, no jobs.

Each entry in `symbols.json`:
- `sym` display ticker (also the key used by the cycle bot)
- `group` one of `groups` (controls order and tag on Price Movement)
- `ccy` currency symbol shown (`$` or `£`)
- `yahoo` Yahoo ticker if it differs from `sym` (London ETFs use `.L`)
- `pence` true if Yahoo quotes in pence
- `etf` true for ETFs: the cycle bot shows them on their own page after the stocks
- `feeds` which producers use the symbol (`cycle` = cycle bot, `options` = Options Gravity board option cards; `pm` is informational). Price Movement shows EVERY symbol in this file; where a producer doesn't cover it yet, the page shows a Gap.

No holdings, quantities or prices belong here. Adding a symbol gives it a row on Price Movement;
prices, targets and cycle stage appear once the producing tool covers it.
