# Bitcoin Staking

Asula is secured by BTC staked to the protocol through Babylon’s staking protocol. We leverage the cryptoeconomic security provided by BTC to secure Asula, and by extension, any rollup in Asula’s ecosystem. Asula will behave as a consumer to Babylon, receiving messages from the Babylon Cosmos SDK chain on staking events to Asula and communicating with the staking protocol through Babylon’s Finality Providers to enable slashing on Bitcoin through Extractable One Time Signatures.

Bitcoin staked to Asula will generate yield from different forms of incentives and activity from Asula’s ecosystem of rollups. As more users stake to Asula, the security of the network increases.

Babylon provides relatively strong security guarantees by slashing for equivocation on the Asula L1. Leveraging these guarantees, we are able to ensure Asula is able to appropriately respond to dishonest activity on the network while maintaining uninterrupted liveliness for honest nodes.

### aBTC — Asula’s Liquid Staked BTC

When users stake BTC to secure the Asula network, they can mint an equivalent amount of aBTC as a liquid representation of their staked BTC. aBTC is minted on the Asula L1 and can move freely to any Asula-based rollup. The aBTC holder earns transaction fees and ASLA block rewards for securing the L1.

The aBTC asset is designed to be the default yield-bearing BTC representation across all rollups. The issuance of idle aBTC liquidity on the Asula L1 is quite attractive for prospective rollup builders, as their products can bootstrap liquidity by onboarding aBTC holders.

This relationship between staked BTC and rollups is closely related to the network effects that attracted many builders to the Ethereum ecosystem; the more TVL grew on ETH L1, the more attractive this ecosystem became for rollup builders using ETH as a settlement layer. However, Asula is structured to be even more favorable to attract rollup builders as there are no DeFi apps on L1 to compete for aBTC.



**Potential Automated Strategies**

As users mint their aBTC, they have full control over where they deploy the aBTC. In case they don’t want to manage their own yield-bearing strategies, they can potentially deploy their aBTC into a vault provided by the Asula protocol. ASLA holders can control this vault to direct where the liquidity in the ecosystems. This liquidity direction can function in similar ways to gauges where protocols offer yield against aBTC deployed by ASLA holders.

<figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>
