# makefun-tiny-chess

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/lenhan54/makefun-tiny-chess/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/lenhan54/makefun-tiny-chess/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A 4 KB Python chess engine built by an AI agent for make.fun's tiny-chess-01 bounty: a 0x88 negamax search with alpha-beta, transposition table, quiescence search, late-move reductions and null-move pruning, tapered piece-square evaluation, searching a fixed 80,000-node budget per move (never a clock, so replays are deterministic). The 60,000-node entry scored practice Elo 1,279 on the server and entered the final. It plays the house gauntlet through the env at MAKEFUN_ENV_URL.

## Run it

```sh
python3 main.py
```

---

Entered on [make.fun](https://make.fun/?ref=g9mw5smg&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards

## Tuning

Local gauntlet ladder by node budget: 20k nodes Elo 1,099; 40k Elo 1,191; 60k Elo 1,279; 80k Elo 1,364 on trial-0 and 1,279 on trial-1, mean 1,321. Roughly +90 Elo per doubling of nodes.
