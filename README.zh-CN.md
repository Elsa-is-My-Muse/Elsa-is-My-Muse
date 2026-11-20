![Elsa — 嵌入式软件、EV 充电通信与硬件安全](assets/profile-banner.svg)

# Elsa · 嵌入式软件工程师

**EV 充电系统 · 实时固件 · 硬件安全**

[English](README.md) · **简体中文**

我从事 EV 充电系统的嵌入式软件开发，工作涉及 MCU 驱动、RTOS 应用、充电通信协议与安全芯片集成。我关注清晰的模块接口、可复现的构建流程，以及能够脱离目标板进行验证的固件设计。

目前的开源工作主要围绕密码学中间件和嵌入式开发工具展开。

## 代表项目

### [SE050E Crypto Middleware](https://github.com/Elsa-is-My-Muse/se050e-crypto-middleware)

面向 **NXP SE050E** 安全芯片的可移植 C99 密码学中间件，提供 **PSA Crypto / Mbed TLS** 适配层，以及 **AT32F435 + RT-Thread** 参考移植。

- 会话与密钥管理、ECDSA 签名，以及可选的 ECDH 支持。
- 明确的 OS 与板级接口、主机端 mock 测试和源码导出完整性检查。
- 在 Linux GCC、Linux Clang 和 Windows MinGW 上执行自动化验证。

[源码](https://github.com/Elsa-is-My-Muse/se050e-crypto-middleware) · [集成说明](https://github.com/Elsa-is-My-Muse/se050e-crypto-middleware/blob/main/README.md) · [构建记录](https://github.com/Elsa-is-My-Muse/se050e-crypto-middleware/actions/workflows/ci.yml)

[![SE050E 中间件 CI](https://github.com/Elsa-is-My-Muse/se050e-crypto-middleware/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/Elsa-is-My-Muse/se050e-crypto-middleware/actions/workflows/ci.yml)

### [Keil Builder](https://github.com/Elsa-is-My-Muse/keil_builder)

用于 Windows 平台 **Keil MDK** 工程构建自动化的 Python 命令行工具，支持工程文件发现、构建目标配置、实时输出，以及日志和固件产物收集。

[源码与使用说明](https://github.com/Elsa-is-My-Muse/keil_builder#readme)

## 技术方向

| 方向 | 关注内容 |
| --- | --- |
| 嵌入式固件 | C / C++、ARM Cortex-M、STM32、AT32、RT-Thread、FreeRTOS |
| EV 充电通信 | OCPP 1.6、ISO 15118、DIN 70121、EVCC / SECC 集成 |
| 密码学与安全芯片 | NXP SE050E、PSA Crypto、Mbed TLS、密钥与证书集成 |
| 构建与验证 | Python、CMake、Keil MDK、GCC / Clang、GitHub Actions、主机端测试 |

## 工程实践

- 通过明确的移植接口隔离硬件相关代码。
- 说明支持的配置与集成要求。
- 让构建和检查能够在不同开发环境中重复执行。
- 在介绍能力的同时说明使用边界。

## 交流与反馈

欢迎围绕技术问题、集成反馈或合作想法，在对应项目中发起 Issue：

[SE050E 中间件](https://github.com/Elsa-is-My-Muse/se050e-crypto-middleware/issues) · [Keil Builder](https://github.com/Elsa-is-My-Muse/keil_builder/issues)
