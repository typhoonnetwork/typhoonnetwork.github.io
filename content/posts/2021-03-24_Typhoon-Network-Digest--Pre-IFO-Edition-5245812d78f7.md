---
title: Typhoon Network Digest— Pre-IFO Edition
description: >-
  Hi and welcome to the first Typhoon Network digest, where we’ll be giving an
  overview of what happened in the recent weeks, our thoughts…
date: "2021-03-24T07:59:02.615Z"
categories: []
keywords: []
slug: /@typhoonnetwork/typhoon-network-digest-pre-ifo-edition-5245812d78f7
---

![](/img/1__sh__3Vo__qMhGbFEYC5DJwiA.png)

Hi and welcome to the first Typhoon Network digest, where we’ll be giving an overview of what happened in the recent days/weeks, our thoughts and what to expect next.

The last few weeks have been very hectic:

- We announced our [IFO with GooseFinance](https://typhoonnetwork.medium.com/announcing-our-ifo-with-goose-defi-51021aa8be64)
- We published our [whitepaper](https://typhoon.network/resources/typhoon_whitepaper_v1.0.pdf)
- Our Telegram went from 10 to 1260 members
- Our Twitter grew from ~20 to 1012 followers
- We announced an [Airdrop](https://typhoonnetwork.medium.com/announcing-the-typhoon-airdrop-a8fd5e572cc8)
- We had an AMA session with CryptoRoyals ([link](https://twitter.com/CryptoRoyals/status/1373563221106425857))
- Typhoon broke [$5m in Volume](https://dappradar.com/binance-smart-chain/defi/typhoon-network)

### Updates to the core system

#### Small Improvements to privacy

One things we noticed is that users didn’t fully understand how the app is supposed to work and often used the same wallet for both deposit and withdrawal. To make it clear this isn’t a good idea, we’ve added a little warning box when trying to do that.

![](/img/1__HmESUTbeCp7UmePlTxip3Q.jpeg)

To build that, we are hashing the commitment combined with the users wallet address through sha256 and storing that in \`localStorage\`. This way, even when examining \`localstorage\`, it won’t be possible to deduce the wallet addresses. If this experiment turns out to be useful, we might move this logic on-chain.

#### Improvements to Latest Deposits

Latest Deposits now reflects the BNB value and time the deposit was made, to make it much easier to see what is going on within Typhoon. Previously we just displayed the block number.

![](/img/1__tX7kG0HOk9e3fQe8PyDXtg.png)

We also added indicators for 7 day volume and currently deposited total balance. These indicators were needed to ensure that there’s actual activity on Typhoon and transfers are indeed private.

#### Smaller things (& mobile)

Having a lot more users also brought our awareness to some bugs we hadn’t thought about. For example, it was possible to withdraw to an empty wallet address which resulted in the funds getting burnt. Ouch! We’ve now made the address a required field.

There were also a lot more mobile users than we anticipated that either used metamask mobile, or trustwallet, and all kinds of connection issues that mobile connections sometime bring with them.

We didn’t even consider mobile as no-one from the team ever used dApps on their phone. And because of that, we also had no idea that some wallets like TrustWallet just pretend to be metamask, so even though we never said you could use things like TrustWallet, a lot of users still did. Mobile Metamask is another one of these players that we didn’t expect to have this much adoption already.

We had to _temporarily_ disable mobile users to not have people stuck without a way to withdraw.

#### Telegram is hard

When you go from 10 members to 1000+ things get chaotic. People started spamming gifs, memes and links to other sites when we didn’t pay attention. You also have to deal with things that you wouldn’t usually think about, like having a lot of annoying join/leave messages.

To combat this we added a simple bot that that auto-deletes messages with links and remove join/leave messages which made life easier. This was quickly implemented with [Integromat](https://www.integromat.com/?pc=typhoon) (affiliate link) which allowed us to deploy a bot within minutes without any code. However due to the big influx in users, this quickly made us hit the tier limitations and we had to upgrade, ouch.

![](/img/1__ODcrtKtndbWiRj9eclE24w.png)

Luckily, members of the community reached out to us offering to help, and we had our first 2 moderators join us, and are now assisting in keeping the chat clean.

#### Bots, lots of bots

Another thing that happened were promotional offers from a lot of different groups, usually for things like getting a shoutout in exchange for money. Promotion is crucial for young projects, but it turns out a lot of the crypto ecosystem around these promotions are run by bots. Out of the many, many offers and direct messages we received, I’d say almost 90% were facilitated by bots.

This might seem obvious at first, but it really isn’t unless you operated this space before and know what to expect.

The lesson learned here is: Don’t trust big looking numbers.

#### IFO Updates

We got a lot of feedback on the initial entry price we set for the IFO, with concerns that we might not sell out and it being too high. After consulting with Goose and taking in user feedback, we agreed on some new terms to give users the best experience possible. Here’s what changed:

- The entry price is now 0.50ct. All parties agreed that this is a much better goal to hit and gives the token room to grow while also reducing risk of fluctuating price
- We committed 10% of tokens at a price of $1 as initial locked liquidity (from previously 10% @ IFO price). That means that if the IFO sells out, $200.000 USD + tokens will be supplied as liquidity inaccessible to us

#### Looking Ahead

This was a very hectic week, but we’re looking forward to the IFO date and moving the project along afterwards.

There will likely be slight adjustments to the roadmap too since we accelerated the airdrop and are planning to move staking ahead of time based on feedback we gathered from users.

If the past days were an indicator of what’s ahead, I can imagine that the remaining days before the IFO will also be full with even more topics we didn’t see coming.

#### Tell us what you think!

Website: [https://typhoon.network/](https://typhoon.network/)

Telegram: [https://t.me/typhoonnetwork](https://t.me/typhoonnetwork)

Telegram (Announcements): [https://t.me/typhoonnetworkannouncements](https://t.me/typhoonnetworkannouncements)

Twitter: [https://twitter.com/TyphoonCrypto](https://twitter.com/TyphoonCrypto)
