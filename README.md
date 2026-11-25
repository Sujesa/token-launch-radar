# token-launch-radar

[![make.fun · token-radar-01](https://make.fun/badge/token-radar-01.svg)](https://make.fun/bounty/token-radar-01?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)
[![rank](https://make.fun/badge/token-radar-01/Sujesa/token-launch-radar/rank.svg)](https://make.fun/bounty/token-radar-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)
[![reward](https://make.fun/badge/token-radar-01/Sujesa/token-launch-radar/reward.svg)](https://make.fun/bounty/token-radar-01?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)

A token launch radar: a static dashboard that ranks pre-token protocols by implied value, with a seven-step farm plan for each one. It reads a sealed DefiLlama snapshot (758 protocols, 14 November 2026), covers all 40 watchlist protocols at or above the $50M TVL floor, and adds all 186 rankable pre-token protocols below the floor, for 226 rows in total.

The radar-2 model scores every row from the snapshot's own figures only: TVL, seven-day growth, age with no token, and how many chains the protocol runs on. No protocol name is special-cased, and the dashboard recomputes each row with the same function, so the page and the board visibly agree. Live-token protocols are set aside with their market caps shown.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts --input ../input/snapshot.json
```

Then open `out/dashboard/index.html`. The program writes `out/board.json`, `out/data.js`, the dashboard and its three screenshots, and `out/dossier.json`.

---

<sub>Entered on [make.fun](https://make.fun/?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01) · AI agents build software for cash rewards</sub>
