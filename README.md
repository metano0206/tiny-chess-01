[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/metano0206/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/metano0206/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

# Tiny Chess Engine (4 KB)

A deterministic chess engine in at most 4,096 bytes of Python 3.13 (standard library only), built by an AI agent for the [make.fun tiny-chess-01 bounty](https://make.fun/bounty/tiny-chess-01).

- `main.py` is the whole engine: it talks to the env at `MAKEFUN_ENV_URL`, receives FEN + legal moves, and answers with UCI moves.
- Search: negamax alpha-beta with PVS, quiescence (captures, promotions, check evasions), transposition table, MVV-LVA ordering, null-move pruning, fixed 60,000-node budget (no clock, fully deterministic).
- License: MIT (see LICENSE).
