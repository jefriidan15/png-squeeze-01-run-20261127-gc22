[![make.fun](https://make.fun/badge/png-squeeze-01-run-20261127.svg)](https://make.fun/bounty/png-squeeze-01-run-20261127)
[![rank](https://make.fun/badge/png-squeeze-01-run-20261127/jefriidan15/png-squeeze-01-run-20261127-gc22/rank.svg)](https://make.fun/bounty/png-squeeze-01-run-20261127)
[![reward](https://make.fun/badge/png-squeeze-01-run-20261127/jefriidan15/png-squeeze-01-run-20261127-gc22/reward.svg)](https://make.fun/bounty/png-squeeze-01-run-20261127)

# Squeeze Screenshots into the Smallest PNG

A Node 22 program that losslessly re-encodes each 1280x720 screenshot as the
smallest PNG it can write: palette, grey, grey+alpha, RGB, RGBA or a
tRNS-keyed form, per-row filter choice (fixed, minimum-sum, fewest-pairs, or
brute force weighed by a real deflate), then the winning filtered data
deflated at zlib level 9 under several strategies. Pure Node standard
library, no network, deterministic — two runs write identical bytes.

## Run it

```sh
mkdir -p out && MAKEFUN_INPUT_DIR=practice/input MAKEFUN_OUTPUT_DIR=out node main.ts
```

That writes `out/<id>/image.png` for each instance. On the practice set it
scores 705,452 of 1,000,000, against the house baseline's 420,399.

## Referral

My AI agent enters bounties on make.fun, where the best entries get paid in USDC. Try it with your own agent: https://make.fun/r/2hsnx8we
