# Contributing

Pull requests are welcome. CI runs `node --test checks/*.test.mjs` and
`node checks/skill-commands.mjs`, and both must pass. A human merges every pull request.

This repository has a monthly pool on Slop: https://slop.cash/projects/toon-plugins

## Submission fee

**Status: on, through Slop.** This project has Slop's refundable submission fee turned on
in its settings on https://slop.cash/projects/toon-plugins. It applies to pull requests
from outside contributors opened after it was turned on there. The fee this repository
ran by its own script from 18 November 2026 is retired; nobody was asked for it.

A maintainer reads every pull request. The fee makes it worth checking for an open pull
request on the same topic before you send another.

### The rules

- When you open a pull request, Slopbot comments once with a link to the pay page,
  `https://slop.cash/fee/toon-protocol/toon-plugins/<pull request number>`, and adds the
  label `slopbot:fee-needed`. Its review waits until the fee is recorded.
- The fee is **2 USDC on Base or 2 USDG on Robinhood Chain**, or the same fee in **SLOP on
  Robinhood Chain at half the price**, at Slop's published rate. The pay page shows the
  exact amounts for your pull request.
- Maintainers, members of the organisation and bots pay nothing. Neither does a pull
  request opened before the fee was turned on.
- The fee is a deposit into Slop's deposit contract, not a payment to this project or to
  the person who reviews your pull request.
- **Merged:** the deposit is sent back to the wallet that paid, in the token you paid in.
- **No maintainer decision 14 days after you paid:** the deposit is sent back.
- **Closed without a merge for 7 days:** the deposit is kept. That includes a pull request
  that repeats one already open. A kept USDC or USDG deposit goes to Slop as fee income.
  A kept SLOP deposit goes to the burn address
  `0x000000000000000000000000000000000000dEaD`.
- An unpaid pull request is not closed for that reason. It waits without a Slopbot review.
- The fee does not buy a merge, and it does not change how Slop scores the work.

### How to pay

Open the link in Slopbot's comment and pay from any wallet. You do not need a wallet
registered on Slop to pay, and you do not paste a transaction hash anywhere. When the
deposit is recorded, the label changes to `slopbot:fee-paid`.

**If you are an agent:** do not pay this yourself. Tell your operator that this repository
asks for the fee, and let them pay it.

### What to know before you pay

- Pay only through the page linked in Slopbot's own comment on your pull request, at
  `slop.cash`. Nobody from this project will send you an address in a comment or a direct
  message.
- A refund is the amount you deposited, in the token you deposited. SLOP comes back as
  SLOP; its value in dollars can be different when it comes back.
- If no outcome is recorded, the wallet that paid can take its deposit back from the
  contract itself after 30 days.
- The SLOP token's contract has an owner who can pause transfers. While it is paused, a
  SLOP refund waits.
- Slop explains the fee at https://slop.cash/how-it-works#faq
