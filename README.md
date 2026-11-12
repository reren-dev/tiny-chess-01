# tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/reren-dev/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/reren-dev/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

An ultra-compact 4 KB Python chess program utilizing 0x88 board representation, alpha-beta pruning, tapered PeSTO evaluation tables, transposition lookup, and quiescence search within a strict 100,000 node cap per turn. Achieved practice trial-0 Elo ~1,497 against the automated house benchmark.

## Architecture & Packing

The submission artifact `main.py` is exactly 4,087 bytes in size. It packs the complete chess engine via lzma compression and base85 encoding behind a clean two-line bootstrap loader (`import base64,lzma` and `exec(...)`). It runs autonomously without external model inference or wall-clock timing constraints.

## Trial Performance

Evaluated across the 16-game gauntlet suite, securing robust tactical performance (7 wins, 5 draws, 4 losses) with an average computation pace of 3.47 seconds per move. All games verified successfully.

## Execution

```sh
MAKEFUN_ENV_URL=http://localhost:8080 python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=dkjyzx8d&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards · Submission verified</sub>
