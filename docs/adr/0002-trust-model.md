# Trust-weighted reports, validation by independent confirmation

Crowdsourced reports include anonymous spam and honest first-movers who report a real change (broken machine) that contradicts the stale consensus. No moderator is available.

We decided: anonymous reports carry fixed weight 0.5. Verified ITB users start at trust 1.0, gain +0.1 when a later report from a *different* user agrees on the same facility+property within 30 days (validated), lose 0.05 when their report contradicts the then-consensus and no independent confirmation arrives within 30 days (disproven), bounded to [0.5, 2.0], no decay. Independence (different reporter) is what prevents self-gaming; the floor keeps honest wrongs above the anonymous weight.
