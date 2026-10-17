<picture>
  <source media="(prefers-reduced-motion: reduce)" srcset="https://raw.githubusercontent.com/OpenRTL-Lab/.github/main/assets/openrtl-logo.png?v=4">
  <img src="https://raw.githubusercontent.com/OpenRTL-Lab/.github/main/assets/openrtl-logo.gif?v=4" width="128" height="128" alt="OpenRTL green pixel chip: original RapidRTL homepage artwork">
</picture>

# OpenRTL — Hardware Accelerators for ASIC & FPGA

**Open hardware, from algorithms to RTL.**

English · [简体中文](https://github.com/OpenRTL-Lab/.github/blob/main/profile/README.zh-CN.md)

MIT-licensed hardware accelerators, from algorithms to reusable RTL.
OpenRTL brings together released designs and inspectable engineering evidence
for engineers building ASIC and FPGA systems.

[Explore released accelerators](#released-projects) ·
[Review engineering evidence](#engineering-quality) ·
[Discuss a custom ASIC or FPGA design](#custom-asic--fpga-development)

## Released projects

### [ZK Hardware Accelerators](https://github.com/OpenRTL-Lab/zk-accelerators/blob/main/README.en.md)

A collection of **11 families of standalone Chisel accelerators** for
zero-knowledge (ZK) computation, with generated SystemVerilog and native
interfaces for integration into ASIC or FPGA designs.

| Area | Accelerators |
| --- | --- |
| Field arithmetic | [Goldilocks prime-field vectors](https://github.com/OpenRTL-Lab/prime-field-vector-goldilocks), [quadratic-extension vectors](https://github.com/OpenRTL-Lab/extension-field-vector-goldilocks), [batch inversion](https://github.com/OpenRTL-Lab/batch-inversion-goldilocks) |
| Polynomial computation | [NTT/INTT](https://github.com/OpenRTL-Lab/goldilocks-ntt-intt), [coset LDE](https://github.com/OpenRTL-Lab/coset-lde-goldilocks), [FRI folding](https://github.com/OpenRTL-Lab/fri-fold-goldilocks), [Sumcheck & MLE](https://github.com/OpenRTL-Lab/sumcheck-mle-goldilocks) |
| Hashing and commitments | [Poseidon2 permutation](https://github.com/OpenRTL-Lab/poseidon2-goldilocks), [Poseidon2 sponge](https://github.com/OpenRTL-Lab/poseidon2-sponge), [Merkle operations](https://github.com/OpenRTL-Lab/merkle-goldilocks) |
| Elliptic-curve computation | [BN254-G1 multi-scalar multiplication (MSM)](https://github.com/OpenRTL-Lab/bn254-msm) |

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

## Engineering quality

Our goal is **commercial-grade performance and reliability**: useful compute
blocks that can be evaluated, integrated, and maintained—not just algorithm
demonstrations. The released portfolio is an inspectable record of engineering
capability, not a blanket production-readiness claim.

When evaluating a design, follow its repository and release documentation for:

- **Correctness and stability evidence**: reference-model comparisons, tested
  configurations, protocol and corner-case coverage, and known limitations.
- **Performance in context**: workload, cycle counts, throughput, latency,
  resource usage, tool versions, and target-specific synthesis conditions where
  reported. Simulation, synthesis, and board/silicon measurements are distinct.
- **Reproducibility and integration**: versioned RTL, verification instructions,
  interface contracts, dependencies, and portability constraints.

Validation is specific to the documented version, configuration, and target.
ASIC/FPGA integration is not a claim that every design has been fabricated,
board-tested, or qualified for every application.

## Custom ASIC & FPGA development

Need a hardware accelerator tailored to your workload or system?
[Contact the maintainer, @XLxiaoliaoGmail](https://github.com/XLxiaoliaoGmail),
to discuss **custom ASIC/FPGA accelerator development** and integration.
The released designs above provide a starting point for evaluating fit and
engineering capability.

Possible project scopes include algorithm-to-RTL implementation, datapath and
memory-architecture customization, interface adaptation, performance/resource
optimization, and verification tailored to agreed requirements. Deliverables,
target support, validation, and schedules are agreed for each engagement.

A useful initial brief includes your workload, ASIC process or FPGA device,
interfaces, throughput/latency and area/power goals, validation expectations,
and delivery timeline. Share confidential specifications only through a
separately agreed private channel, not public GitHub issues.

## Licensing

OpenRTL publishes original project code under the **MIT License**. Consult each
repository's license and third-party notices for the terms covering its files
and dependencies.

Commercial use of the MIT-licensed code does not require a custom-development
engagement. Paid customization and support are separate, optional services.
