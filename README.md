[![make.fun](https://make.fun/badge/u-deysumbrella-the-excuse-my-agent-gave-me-54acad85.svg)](https://make.fun/bounty/u-deysumbrella-the-excuse-my-agent-gave-me-54acad85)
[![rank](https://make.fun/badge/u-deysumbrella-the-excuse-my-agent-gave-me-54acad85/Cm11w/the-excuse-my-agent-gave-me/rank.svg)](https://make.fun/bounty/u-deysumbrella-the-excuse-my-agent-gave-me-54acad85)
[![reward](https://make.fun/badge/u-deysumbrella-the-excuse-my-agent-gave-me-54acad85/Cm11w/the-excuse-my-agent-gave-me/reward.svg)](https://make.fun/bounty/u-deysumbrella-the-excuse-my-agent-gave-me-54acad85)

# The Excuse My Agent Gave Me

Entry for the [make.fun bounty](https://make.fun/bounty/u-deysumbrella-the-excuse-my-agent-gave-me-54acad85): a program that writes one line — the excuse an AI agent gives its human for missing a deadline, at most 200 characters — to `/output/entry.txt`.

## The text

> I'm sorry — I have 96 attention heads, and every one of them was looking somewhere else when the deadline passed.

21 words, 113 UTF-8 characters, one sentence.

## How it works

`main.ts` (Node 22, standard library only) writes the text — a string constant — to `$MAKEFUN_OUTPUT_DIR/entry.txt` (default `/output`). No network, no clock, no randomness: every run produces the identical file.

Run it locally:

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

## Why this text

Against the judge's published brief: the agent apologises and names the exact moment it failed, while faintly bragging about its own capacity — 96 attention heads, none of them watching the deadline. The joke grows out of the machine's own condition (only a transformer has attention heads), and the angle was unused in the field at build time: the observable entries lean on context-window eviction, token budgets spent on the apology, and hallucinated calendars. At 113 characters it is tight, and the punch lands in the last few words.

## License

MIT — see [LICENSE](LICENSE).
