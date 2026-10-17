[English](https://github.com/OpenRTL-Lab/.github/blob/main/profile/README.md) · 简体中文

<picture>
  <source media="(prefers-reduced-motion: reduce)" srcset="https://raw.githubusercontent.com/OpenRTL-Lab/.github/main/assets/openrtl-logo.png?v=4">
  <img src="https://raw.githubusercontent.com/OpenRTL-Lab/.github/main/assets/openrtl-logo.gif?v=4" width="128" height="128" alt="OpenRTL 绿色像素芯片：提取自 RapidRTL 首页原画">
</picture>

# OpenRTL — MIT 开源数字硬件

**从算法到 RTL，构建面向商业应用的高性能、稳定可靠的数字硬件。**

[官方网站](https://openrtl.top/)

OpenRTL 持续发布采用 MIT 许可的自研数字硬件，涵盖计算加速器、控制器与接口模块，
提供可复用的 RTL、可复现的验证和可检查的工程证据。

面向 ASIC 与 FPGA，我们提供可复用设计，以及可选的定制开发与集成服务。

[浏览已发布项目](#已发布项目) · [了解工程质量](#工程质量) ·
[讨论 ASIC/FPGA 定制开发](https://openrtl.top/)

## 已发布项目

从系列索引进入，查找已发布的硬件设计和工程证据。新系列在正式发布后加入本页。

| 已发布系列 | 覆盖方向 | 索引 |
| --- | --- | --- |
| ZK 硬件加速器 | Goldilocks 有限域运算；NTT/INTT、LDE、FRI、Sumcheck/MLE；Poseidon2、Merkle 运算；BN254-G1 MSM | [浏览 ZK 加速器目录](https://github.com/OpenRTL-Lab/zk-accelerators) |
| OpenETH | 千兆以太网控制器与 DMA；整帧缓存与跨时钟域；MAC/CRC、RGMII、PHY 管理；Linux 驱动与测试程序 | [浏览 OpenETH 系列](https://github.com/OpenRTL-Lab/openeth/blob/main/README.zh-CN.md) |

ZK 系列提供独立的 Chisel 加速器、生成好的 SystemVerilog 和原生接口，
供用户集成到 ASIC 或 FPGA 设计。系列索引链接至各模块的版本、源码、发布产物、
接口与数学模型文档、参考模型及测试。

OpenETH 提供可复用的以太网 RTL 与软件，包括 Chisel 和 SystemVerilog 源码、
接口文档、仿真测试及有记录的参考板验证。千兆以太网指接口规格，实际应用吞吐
和交付范围以仓库文档为准。

模块的具体版本和测量结果由各系列及对应仓库维护，不在组织首页重复罗列。

支持的配置、验证范围、性能测量和综合条件以各独立项目的文档为准。
ZK 系列中的计算模块相互独立，并非端到端零知识证明生成系统。

## 工程原则

- **可读的 RTL**：结构清晰，行为有文档可查。
- **可复现的验证**：提供参考模型、测试说明，并明确工具链要求。
- **明确的接口与验证边界**：说明协议、支持的配置和已报告结果的覆盖范围。
- **容易移植**：保持可复用的模块边界，明确依赖和集成要求，便于适配不同目标系统。

## 工程质量

我们以**商业级性能与稳定性**为工程目标：让数字硬件设计不仅能够演示算法，
还便于评估、集成和维护。已发布作品是可供检查的工程能力证明，
并不代表所有设计都已完成面向所有应用的量产认证。

评估具体模块时，请沿仓库和发布文档查看：

- **正确性与稳定性证据**：参考模型对照、已测配置、协议与边界场景覆盖、已知限制。
- **有条件的性能数据**：工作负载、周期、吞吐、延迟、资源消耗，以及已报告的工具版本
  和目标综合条件。仿真、综合与板级或硅后实测应分别理解。
- **可复现与可集成性**：版本化 RTL、验证步骤、接口约定、依赖和移植约束。

验证结论以相应版本、配置和目标为边界；可集成到 ASIC/FPGA，
不等于每个设计均已流片、完成上板测试或适合任意应用。

## ASIC/FPGA 定制开发

如果你需要适配特定工作负载或系统的数字硬件，欢迎通过
[OpenRTL Lab 官方网站](https://openrtl.top/)查看服务介绍和联系方式，
讨论 **ASIC/FPGA 数字硬件定制开发与集成**。
上述已发布作品可作为评估技术适配性和工程能力的起点。

可讨论的项目范围包括算法到 RTL 实现、数据通路与存储架构定制、接口适配、
性能与资源优化，以及按约定需求开展验证。
具体交付物、目标平台支持、验证范围和时间安排按项目另行确认。

初步需求建议说明：算法与工作负载、ASIC 工艺或 FPGA 器件、接口、
吞吐与延迟目标、面积与功耗约束、验证要求和交付时间。
保密规格请通过另行约定的私密渠道交流，不要提交到公开 GitHub 议题。

## 开源许可

OpenRTL 自研项目代码采用 **MIT 许可证**发布。
各仓库中的文件及依赖以相应仓库的许可证和第三方声明为准。

使用 MIT 许可代码进行商业用途，不以购买定制服务为前提。
付费定制与支持是独立、可选的服务。
