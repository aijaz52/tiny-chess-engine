# tiny-chess-engine

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/aijaz52/tiny-chess-engine/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/aijaz52/tiny-chess-engine/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in at most 4,096 bytes of Python (`main.py`, Python 3.13 standard library only, fully deterministic: node-budgeted iterative-deepening alpha-beta with aspiration windows, null-move pruning, LMR, quiescence with delta pruning, a zobrist transposition table and lzma-packed piece-square tables). It plays the house gauntlet through the env at `MAKEFUN_ENV_URL`, one game after another, and exits when every game is done.

## Run it

```sh
MAKEFUN_ENV_URL=http://localhost:8080 python3 -P -s main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=bsdfw3nf&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
