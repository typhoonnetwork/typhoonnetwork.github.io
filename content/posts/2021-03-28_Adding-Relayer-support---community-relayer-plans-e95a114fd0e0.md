---
title: Adding Relayer support & community relayer plans
description: >-
  We’re happy to announce that we added support for relayers to Typhoon to
  further improve anonymity, with the first official relayer being…
date: "2021-03-28T22:23:54.113Z"
categories: []
keywords: []
slug: /@typhoonnetwork/adding-relayer-support-community-relayer-plans-e95a114fd0e0
---

This story has originally appeared on https://medium.com/@typhoonnetwork/adding-relayer-support-community-relayer-plans-e95a114fd0e0

![](/img/1__XpJhHE4sefLxw6kzGraeIw.png)

We’re happy to announce that we added _experimental_ support for relayers to Typhoon to further improve anonymity, with the first official relayer being available on the mainnet app from today. To use the official relayer, simply tick the “use relayer” checkbox (this will incur a 1% fee to the relayer wallet).

![](/img/1__lYr8__Fv07b69bs2F__4tgOA.png)

Confused what relayers are? Fear not, we’re taking a dive into what they do and why we need them:

#### Why we need relayers

When withdrawing a deposit, the wallet that called the `withdraw()` function is recorded on-chain. Think of it as a “withdraw 0.1 BNB to wallet 0x123” record that gets saved publicly.

If you withdraw with a different wallet than the one you deposited with, this is absolutely no problem and by design. The problem however happens when the wallet that deposited the funds is the same wallet that called `withdraw`. This exposes the transaction deposit and destination and makes transactions public.

Another problem with the current design is that you can’t use withdraw from wallets that have no BNB in them because each transaction costs gas, and that includes withdrawing. So how do you get funds to a new wallet so you can withdraw, without exposing where those funds are coming from?

This is where relayer come in.

#### What is a relayer

A relayer is something like another middleman in the current ecosystem: instead of calling `withdraw()` directly, the user passes the withdraw information to a third party, and that third party initiates the withdraw. As a result, withdraw transactions using a relayer will always get recorded using the relayer wallet and not the users wallet, further improving privacy.

![](/img/1__mcc__kHpnJsufIshNK49Vlw.png)

In return for this, relayers get a small fee of the total transaction.

#### When should I use relayers?

When you don’t mind the fees and want an extra hop between deposit and withdraw.

If you withdraw with a different wallet that already has bnb in it, you don’t need a relayer.

#### Next Up: Host your own relayer and earn fees!

Furthermore we’re calling for community relayers! If you have some IT knowledge and want to earn some of the fees directly from Typhoon, your chance is coming! We want to start by adding at least **2–3 community relayers.**

The details are currently getting finalized and will be summarized in a separate announcement, but here’s the gist of it:

- You host a relayer server (either self-written or the one we made) with a wallet to be used for relaying transactions
- Whenever a transaction goes through your relayer, you make some money through fees (you decide the amount of fees upfront)
- To get listed as a relayer on the Typhoon website, you’ll need to hold a certain amount of TYPH tokens in the relayer wallet (currently considering _5000_ as the minimum, but that will be finalized in the next announcement*)*

More details, including a ready-to-go relayer implementation will follow in the next few days.

#### Looking ahead

We decided to do relayers earlier since we got a lot of feedback from users about this. Adding relayers makes us mostly feature complete and fixes the remaining puzzle piece of sending to wallets without balance.

Tell us what you think

Website: [https://typhoon.network/](https://typhoon.network/)

Telegram: [https://t.me/typhoonnetwork](https://t.me/typhoonnetwork)

Telegram (Announcements): [https://t.me/typhoonnetworkannouncements](https://t.me/typhoonnetworkannouncements)

Twitter: [https://twitter.com/TyphoonCrypto](https://twitter.com/TyphoonCrypto)
