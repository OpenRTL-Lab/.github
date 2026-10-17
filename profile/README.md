<picture>
  <source media="(prefers-reduced-motion: reduce)" srcset="https://raw.githubusercontent.com/OpenRTL-Lab/.github/main/assets/openrtl-logo.png?v=4">
  <img src="https://raw.githubusercontent.com/OpenRTL-Lab/.github/main/assets/openrtl-logo.gif?v=4" width="128" height="128" alt="OpenRTL green pixel chip: original RapidRTL homepage artwork">
</picture>

<a name="english"></a>

# OpenRTL — Hardware Accelerators for ASIC & FPGA

**Open hardware, from algorithms to RTL.**

[Website](https://openrtl.top/) · [English](#english) · [简体中文](#简体中文)

MIT-licensed hardware accelerators, from algorithms to reusable RTL.
OpenRTL brings together released designs and inspectable engineering evidence
for engineers building ASIC and FPGA systems.

[Explore released accelerators](#released-projects) ·
[Review engineering evidence](#engineering-quality) ·
[Discuss a custom ASIC or FPGA design](https://openrtl.top/)

## Released projects

Start with a series catalogue to find released accelerators and their
engineering evidence. New series are listed here after release.

| Released series | Scope | Catalogue |
| --- | --- | --- |
| ZK Hardware Accelerators | Goldilocks field arithmetic; NTT/INTT, LDE, FRI and Sumcheck/MLE; Poseidon2 and Merkle operations; BN254-G1 MSM | [Browse ZK accelerators](https://github.com/OpenRTL-Lab/zk-accelerators/blob/main/README.en.md) |

The ZK series provides standalone Chisel accelerators, generated SystemVerilog,
and native interfaces for integration into ASIC or FPGA designs.
Its catalogue links to each module's versions, source, released artifacts,
interface and mathematical-model documentation, reference models, and tests.
Module-specific releases and measurements are maintained there rather than
duplicated on this organization page.

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
[Visit the OpenRTL Lab website](https://openrtl.top/) for service information
and contact details to discuss **custom ASIC/FPGA accelerator development**
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

---

## 简体中文

# OpenRTL — 面向 ASIC 与 FPGA 的硬件加速器

**从算法到 RTL，构建开放、可复用、可验证的数字硬件。**

[官方网站](https://openrtl.top/) · [English](#english) · [简体中文](#简体中文)

OpenRTL 持续发布 **MIT 许可的硬件加速器**，把算法变成可复用的 RTL，
为 ASIC 与 FPGA 系统开发者提供已发布设计和可检查的工程证据。

[浏览已发布加速器](#已发布项目) · [了解工程质量](#工程质量) ·
[讨论 ASIC/FPGA 定制开发](https://openrtl.top/)

## 已发布项目

从系列索引进入，查找已发布的加速器和工程证据。新系列在正式发布后加入本页。

| 已发布系列 | 覆盖方向 | 索引 |
| --- | --- | --- |
| ZK 硬件加速器 | Goldilocks 有限域运算；NTT/INTT、LDE、FRI、Sumcheck/MLE；Poseidon2、Merkle 运算；BN254-G1 MSM | [浏览 ZK 加速器目录](https://github.com/OpenRTL-Lab/zk-accelerators) |

ZK 系列提供独立的 Chisel 加速器、生成好的 SystemVerilog 和原生接口，
供用户集成到 ASIC 或 FPGA 设计。系列索引链接至各模块的版本、源码、发布产物、
接口与数学模型文档、参考模型及测试。
模块的具体版本和测量结果由系列索引及对应仓库维护，不在组织首页重复罗列。

支持的配置、验证范围、性能测量和综合条件以各独立项目的文档为准。
这些是独立计算模块，不是端到端零知识证明生成系统。

## 工程原则

- **可读的 RTL**：结构清晰，行为有文档可查。
- **可复现的验证**：提供参考模型、测试说明，并明确工具链要求。
- **明确的接口与验证边界**：说明协议、支持的配置和已报告结果的覆盖范围。
- **容易移植**：保持可复用的模块边界，明确依赖和集成要求，便于适配不同目标系统。

## 工程质量

我们以**商业级性能与稳定性**为工程目标：让计算模块不仅能够演示算法，
还便于评估、集成和维护。已发布作品是可供检查的工程能力证明，
并不代表所有设计都已完成面向所有应用的量产认证。

评估具体模块时，请沿仓库和 Release 文档查看：

- **正确性与稳定性证据**：参考模型对照、已测配置、协议与边界场景覆盖、已知限制。
- **有条件的性能数据**：工作负载、周期、吞吐、延迟、资源消耗，以及已报告的工具版本
  和目标综合条件。仿真、综合与板级或硅后实测应分别理解。
- **可复现与可集成性**：版本化 RTL、验证步骤、接口约定、依赖和移植约束。

验证结论以相应版本、配置和目标为边界；可集成到 ASIC/FPGA，
不等于每个设计均已流片、完成上板测试或适合任意应用。

## ASIC/FPGA 定制开发

如果你需要适配特定工作负载或系统的硬件加速器，欢迎通过
[OpenRTL Lab 官方网站](https://openrtl.top/)查看服务介绍和联系方式，
讨论 **ASIC/FPGA 加速器定制开发与集成**。
上述已发布作品可作为评估技术适配性和工程能力的起点。

可讨论的项目范围包括算法到 RTL 实现、数据通路与存储架构定制、接口适配、
性能与资源优化，以及按约定需求开展验证。
具体交付物、目标平台支持、验证范围和时间安排按项目另行确认。

初步需求建议说明：算法与工作负载、ASIC 工艺或 FPGA 器件、接口、
吞吐与延迟目标、面积与功耗约束、验证要求和交付时间。
保密规格请通过另行约定的私密渠道交流，不要提交到公开 GitHub Issue。

## 开源许可

OpenRTL 自研项目代码采用 **MIT 许可证**发布。
各仓库中的文件及依赖以相应仓库的许可证和第三方声明为准。

使用 MIT 许可代码进行商业用途，不以购买定制服务为前提。
付费定制与支持是独立、可选的服务。
