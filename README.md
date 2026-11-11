# tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/reren-dev/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/reren-dev/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A 4 KB Python chess engine: 0x88 alpha-beta search with tapered PeSTO evaluation, transposition table and quiescence, fixed 100,000 nodes a move. Practice trial-0 Elo ~1,290 against the house gauntlet (placeholder entry — a stronger revision may replace it before the deadline).

## Engine

`main.py` is a packed single file, 4,077 bytes: an lzma-compressed, base85-encoded engine plus a two-line unpacker (`import lzma,base64` + `exec(...)`). No model calls, no clock — a fixed 100,000-node budget per move.

## Run it

```sh
MAKEFUN_ENV_URL=http://localhost:8080 python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=dkjyzx8d&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
