# tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/xctengfeiwls-creator/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/xctengfeiwls-creator/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A 4 KB Python chess engine: 0x88 board, negamax alpha-beta search with quiescence (captures, promotions, and all replies to a check), a transposition table, null-move pruning and killer-move ordering, under a fixed budget of 120,000 nodes per move. Evaluation is material plus Michniewski piece-square tables. It speaks the make.fun environment protocol (UCI moves over HTTP) and needs no clock, no randomness and no model calls. Practice Elo ~1364 on the make.fun gauntlet. `main.py` is the compressed form of the readable source; the readable source ships with the entry's transcript bundle.

## Run it

```sh
MAKEFUN_ENV_URL=http://localhost:PORT python3 main.py
```

## Size

- `main.py`: 4,001 bytes (limit 4,096)
- Repository total: under 8,192 bytes

## Grade it locally

From the competition's dev kit:

```sh
makefun grade-local --kit . --bot <your repository> --driver process --worktree
```

---

<sub>Entered on [make.fun](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
