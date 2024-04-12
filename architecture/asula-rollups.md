# Asula Rollups

Asula rollups are Layer 2 blockchains that leverage Asula for verification and settlement. These rollups access the security guarantees provided by BTC staked to the Asula L1 and benefit from Asula's optimizations for easy deployment of app-specific rollups.

However, rollup optimization is not only focused on ease of deployment; the Asula base layer embeds features that reflect developer demand for different customizations and preferences.

Rollups deploying using the Asula SDK can configure:

* **Execution environments**: Rollups can choose between EVM, Move VM, and SVM. Eventually, we hope to allow users to bring their own execution environments.
* **Block times:** Rollups can decide to have sub-second blocks (with goals to get as low as 500ms).
* **Trust Assumptions:** Rollups can run under optimistic or zk trust assumptions. We will also allow developers to go from optimistic to zk rollups as the Asula zk stack matures. ZK rollups will be able to verify proofs from different proving systems using the Asula L1.
