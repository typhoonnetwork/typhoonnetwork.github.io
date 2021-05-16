---
title: Typhoon launches to bring private transactions to Binance Smart
description: >-
  Blockchains are designed to be public ledgers by default: Everyone can see
  everything that happens on those chains, that’s just how they…
date: "2021-03-10T09:31:31.837Z"
categories: []
keywords: []
slug: >-
  /@typhoonnetwork/typhoon-launches-to-bring-private-transactions-to-binance-smart-9306852452fd
---

This story has originally appeared on https://medium.com/@typhoonnetwork/typhoon-launches-to-bring-private-transactions-to-binance-smart-9306852452fd

![](/img/1__oyD5tLUh1pFiD2a3Zhk7TA.png)

Blockchains are _designed_ to be public ledgers: Everyone can see everything that happens on those chains, that’s just how they work. It’s very easy to open bscscan.com, type in a wallet address and see what that wallet was up to:

- Where that person sent funds recently
- Which smart contracts he interacted with
- Which apps they used
- How much money they hold in any specific asset
- …and much more!

The more information available online, the easier it is to create a profile on people based on their online activity with no way to really escape: Because even if you decide to send your funds to a new wallet, the connection to that new wallet is recorded publicly as well!

#### Where Typhoon steps in

Typhoon is a decentralized, fully on-chain implemented, project to enable private transactions between 2 wallets. It does this cleverly by somewhat taking on the role of proxy, but on cryptography steroids.

Typhoon utilizes [zkSNARK](https://z.cash/technology/zksnarks/), a novel form of zero-knowledge cryptography. zkSNARK makes it possible for users to prove possession of information, without actually revealing that information.

When depositing money into Typhoon, the user generates a random secret and submits a part of it (a hash) along with the assets into the smart contract. In order to then withdraw that deposit again, the user has to provide cryptographic proof that he is indeed the owner of a secret to an unspent deposit. All without revealing the secret he holds to the public blockchain, thanks to zkSNARK!

#### In more simple words

When depositing into Typhoon, a random piece of text will be generated. Whoever possesses the piece of text is eligible to withdraw the deposited funds to any address of their liking.

Since all transactions come and go to the Typhoon smart contract, it will all look the same to an observer and thus makes it no longer possible to deduce who actually sent what to whom! Neat!

#### Give us a try and tell us what you think!

> Website: [https://typhoon.network/](https://typhoon.network/)

> dApp: [https://app.typhoon.network/](https://typhoon.network/)

> Telegram: [https://t.me/typhoonnetwork](https://t.me/typhoonnetwork)

> Twitter: [https://twitter.com/TyphoonCrypto](https://twitter.com/TyphoonCrypto)
