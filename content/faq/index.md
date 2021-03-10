---
description: ''
sidebar: 'faq'
next: '/faq/howto/'
---

# FAQs

## General FAQs

### What is Loopring?

#### Loopring's Vision and Objectives

Blockchain technology empowers real ownership - ownership of digital assets, and soon, ownership of legacy financial and physical assets as well. This technology and the cryptoassets it supports have upended traditional notions of currency and will establish the foundation of the next generation of finance.

Ironically, however, most cryptoasset holders still trade these assets on Centralized Exchanges, or CEXes, temporarily giving up their ownership (keys) to intermediaries, and eschewing a primary benefit & virtue of the asset itself. Over the years, users have lost more than two billion USD worth of cryptoassets on these custodial platforms. More depressingly, it is often difficult to distinguish if assets were stolen by external hackers or an inside job by malicious owners.

We believe that cryptoasset trading should be and will be risk-free and worry-free in terms of custody. Traders should have strong cryptographic guarantees that their assets cannot be wrongfully taken from the platforms where they trade - not by hackers, not by exchange owners, and not even by state-level adversaries. The solution is to trade on non-custodial exchanges, also referred to as Decentralized Exchanges, or DEXs - powered by the underlying blockchains & smart contracts where these assets natively live.

We also envision that trading cryptoassets on DEXs will be less expensive compared to CEXes, because security is essentially outsourced to the blockchain and cryptographic processes, instead of large, expensive, fallible human teams. These cost savings can be passed through to users. Finally, liquidity will be more fluid, able to be aggregated at a much larger scale, if not globally.

Loopring's objective is to design and engineer the best-in-class orderbook-based DEX protocol on Ethereum. With Loopring v3 - using a cutting-edge construction called zkRollup - we have achieved this. We wish to make this infrastructure available for the entire industry, powering people and projects to build highly scalable non-custodial crypto-exchanges, and improving cryptoasset holders' overall trading experience and peace of mind. Satisfying owners, users, and regulators, we expect that our effort will accelerate the adoption of blockchain technology and cryptocurrencies.

#### Loopring Protocol is Secure

The security of user assets is and will always remain Loopring's top priority. Previous versions of the Loopring protocol did not take custody of user assets at all - traders were always in possession of their funds. The latest version, Loopring 3.0, relies on smart contracts to hold assets to be traded. We designed the protocol in such a way that users can always claim their assets in all circumstances, even when DEX operators are evil or cease to exist. Loopring exchanges inherit 100% Ethereum-level security guarantees.

Loopring 3.0 does not rely on any external cryptoeconomic assumptions, challenge periods, or fraud proofs as found in Optimistic Rollup or other layer 2 scaling solutions. Instead, the Loopring protocol enforces every execution with validity proofs (Zero-Knowledge Proofs) to update and attest DEX states, achieving the highest level of security. All actions are correct by construction, or simply cannot happen: exchange operators are constrained to purely protocol-described behaviour.

We claim that Loopring v3 offers users the same level of security as the underlying Ethereum blockchain if a feature called On-Chain Data Availability (OCDA) is turned on. Trading on Loopring-based DEXs does not demand traders place any trust whatsoever in the DEX owners or operators, nor the Loopring team. In terms of crypto-trading, we believe being trustless will become the new standard of trustworthiness.

#### The Redemption of Centralized Exchanges

If you have ever run a centralized exchange business for cryptocurrencies, you know the stress and fear of being hacked. You also know the regulatory burden which is being imposed on custodial crypto-businesses, and rightfully so. Loopring ensures that even if all your servers were compromised, you will, at worst, only lose a couple of Ether that you use as transaction fees (gas). You can always recover from such an incident and resume your business. Even in the unimaginable case of being blackmailed, extorted or threatend with violence, an exchange owner simply cannot access user funds - a powerful deterrent. And without control over user assets, you also shed the bulk of regulatory burden. Control is a liability. Using an open-sourced, audited, cryptographically sound protocol means less time & money spent on security & compliance, and more on growing your business.

#### Loopring is Remarkably Performant

DEXs have been around on Ethereum for a few years already, but have not yet reached their full potential. One main reason is because most DEX protocols suffer terrible performance issues: the throughput is too low while the cost is too high. This is also commonly referred to as the scalability problem. The performance issues prevent those DEX protocols (and the products built atop) from being massively adopted as no professional market makers or traders can use these as their primary trading venues. The performance vs. security tradeoff has indeed been a polarizing one. Loopring v3 was conceived to solve DEX scalability without compromising on Ethereum security.

We believe the way many trading protocols use the underlying blockchain is fundamentally flawed. Loopring takes a different approach known as zkRollup proposed by Vitalik Buterin. zkRollup migrates most computations off the blockchain and only broadcasts exchanges' new state roots and their corresponding proofs onto the blockchain. In other words, the Loopring protocol uses the underlying Ethereum blockchain mainly as a data layer and a Zero-Knowledge Proof verification thin-logic layer. As a result, Loopring's throughput is as high as 2,025 trades per second with OCDA, and 16,400 trades per second without. The corollary is that the cost per trade settlement is as small as $0.00015 USD, which can be further optimized (halved in near-term) by using techniques such as GPU-based proof generation and recursive SNARKs.

We also believe that Loopring's performance is sufficient for professional traders and market makers to deploy algorithmic strategies and other automated trading bots. This was not previously possible on any DEX as it was prohibitively slow and expensive. By building on top of Loopring 3.0, orderbook-based DEXs can be commercially viable for the first time. With Loopring, we expect non-custodial exchanges to begin outcompeting and displacing many centralized counterparts.

#### What Loopring is

- An application-specific zkRollup protocol, a relayer, a non-custodial exchange, a smart wallet — but eventually it will just be Loopring, where you use, trade, grow, and store your assets.
- Aiming to become the leading user-facing financial services application in the world. Trading, investing, payments, ‘banking’. The gateway of choice for users to experience the parallel financial system of Ethereum — in all its glory and security.

#### What Loopring is not

- A generalizable zkRollup seeking to support arbitrary protocols or functionality deployed atop it.
- An L2 focusing on having other projects build their products atop it.

#### Loopring at large

It’s true that Loopring is fundamentally ‘different’ — vs other L2s, and vs other DEXes or payment platforms. It operates across the stack, consists of multiple components, and at any one time, a reference to Loopring can mean a few things. In our mind, and the mind of our community, Loopring is the collective — all of the components tied together and working in tandem. In its whole, it can be thought of as Loopring, the project. But let’s see what actually makes up Loopring, the project.

- Loopring protocol is an open source Ethereum zkRollup protocol — a layer-2 for securely scaling exchanges and payments.
- Loopring relayer is a closed source zkRollup relayer — the backend (operator) that does all the off-chain duties to make a zkRollup roll.
- Loopring exchange is a non-custodial Ethereum exchange — a highly performant (super fast, gas-free) AMM & orderbook-based exchange with 100% Ethereum security guarantees. It also acts as a payment platform.
- Loopring wallet is an Ethereum smart contract wallet — a mobile wallet app with social recovery, other security features, and with the Loopring L2 baked in. (It is the app, as well as the open source smart contracts which constitute the wallet).

#### From Protocol To Products

While Loopring spends time on all the above components, and the team is indeed split in three groups: protocol, relayer, product, the overarching theme is that Loopring has matured from purely a protocol, to a vertically integrated project, with our user-facing products taking a front seat in our minds. The protocol and relay advancement is ultimately to serve the product needs, serve end-user Ethereans, and more generally, delight our users. This is worth repeating:

- While still investing heavily in protocol R&D and relayer improvement, Loopring is becoming increasingly focused on building our consumer products, the Loopring Exchange, and Loopring Wallet.

In this sense, to our knowledge, Loopring is completely unique vs other layer 2 projects. Other L2s (rollups) are seeking to become platforms for other protocols/projects to build on, while we are focusing on building our own products and capabilities atop our layer 2.

When most people refer to Loopring L2 these days, they are referring to the ‘canonical Loopring L2’, which is our implementation of the Loopring zkRollup protocol, and our products that live atop.

#### L2 Landscape

It helps to have comparisons. Other L2 creators: zkRollup projects MatterLabs and Starkware, and optimistic rollup projects Optimism and Arbitrum, have different goals. [There are other great rollup projects too.] These four projects seek to draw in other protocols or dapps to migrate or build anew on their L2. These L2s don’t build specific protocols, nor user-facing products themselves, at least not at the moment. Loopring on the other hand does not explicitly seek to have other protocols deployed or dapps built on top of us.

There is some nuance in this statement, though. For example, third party apps or projects can integrate Loopring L2, to allow functionality like instant, gas-free swaps, or transfers within their own product. This just uses our API. Or of course they can integrate Loopring to allow their users to see onto L2, displaying their balances, etc., like dashboards Zapper and Zerion have done, or accounting software Rotki has done. Loopring will be a massive hub of financial activity on Ethereum, and anyone can plug into it via API.

But they cannot build their own generalized protocol or product atop Loopring L2. Loopring is what is called an application-specific zkRollup, and our applications/functionality are orderbook exchanges, AMMs, transfers, and related operations. It cannot support arbitrary EVM functionality. That is what optimistic rollups can support (now/~imminently), and zkRollups will be able to support in future.

#### We are building up, not out

While we are building our products upwards, into the hands of hopefully millions of users, other people or projects can indeed build something on Loopring protocol, along the lines of exchange & payment functionality. It is open source, so anyone can use the smart contracts and ZK circuits. But the practical truth is, the relayer is a massive undertaking, and is needed to make a zkRollup run. Our relayer is closed source. We have spent years building and optimizing it for our purposes, and believe it is a strong competitive advantage.

- To be clear, a closed source relayer poses exactly zero threat to users’ assets — such is the beauty of a zkRollup. Using a single relayer is secure since it is constrained to only protocol-allowed behaviour.

For someone else to build on Loopring L2, they can use/fork the protocol, and then need to:

A) Build a relayer so they can run their implementation of a Loopring zkRollup. They can be the single relayer for their L2/product, the same way we are the relayer for ours, or they can use the protocol in a relayer-agnostic format, where anyone can be the relayer servicing it. However, building a powerful, stable relayer is a tremendous task.

B) Use our relayer as a service. This means working with us to replicate an instance of our relayer, which is stood up just to service their project, being configured for their needs, etc. (Not to be confused with using our relayer within your application for our existing capabilities, such as L2 trades & transfers, which is no problem, just using our API).

You may be aware that we have previously mentioned offering our ‘relayer-as-a-service’ to other projects, which is indeed still perfectly viable. However, practically speaking, our energy is being devoted to improving the relayer to strengthen our products and user experiences, not in licensing it, or working with others to tweak it as they may need. Some projects have recently requested to discuss how they can build their products on Loopring L2, and the fact is, we simply do not have the bandwidth to prioritize that, given we are focused on improving our protocol, relayer, and products, for the sake of our current and future users.

#### Future

As you probably grasp, Loopring’s future lies in building beautiful, secure, performant products.

While we currently target crypto-native users (Ethereans), everything we have done is to be able to outcompete the incumbents — the fintech giants. We built our zkRollup protocol ourselves so we can emulate their experience, without sacrificing Ethereum security at all. Loopring made it so the biggest Ethereum UX hurdle was proven possible to solve, and custodial counterparts could no longer claim that non-custodial applications offered inferior experiences.

Loopring is striving to build global, consumer-grade financial applications, and we will measure ourself against this goal. Our metrics are those of users, volume, tx count, liquidity, stickiness, downloads, and overall, delighting users.

It is a rather funny thing that all the engineering effort and heavy R&D over 3.5 years ultimately comes down to the basics: giving users a product they love to use. In the context of Loopring that meant abstracting the difficulties of using Ethereum, and keeping the critical properties.

We built the first ever zkRollup ourselves to support this goal, and we continue improving our zkRollup to support this goal. But as is becoming clear, if other providers make the cryptographic advances that seem likely, we would have no problem ‘ripping out our rollup’ layer of the stack, and upgrading the Loopring project onto a generalizable zkRollup — all in the name of products having more and improved functionality. We believe our relayer and apps would always be a differentiator in powering advanced products.

Similarly, we are even looking into incorporating optimistic rollup constructions into our stack, notably useful for the Loopring wallet, where we can deploy our actual smart wallet logic on L2, and solve remaining pain points for users.

To unleash Ethereum and put the new financial system in everyone’s pockets, we will use whatever technology is best for the job — whether we continue to build it all ourselves, or use a better alternative.
