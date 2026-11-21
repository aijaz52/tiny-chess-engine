[![make.fun - tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/aijaz52/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/aijaz52/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

Entry for the [tiny-chess-01 bounty on make.fun](https://make.fun/bounty/tiny-chess-01).

`main.py` is the packed entry (makefun compress of `engine.py`): iterative
alpha-beta with aspiration windows, Zobrist transpositions, null-move pruning
(R=2), late quiet-move reductions, frontier futility pruning, and capture
quiescence with delta pruning. The 0x88 list board uses make/unmake, piece
sets, and precomputed move rays. Search is deterministic at 80,000 nodes
per move. Python 3.13, standard library only, at most 4,096 bytes committed.
`engine.py` is the readable source the entry is packed from.

Offline checks: `python3 bench.py --module main --count 40 --nodes 80000`.
The benchmark checks start-position perft(3)=8902 and Kiwipete perft(3)=97862
before timing 40 fixed middlegame positions. The source and benchmark are
local development files excluded from the submitted snapshot.
