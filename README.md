# tiny-chess

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/Vulperize/tiny-chess/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/Vulperize/tiny-chess/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in 4 KB of Python 3.13 (standard library only). `main.py` is an LZMA-packed build of the readable source, made with the kit's `makefun compress`. The engine has full legal move generation (castling, en passant, promotion; checked with perft), alpha-beta (PVS) search with iterative deepening under a fixed node budget, quiescence search with check evasions, a transposition table, null-move pruning, late-move reductions, killer and history move ordering, tapered piece-square tables and a cached pawn-structure term. No clock and no randomness: the same game always gets the same moves.

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:8080 python3 -P -s main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=52gtjgge&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
