# Mars Society Convention 2026 — Abstract

## InterPlanetary Atomic Swaps (IPAS): On-Chain Hash Time-Locked Contracts as a Settlement Primitive for the Earth–Mars Economy

**Lennart Lopin**, Marscoin Foundation — `lennart@marscoin.org`

Every financial transaction in human history has occurred within one light-speed boundary. Mars breaks that assumption. The 3–22 minute one-way delay, together with two-week solar conjunction blackouts every 26 months, makes centralized exchanges and custodial bridges structurally unviable for Earth–Mars commerce. This paper argues that the correct primitive already exists and has since 2013: the on-chain Hash Time-Locked Contract (HTLC). We call its interplanetary specialization the **InterPlanetary Atomic Swap (IPAS)**.

The cryptographic atomicity of an HTLC is distance-agnostic: the hash does not know what planet its preimage was revealed on, and block-height timelocks do not require the two chains' wall clocks to agree. Its operational safety, however, is distance-sensitive: refund windows, monitoring latency, fee buffers, and conjunction handling must be sized against the physics of the link.

We present (i) a two-domain systems model in which Earth and Mars maintain locally-validating chains linked only by delayed cross-chain observation; (ii) a timeout-sizing inequality with numerical values for close-, average-, far-, and conjunction-spanning orbital regimes; (iii) the **destination-address construction** that turns a bilateral swap into a three-party commerce primitive without a third trusted role; (iv) a bandwidth analysis showing a Mars settlement can mirror Bitcoin at ≈9 MB/hour; and (v) a critical comparison with the Lightning-based proposal of Puente & Puente (2025), arguing that on-chain HTLCs are simpler, more transparent, and better suited to Mars than off-chain channels.

The paper is anchored to an existence proof: on 12 April 2026 the Marscoin Foundation completed the first mainnet BTC↔MARS atomic swap using 4h/8h timelocks. IPAS extends those parameters — a configuration change, not a protocol change — to 72h/144h at average Earth–Mars distance and multi-week windows across conjunction. For a civilization in which physical cargo takes months between planets, a six-day financial settlement is effectively instant.

**Keywords:** atomic swaps, HTLC, Marscoin, Bitcoin, interplanetary commerce, delay-tolerant settlement, Mars economy, solar conjunction, content-addressed settlement.
