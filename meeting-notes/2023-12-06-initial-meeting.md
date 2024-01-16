## Initial meeting Dec 6th 2023

This is the initial meeting, intended to kick off the process and ensure we met before the end of 2023. No decision was made to

## Agenda

- Intros
- Schedule/frequency discussion
- Project updates
- Discussion

### Pre Meeting Discussion Items

- What is DA (what is and isn’t in scope of WG)
- Charter, Goals, Outcomes and where to host (GitHub?)
- Any CIPs, changes, or new design specifications that need to be - - written or discussed in new year (shwap)
- Open questions and items to discuss

### Meeting Notes

#### Scope

- Network wide params
- Breakages for network specs
- Changes and modifications to expected behavior of the network
- Data and messaging formats

#### Outside scope

- Interface
- Consensus unless related to DA
- Interface wg is more “external” interfaces for builders on node
- DA is internal interfaces (ie: how nodes interact with each other in p2p)


## Project Updates

### Eiger

- Node has header support for p2p protocols
- Currently working on  ipldv2 protocol
- Implementing bitswap in rust
- Multi hash and blockstore (also shwap)
- Can exchange headers, needs to exchange data for sampling

Todo: shrex etc to enable users to interact with blobs and shares with their node

Question:

Concerning Bitswap do we need to re-implement bitswap from scratch? - Are there no half baked solutions to extend?
- Migrated to an existing, didn’t quite “work”
- Found specification is lose and ambiguous
- Appeared to add more than was in spec
- Confusion around bitswap, no good solution - easier to implement
- Existing implementations are not maintained
- Hlib: lets connect eiger team with go-bitswap implementers
- Shwap: Rust implementation is blocked by bitswap so no worry of spec


### Discussion for next time
- Pruning CIP https://github.com/celestiaorg/CIPs/blob/main/cips/cip-4.md

- Ensure we do all team updates


### Actionable Outcomes

- wg repo (ramin to create) to establish goals/outcomes etc
- Eiger to publish Public repo for rust bitswap implementation
- Intro protocol labs with Eiger via Hlib to support bitswap Rust bitswap implementation
- Celesita Node / Hlib to provide Spec for schwap
- Rene: agree on sampling window size (30 days)
