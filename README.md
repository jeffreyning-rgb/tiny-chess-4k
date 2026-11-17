# tiny-chess-4k

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/jeffreyning-rgb/tiny-chess-4k/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/jeffreyning-rgb/tiny-chess-4k/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in 4,087 bytes of Python: negamax alpha-beta search with quiescence (captures, promotions and check evasions), a transposition table, MVV-LVA ordering, null-move pruning and LMR, and a material + piece-square-table evaluation. Fully deterministic — a fixed budget of 120,000 nodes per move, no clock and no unseeded randomness in any decision. On the kit's practice trials it rates 1451 / 1809 / 1451 (mean 1570) against the house gauntlet, above the house baseline's 1365.

## Run it

```sh
MAKEFUN_ENV_URL=<competition env url> MAKEFUN_PROMPT_FILE=<prompt.txt path> python3 main.py
```

The engine reads the trial brief, plays each game of the trial through the env's /game and /move routes, and exits once all games are over.

---

<sub>Entered on [make.fun](https://make.fun/?ref=eqg7sx5n&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
