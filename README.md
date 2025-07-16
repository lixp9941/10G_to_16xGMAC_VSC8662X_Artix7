# 10G 万兆网 → 16路千兆以太网转发系统

本项目基于 Xilinx Artix-7 FPGA 实现一个 10G 以太网帧解析与分发系统，支持将输入帧根据字段内容转发至 16 个千兆以太网端口。

## 结构说明

- `doc/`：文档资料
- `hw/`：硬件设计（KiCad 原理图、PCB、BOM）
- `fpga/`：FPGA 工程（Vivado 设计、IP 核、约束文件）
- `sw/`：软件配置代码（MDIO 寄存器配置、测试脚本）
- `tools/`：工具与模板

## 目标芯片

- FPGA：Xilinx Artix-7 XC7A100T
- SerDes：Marvell 88X5113
- PHY：Microsemi VSC8662X × 2（每片 8 端口）