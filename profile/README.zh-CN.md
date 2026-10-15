<img src="https://raw.githubusercontent.com/OpenRTL-Lab/.github/main/assets/openrtl-logo.png?v=2" width="96" height="96" alt="OpenRTL 像素 Logo：亮蓝色芯片与黄色闪电">

# OpenRTL

**从算法到 RTL，构建开放、可复用、可验证的数字硬件。**

[English](https://github.com/OpenRTL-Lab/.github/blob/main/profile/README.md) · 简体中文

OpenRTL 发布开放、可复用、可验证的数字硬件，注重可读的 RTL、实际集成需求，以及
可供使用者检查和复现的验证证据。

## 已发布项目

### [ZK 硬件加速器集合](https://github.com/OpenRTL-Lab/zk-accelerators)

涵盖 **11 类独立的 Chisel 零知识计算加速器**，提供生成好的 SystemVerilog，
通过原生接口供用户集成到 ASIC 或 FPGA 设计。

| 方向 | 加速器 |
| --- | --- |
| 有限域运算 | Goldilocks 素域与二次扩域向量运算、批量求逆 |
| 多项式计算 | NTT/INTT、陪集 LDE、FRI 折叠、Sumcheck 与 MLE |
| 哈希与承诺 | Poseidon2 置换、海绵哈希、Merkle 运算 |
| 椭圆曲线计算 | BN254-G1 多标量乘法 |

通过[加速器目录](https://github.com/OpenRTL-Lab/zk-accelerators)可查阅各模块的
版本、源码、发布产物、接口与数学模型文档、参考模型及仿真测试。
版本化发布示例：[Goldilocks NTT/INTT v1.1.0](https://github.com/XLxiaoliaoGmail/goldilocks-ntt-intt/releases/tag/v1.1.0)。

支持的配置、验证范围、性能测量和综合条件以各独立项目的文档为准。
这些是独立计算模块，不是端到端零知识证明生成系统。

## 工程原则

- **可读的 RTL**：结构清晰，行为有文档可查。
- **可复现的验证**：提供参考模型、测试说明，并明确工具链要求。
- **明确的接口与验证边界**：说明协议、支持的配置和已报告结果的覆盖范围。
- **容易移植**：保持可复用的模块边界，明确依赖和集成要求，便于适配不同目标系统。

## 开源许可

OpenRTL 自研项目代码采用 **MIT 许可证**发布。
各仓库中的文件及依赖以相应仓库的许可证和第三方声明为准。
