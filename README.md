![Elsa — Embedded software, EV charging, and hardware security](assets/profile-banner.svg)

# Elsa · Embedded Software Engineer

**EV charging systems · Real-time firmware · Hardware-backed security**

**English** · [简体中文](README.zh-CN.md)

I develop embedded software for EV charging systems, from MCU drivers and RTOS applications to charging communication and secure-element integration. I care about clear interfaces, reproducible builds, and firmware that can be tested beyond the target board.

My current open-source work covers EV charging communication experiments, cryptographic middleware, and practical tools for embedded development.

## Selected work

### [V2ICP Lab · VDV 261](https://github.com/Elsa-is-My-Muse/v2icp-lab)

A local **VDV 261 / V2ICP** learning and integration lab that runs a simulated EVCC, a relay for encrypted bytes, and a backend on one machine, using real **IPv6, TLS, and HTTP** communication over loopback.

- Browser dashboard with live vehicle/backend inputs, automatic cycles, and step-by-step exchanges.
- Fault injection, event inspection, and redacted JSON report export for reproducible experiments.
- Illustrative C interfaces and hardware integration references for exploring EVCC / SECC integration.

[Source](https://github.com/Elsa-is-My-Muse/v2icp-lab) · [Usage & scope](https://github.com/Elsa-is-My-Muse/v2icp-lab/blob/master/README.en.md) · [Integration references](https://github.com/Elsa-is-My-Muse/v2icp-lab/blob/master/docs/hardware-integration.md)

### [SE050E Crypto Middleware](https://github.com/Elsa-is-My-Muse/se050e-crypto-middleware)

Portable C99 cryptographic middleware for the **NXP SE050E** secure element, with a **PSA Crypto / Mbed TLS** integration layer and an **AT32F435 + RT-Thread** reference port.

- Session and key management, ECDSA signing, and optional ECDH support.
- Explicit OS and board interfaces, host-based mocks, and source-export integrity checks.
- Automated validation on Linux GCC, Linux Clang, and Windows MinGW.

[Source](https://github.com/Elsa-is-My-Muse/se050e-crypto-middleware) · [Integration guide](https://github.com/Elsa-is-My-Muse/se050e-crypto-middleware/blob/main/README.en.md) · [Builds](https://github.com/Elsa-is-My-Muse/se050e-crypto-middleware/actions/workflows/ci.yml)

[![SE050E middleware CI](https://github.com/Elsa-is-My-Muse/se050e-crypto-middleware/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/Elsa-is-My-Muse/se050e-crypto-middleware/actions/workflows/ci.yml)

### [Keil Builder](https://github.com/Elsa-is-My-Muse/keil_builder)

A Python command-line tool for automating **Keil MDK** builds on Windows. It discovers project files, supports configurable build targets, streams build output, and collects logs and firmware artifacts.

[Source & usage](https://github.com/Elsa-is-My-Muse/keil_builder#readme)

## Technical focus

| Area | Focus |
| --- | --- |
| Embedded firmware | C / C++, ARM Cortex-M, STM32, AT32, RT-Thread, FreeRTOS |
| EV charging communication | OCPP 1.6, ISO 15118, DIN 70121, VDV 261 / V2ICP, EVCC / SECC integration |
| Cryptography & secure elements | NXP SE050E, PSA Crypto, Mbed TLS, key and certificate integration |
| Build & verification | Python, CMake, Keil MDK, GCC / Clang, GitHub Actions, host-based tests |

## Engineering approach

- Keep hardware-specific code behind explicit port interfaces.
- Document supported configurations and integration requirements.
- Make builds and checks repeatable across development environments.
- Describe limitations alongside capabilities.

## Get in touch

For technical questions, integration feedback, or collaboration ideas, open an issue in the relevant project:

[V2ICP Lab](https://github.com/Elsa-is-My-Muse/v2icp-lab/issues) · [SE050E middleware](https://github.com/Elsa-is-My-Muse/se050e-crypto-middleware/issues) · [Keil Builder](https://github.com/Elsa-is-My-Muse/keil_builder/issues)
