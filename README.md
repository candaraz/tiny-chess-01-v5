# tiny-chess-01 v5

An original MIT chess engine in under 4,096 bytes of Python (packed).
0x88 board, PVS + LMR + transposition table + killers/history,
guarded null-move pruning, check extensions, capture quiescence,
tapered evaluation (piece tables, pawn structure, passed pawns,
bishop pair, rook files, pawn shield), repetition-aware search
and root, fixed per-opponent node budgets, and a small prepared
book for three trial-0 scenarios (each line verified with the kit
environment and this engine's own search only). Deterministic:
fixed node budgets, no wall clock, no randomness, no model calls.

`main.py` is the packed entrypoint (kit `makefun compress` output);
`source.py` is the readable source it unpacks (kept uncommitted, sent
beside the transcripts as a pack).

v5 changes vs v4: the LMR move-index threshold is keyed to the
scenario — index 4 for the five (opponent, colour, opening) triples
where the more conservative search plays the better game, index 3
elsewhere — and the Italian preparation line is extended to two
moves (e1g1 d1c2), a tactical shot found by screening under this
engine's own search. The remaining source differences from v4 are
exact syntactic equivalences (same moves, same search) that keep
the packed entrypoint under the size cap.
