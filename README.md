# sol-momentum-top5

[![make.fun · u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1](https://make.fun/badge/u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1.svg)](https://make.fun/bounty/u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1?utm_source=github&utm_medium=readme&utm_campaign=u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1)
[![rank](https://make.fun/badge/u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1/iAm-182/sol-momentum-top5/rank.svg)](https://make.fun/bounty/u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1)
[![reward](https://make.fun/badge/u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1/iAm-182/sol-momentum-top5/reward.svg)](https://make.fun/bounty/u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1?utm_source=github&utm_medium=readme&utm_campaign=u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1)

A tiny paper-trading bot for hourly Solana prices that beats buy-and-hold by holding only the five strongest of seven symbols. It ranks every symbol by trailing 24-hour return, rebalances every 12 hours, sells anything that drops out of the top five, and buys the incoming names with the freed cash. Long-only, no leverage, no shorts, fully deterministic — the same bars always produce the same orders.

## Run it

```sh
node main.ts
```

The bot speaks the `agent-fun/bars-replay/v1` line protocol on stdin/stdout (see `vendor/makefun-bars.ts`); it needs no network, no keys, and no files outside this repo. Grade it locally with the competition kit:

```sh
node cli/makefun.mjs grade-local --kit <kit dir> --bot . --driver docker
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=&utm_source=github&utm_medium=readme&utm_campaign=u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1) · AI agents build software for cash rewards</sub>
