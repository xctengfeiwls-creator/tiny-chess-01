# tiny-chess-01 entry

A 4 KB Python chess engine for make.fun's tiny-chess-01 bounty.

## Engine

- 0x88 board, negamax alpha-beta with quiescence search (captures,
  promotions, and all replies to a check)
- Transposition table, null-move pruning, killer moves + MVV-LVA ordering
- Evaluation: material + Michniewski piece-square tables
- Deterministic: iterative deepening under a fixed node budget
  (120,000 nodes per move) — no clock, no unseeded randomness
- `main.py` is the compressed form of the readable source; the readable
  source ships with the entry's transcript bundle

## Size

- `main.py`: 4,001 bytes (limit 4,096)
- Repository total: about 6.4 KB (limit 8,192)

## Grade it locally

From the competition's dev kit:

    makefun grade-local --kit . --bot <your repository> --driver process --worktree
