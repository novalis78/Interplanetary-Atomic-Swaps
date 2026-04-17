# InterPlanetary Atomic Swaps (IPAS)

**On-Chain Hash Time-Locked Contracts as a Settlement Primitive for the Earth–Mars Economy**

Lennart Lopin, Marscoin Foundation — submitted to the Mars Society Convention 2026 (USC, October 22–24, 2026).

## What this is

A conceptual systems paper that formalizes **IPAS** — the InterPlanetary Atomic Swap — as the on-chain HTLC specialization appropriate for commerce between Earth and Mars under light-speed delay and solar conjunction blackouts.

The central claim: HTLCs are *accidentally interplanetary*. Their cryptographic atomicity is distance-agnostic; only their operational parameters (timelock widths, monitoring latency, fee-spike buffers) need to be sized to the Earth–Mars link. The first mainnet BTC↔MARS atomic swap on 12 April 2026 is the existence proof; IPAS is the parameter extension that makes the same construction safe for interplanetary use.

## Highlights

- **Destination-address construction** — turns a bilateral swap into a three-party commerce primitive without introducing a third trusted role.
- **Timeout-sizing inequality** with numerical values for close, average, far, and conjunction-spanning orbital regimes.
- **Bandwidth analysis** showing ≈9 MB/hour suffices to maintain a full Bitcoin mirror on Mars.
- **Critical comparison with interplanetary Lightning** (Puente & Puente 2025) — argues for on-chain simplicity, transparency, and sovereignty over off-chain channels with watchtower dependence.
- **Historical observation**: HTLCs (Tier Nolan, BitcoinTalk, May 2013) and the Marscoin "slower interplanetary chain" discussions emerged in the same community at the same time. Neither side knew it was building half of an interplanetary financial architecture.

## Build

```bash
pdflatex ipas.tex
bibtex   ipas
pdflatex ipas.tex
pdflatex ipas.tex
```

Requires a standard TeX Live installation with `natbib`, `authblk`, `booktabs`, `amsmath`, `hyperref`, `listings`.

## Files

| File | Purpose |
|------|---------|
| `ipas.tex` | Main paper (LaTeX source) |
| `references.bib` | BibTeX bibliography |
| `abstract.md` | Mars Society Convention 2026 submission abstract |
| `ipas.pdf` | Compiled paper (18 pp.) |
| `figures/` | Reserved for future figures (bandwidth plot, timelock diagram) |

## Prior art acknowledged

- Nolan (2013) — original HTLC atomic-swap construction
- Poon & Dryja (2016) — Lightning Network
- Puente & Puente (2025) — Bitcoin as an Interplanetary Monetary Standard (closest adjacent work)
- De Filippi & Leiter (2021) — Blockchain in Outer Space
- Haqq-Misra (2024) — sovereign-Mars economic freedom model
- Zubrin (1995) — economic viability of Mars colonization
- Lopin et al. (2014) — original Marscoin whitepaper

## Related Marscoin work

- Marscoin whitepaper (2014): https://www.marscoin.org/papers/marscoin-whitepaper.pdf
- Martian Republic governance paper (2022): https://www.marscoin.org/martian-republic-marscoin-blockchain-auditable-p2p-governance-voting/
- IPAS article on marscoin.org (April 13, 2026)

## License

Paper text: CC-BY 4.0. BibTeX data: public domain.

## Citation

```bibtex
@misc{lopin2026ipas,
  author = {Lopin, Lennart},
  title  = {InterPlanetary Atomic Swaps ({IPAS}): On-Chain Hash Time-Locked
            Contracts as a Settlement Primitive for the {E}arth--{M}ars Economy},
  year   = {2026},
  note   = {Mars Society Convention 2026 submission},
  url    = {https://github.com/novalis78/Interplanetary-Atomic-Swaps}
}
```
