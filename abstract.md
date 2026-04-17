# Mars Society Convention 2026 — Abstract

## InterPlanetary Atomic Swaps (IPAS): On-Chain Hash Time-Locked Contracts as a Settlement Primitive for the Earth–Mars Economy

**Lennart Lopin**, Marscoin Foundation — `lennart@marscoin.org`

Every financial transaction in human history has occurred within a single light-speed boundary. Mars breaks that assumption. The 3–22 minute one-way communication delay, together with approximately two-week solar conjunction blackouts every 26 months, makes centralized exchanges, custodial bridges, and synchronous settlement infrastructures structurally unviable for Earth–Mars commerce. This paper argues that the correct primitive already exists and has, in fact, existed since 2013: the on-chain Hash Time-Locked Contract (HTLC). We call its interplanetary specialization the **InterPlanetary Atomic Swap (IPAS)**.

The cryptographic atomicity of an HTLC — either both parties complete or both refund — is distance-agnostic: the hash does not know what planet its preimage was revealed on, and block-height timelocks do not require the two chains' wall clocks to agree. The operational safety of an HTLC, however, is distance-sensitive: refund windows, monitoring latency, fee-spike buffers, and conjunction handling must all be sized against the physics of the link.

We present (i) a two-domain systems model in which Earth and Mars each maintain locally-validating chains linked only by delayed cross-chain observation; (ii) a formal timeout-sizing inequality with numerical values for close-, average-, far-, and conjunction-spanning orbital regimes; (iii) the **destination-address construction** that turns a bilateral swap into a three-party commerce primitive without introducing a third trusted role; (iv) a bandwidth analysis showing that maintaining delayed mirrors of each other's chains is well within the communication budget of any human Mars settlement (≈9 MB/hour for full Bitcoin blocks); and (v) a critical comparison with the Lightning-based interplanetary proposal of Puente & Puente (2025), arguing that on-chain HTLC swaps are simpler, more transparent, more custody-free, and better suited to the Mars case than any off-chain payment-channel construction.

The paper is anchored to an existence proof: on 12 April 2026, the Marscoin Foundation completed the first mainnet BTC↔MARS atomic swap using 4-hour and 8-hour terrestrial timelocks. IPAS extends those parameters — a configuration change, not a protocol change — to 72h/144h for Earth–Mars average distance and to multi-week windows across conjunction. For a civilization in which physical cargo takes months to cross between planets, a six-day financial settlement is effectively instant.

**Keywords:** atomic swaps, HTLC, Marscoin, Bitcoin, interplanetary commerce, delay-tolerant settlement, Mars economy, solar conjunction, content-addressed settlement.
