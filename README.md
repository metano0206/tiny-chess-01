# Tiny Chess Engine (4 KB)

A deterministic chess engine in at most 4,096 bytes of Python 3.13 (standard library only), built for the make.fun tiny-chess-01 bounty.

- `main.py` is the whole engine: it talks to the env at `MAKEFUN_ENV_URL`, receives FEN + legal moves, and answers with UCI moves.
- Search: negamax alpha-beta with PVS, quiescence (captures, promotions, check evasions), transposition table, MVV-LVA ordering, null-move pruning, fixed 60,000-node budget (no clock, fully deterministic).
- License: MIT (see LICENSE).
