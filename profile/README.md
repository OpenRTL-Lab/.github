<picture>
  <source media="(prefers-reduced-motion: reduce)" srcset="https://raw.githubusercontent.com/OpenRTL-Lab/.github/main/assets/openrtl-logo.png?v=4">
  <img src="https://raw.githubusercontent.com/OpenRTL-Lab/.github/main/assets/openrtl-logo.gif?v=4" width="128" height="128" alt="OpenRTL green pixel chip: original RapidRTL homepage artwork">
</picture>

# OpenRTL

**Open hardware, from algorithms to RTL.**

English · [简体中文](https://github.com/OpenRTL-Lab/.github/blob/main/profile/README.zh-CN.md)

OpenRTL publishes open, reusable, and verifiable digital hardware. Our focus is
readable RTL, practical integration, and verification evidence that users can
inspect and reproduce.

## Released projects

### [ZK Hardware Accelerators](https://github.com/OpenRTL-Lab/zk-accelerators/blob/main/README.en.md)

A collection of **11 families of standalone Chisel accelerators** for
zero-knowledge computation, with generated SystemVerilog and native interfaces
for integration into ASIC or FPGA designs.

| Area | Accelerators |
| --- | --- |
| Field arithmetic | Goldilocks prime-field and quadratic-extension vectors; batch inversion |
| Polynomial computation | NTT/INTT, coset LDE, FRI folding, Sumcheck and MLE |
| Hashing and commitments | Poseidon2 permutation, sponge hashing, and Merkle operations |
| Elliptic-curve computation | BN254-G1 multi-scalar multiplication |

[Browse the accelerator catalogue](https://github.com/OpenRTL-Lab/zk-accelerators/blob/main/README.en.md)
to find each module's version, source, released artifacts, interface and
mathematical-model documentation, reference models, and simulation tests.
An example versioned release is
[Goldilocks NTT/INTT v1.1.0](https://github.com/OpenRTL-Lab/goldilocks-ntt-intt/releases/tag/v1.1.0).

Supported configurations, verification scope, performance measurements, and
synthesis conditions are documented by each individual project. These are
standalone compute blocks, not an end-to-end zero-knowledge prover.

## Engineering principles

- **Readable RTL** — clear structure and documented behavior.
- **Reproducible verification** — reference models, test instructions, and
  explicit toolchain requirements.
- **Explicit interfaces and verification boundaries** — documented protocols,
  supported configurations, and the scope of reported results.
- **Portability** — reusable boundaries, documented dependencies, and clear
  integration requirements for adapting designs to different target systems.

## Licensing

OpenRTL publishes original project code under the **MIT License**. Consult each
repository's license and third-party notices for the terms covering its files
and dependencies.
