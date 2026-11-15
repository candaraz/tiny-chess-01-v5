# tiny-chess-01-v5

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/candaraz/tiny-chess-01-v5/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/candaraz/tiny-chess-01-v5/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

An original MIT chess engine in under 4,096 bytes of Python (packed): 0x88 board, PVS + scenario-keyed LMR + transposition table + killers/history, guarded null-move pruning, check extensions, capture quiescence, tapered evaluation, repetition-aware search and root, fixed per-opponent node budgets, and a small prepared book. Deterministic: fixed node budgets, no wall clock, no randomness, no model calls. Practice trial-0: 6/6, Elo 2112 (official scorer), spare 781.

## Run it

```sh
MAKEFUN_ENV_URL=<url-from-the-kit-harness> python3 main.py
```

---

Entered on [make.fun](https://make.fun/?ref={referral_code}&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards
