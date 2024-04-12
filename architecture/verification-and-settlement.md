# Verification & Settlement

To build a verification layer as a standalone blockchain is to allow proofs to be verified on it. The edge a verification layer has is to make it as cheap and simple as possible to verify these proofs. Today's primary use for proofs and verification are rollups, which are most relevant for Asula to enable scaling on Bitcoin. We can, however, imagine a world where arbitrary applications use proofs to secure transactions or agreements between two parties.

The primary reasons why proof verification is difficult, if not impossible, on Bitcoin today are:

* The Bitcoin scripting language is not expressive enough to enable arbitrarily complex business logic. Due to the lack of Turing-completeness, writing even basic verification scripts becomes complex.
* Bitcoin blocks are slow with 10 minute average block times. This means that if proving and verification were 0 cost, the fastest we could do verification would be 10 minutes.
* Bitcoin finality is probabilistic due to the nature of Proof-of-Work. Even after 6 blocks (\~60 minutes) the probability of a reorg is \~0.1%. The probabilistic finality combined by slow block times would lead to several UX issues when it comes to bridging.
* Doing verification natively on Bitcoin requires all data to be posted to Bitcoin. This becomes expensive as Bitcoin has very limited throughput of about (4MB every 10 minutes). If we were to post DA to a different layer like Celestia, the argument to do verification on a different layer also becomes quite strong (even if proofs are posted to BTC).
* Contention with other applications. Like Ethereum, since Bitcoin is a general-purpose blockchain, applications like ordinals or inscriptions can effectively impact fees on the blockchain leading to verification becoming more expensive than it normally is.

The result of these restrictions for verification on Bitcoin is a bespoke (likely unsafe) and heavily fragmented Bitcoin scaling ecosystem. This creates the need for an Asula-like verification + settlement layer. In a modular blockchain ecosystem, a verification or settlement layer is designed to check that transactions from the rollup represent changes to state that were executed correctly. Asula will facilitate this via both both fraud proofs and zk proofs. In many ways a settlement layer is like a specialized bridge which acts as a hub between many rollups
