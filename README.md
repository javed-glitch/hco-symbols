# hco-symbols
The single list of symbols the HCO tools watch. Data only: no scripts, no jobs.

Each entry in `symbols.json`:
- `sym` display ticker (also the key used by the cycle bot)
- `group` one of `groups` (controls order and tag on Price Movement)
- `ccy` currency symbol shown (`$` or `£`)
- `yahoo` Yahoo ticker if it differs from `sym` (London ETFs use `.L`)
- `pence` true if Yahoo quotes in pence
- `feeds` which tools use the symbol: `pm` (Price Movement page), `cycle` (market-scan cycle bot). Each tool takes its own subset, in file order. A missing `feeds` means `pm` only.

No holdings, quantities or prices belong here. Adding a symbol gives it a row on Price Movement;
prices, targets and cycle stage appear once the producing tool covers it.
