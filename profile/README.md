English · [简体中文](https://github.com/OpenRTL-Lab/.github/blob/main/profile/README.zh-CN.md)

<picture>
  <source media="(prefers-reduced-motion: reduce)" srcset="https://raw.githubusercontent.com/OpenRTL-Lab/.github/main/assets/openrtl-logo.png?v=4">
  <img src="https://raw.githubusercontent.com/OpenRTL-Lab/.github/main/assets/openrtl-logo.gif?v=4" width="128" height="128" alt="OpenRTL green pixel chip: original RapidRTL homepage artwork">
</picture>

# OpenRTL — MIT-Licensed Digital Hardware

**From algorithms to RTL: high-performance, reliable digital hardware for commercial applications.**

[Website](https://openrtl.top/)

OpenRTL develops and publishes original digital hardware under the MIT License.
Our released portfolio includes compute accelerators, controllers and interfaces,
with reusable RTL, reproducible verification and inspectable engineering evidence.

For ASIC and FPGA systems, we provide reusable designs and optional custom
development and integration services.

[Explore released projects](#released-projects) ·
[Review engineering evidence](#engineering-quality) ·
[Discuss a custom ASIC or FPGA design](https://openrtl.top/)

## Released projects

Start with a series catalogue to find released hardware designs and their
engineering evidence. New series are listed here after release.

| Released series | Scope | Catalogue |
| --- | --- | --- |
| ZK Hardware Accelerators | Goldilocks field arithmetic; NTT/INTT, LDE, FRI and Sumcheck/MLE; Poseidon2 and Merkle operations; BN254-G1 MSM | [Browse ZK accelerators](https://github.com/OpenRTL-Lab/zk-accelerators/blob/main/README.en.md) |
| OpenETH | Gigabit Ethernet controller and DMA; frame buffering and clock-domain crossing; MAC/CRC, RGMII and PHY management; Linux driver and test programs | [Explore OpenETH](https://github.com/OpenRTL-Lab/openeth) |

The ZK series provides standalone Chisel accelerators, generated SystemVerilog,
and native interfaces for integration into ASIC or FPGA designs.
Its catalogue links to each module's versions, source, released artifacts,
interface and mathematical-model documentation, reference models, and tests.
OpenETH provides reusable Ethernet RTL and software, including Chisel and
SystemVerilog sources, interface documentation, simulation tests and documented
reference-board validation. Gigabit Ethernet describes the interface; measured
application throughput and delivery limits are documented in the repository.

Module-specific releases and measurements are maintained by each series rather
than duplicated on this organization page.

Supported configurations, verification scope, performance measurements, and
synthesis conditions are documented by each individual project. The ZK series
contains standalone compute blocks, not an end-to-end zero-knowledge prover.

## Engineering principles

- **Readable RTL** — clear structure and documented behavior.
- **Reproducible verification** — reference models, test instructions, and
  explicit toolchain requirements.
- **Explicit interfaces and verification boundaries** — documented protocols,
  supported configurations, and the scope of reported results.
- **Portability** — reusable boundaries, documented dependencies, and clear
  integration requirements for adapting designs to different target systems.

## Engineering quality

Our goal is **commercial-grade performance and reliability**: useful hardware
designs that can be evaluated, integrated, and maintained—not just algorithm
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

Need digital hardware tailored to your workload or system?
[Visit the OpenRTL Lab website](https://openrtl.top/) for service information
and contact details to discuss **custom ASIC/FPGA hardware development**
and integration.
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
