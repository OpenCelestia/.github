# Celestia

面向安凯微（Anyka）视觉 SoC 的应用软件平台。

Celestia 跑在安凯微影像 SoC 的厂商 SDK 之上。固定五层（应用、框架、硬件适配、系统基础、内核与板级），产品差异只来自 `project/<product>/config.mk`。面向摄像机、AI 眼镜、平板、穿戴。嵌入式 C / C++，支持 Linux 与 AOS RTOS。

本组织是发布源，默认分支 `main`。同一批提交的镜像在 [Gitee](https://gitee.com/OpenCelestia)。

自有源码使用 Apache-2.0，文档使用 CC BY 4.0。`third_party` 遵循各上游许可证。`project` 中随仓提供的厂商二进制、模型、字库和烧录镜像不属于 Apache-2.0。芯片 SDK 不在这些仓库中，需另行获取。

文档：[中文](https://github.com/OpenCelestia/docs/blob/main/README.md) · [English](https://github.com/OpenCelestia/docs/blob/main/README.en.md)

整树下载：

```bash
repo init -u https://github.com/OpenCelestia/manifest.git -b main -m default.xml
repo sync -c -j4
```

从 Gitee 下载须使用 `gitee.xml`。使用 `default.xml` 时，仓库仍会从 GitHub 拉取。

`system/core` 的仓库名是 `core`。

---

## English

Image software stack for Anyka image SoCs.

Celestia sits on the Anyka image SoC vendor SDK. Five fixed layers (application, framework, hardware adaptation, system base, kernel and board) are separated by one configuration entry: each product's `config.mk` under `project`. The same tree targets cameras, AI glasses, tablets, and wearables. Embedded C/C++, Linux and AOS RTOS.

This organization is the publication source. The default branch is `main`. [Gitee](https://gitee.com/OpenCelestia) mirrors the same commits.

First-party source is Apache-2.0. Documentation is CC BY 4.0. `third_party` follows each upstream license. Vendor binaries, models, fonts, and burn images shipped in `project` are not Apache-2.0. The chip SDK is not in these repositories.

Docs: [English](https://github.com/OpenCelestia/docs/blob/main/README.en.md) · [中文](https://github.com/OpenCelestia/docs/blob/main/README.md)

```bash
repo init -u https://github.com/OpenCelestia/manifest.git -b main -m default.xml
repo sync -c -j4
```

Download the full tree from Gitee with `gitee.xml`. Using `default.xml` still fetches the repositories from GitHub.

The `system/core` tree is published as the repository named `core`.
