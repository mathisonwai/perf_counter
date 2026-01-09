# Response to PD PHY MCU Inquiry / 关于PD PHY MCU咨询的回复

## Important Notice / 重要提示

**English**: This repository (perf_counter) is a performance measurement library for embedded systems, not a hardware recommendation or procurement resource. The questions below appear to be posted in the wrong repository.

**中文**: 本仓库 (perf_counter) 是一个嵌入式系统性能测量库，而不是硬件推荐或采购资源。以下问题似乎发布在了错误的仓库中。

---

## Original Questions / 原始问题

The following questions were raised regarding USB Power Delivery PHY MCUs:

1. 求推荐最便宜的带PD PHY的MCU，要便宜的，请带上价格
2. 应用情景：诱骗器，替代芯海 34P16（要停产了），能写代码用188数码管显示电流、电压的
3. 最好是寄存器开放的，沁恒543D代理给我报价 1.8元，太贵了，没法玩！
4. 沁恒 CHX032大家能拿到的价格，准备用它做一个项目，问了一圈居然要2.4以上，期待的价格1.5元左右
5. 不带PD PHY 的芯片需要什么资源才能软解 PD协议

**Translation**:
1. Request for the cheapest MCU with PD PHY, with pricing
2. Application: PD trigger/decoy device to replace Sinowealth 34P16 (being discontinued), capable of displaying current and voltage on a 7-segment display
3. Preferably with open registers; WCH 543D quoted at 1.8 yuan, too expensive
4. What price can people get for WCH CHX032? Planning to use it for a project, quotes are above 2.4 yuan, expecting around 1.5 yuan
5. What resources are needed to implement PD protocol in software on chips without PD PHY?

---

## Why This Is Not Appropriate Here / 为什么这些问题不适合在此处提出

**English**: This repository is focused on software performance measurement, not hardware selection or purchasing. Questions about MCU recommendations, pricing, and hardware alternatives should be directed to appropriate forums and communities.

**中文**: 本仓库专注于软件性能测量，而非硬件选型或采购。关于MCU推荐、价格和硬件替代方案的问题应该在适当的论坛和社区中提出。

---

## Where to Ask These Questions / 应该在哪里提问

### Recommended Chinese Communities / 推荐的中文社区

1. **电子工程世界 (EEWorld)**: https://bbs.eeworld.com.cn/
   - 专门的MCU和嵌入式系统板块
   - 活跃的工程师社区

2. **21ic电子技术论坛**: https://bbs.21ic.com/
   - MCU和电源管理讨论区
   - 器件选型经验分享

3. **沁恒官方技术支持**:
   - 对于CHX032和543D等沁恒芯片的具体问题
   - 可以获得官方的技术支持和价格信息

4. **立创社区**: https://club.szlcsc.com/
   - 元器件采购和选型讨论
   - 价格比较和供应链信息

5. **知乎 - 硬件/嵌入式话题**:
   - 搜索"USB PD"、"MCU选型"等话题
   - 工程师经验分享

### International Communities / 国际社区

1. **EEVblog Forum**: https://www.eevblog.com/forum/
2. **Electronics StackExchange**: https://electronics.stackexchange.com/
3. **Reddit r/embedded**: https://www.reddit.com/r/embedded/

---

## General Guidance on Your Questions / 关于您问题的一般性指导

### For PD PHY MCU Selection / 关于PD PHY MCU选型

**Considerations / 考虑因素**:
- **Cost vs. Features / 成本与功能**: Lower-cost MCUs may have limited features or require external components
- **Development Ecosystem / 开发生态**: SDK availability, documentation quality, community support
- **Supply Chain / 供应链**: Long-term availability, multiple sourcing options
- **Compliance / 合规性**: USB-IF certification requirements for commercial products

### Alternative Approaches / 替代方案

1. **Discrete PD Controller + Low-cost MCU**:
   - Use a dedicated PD controller chip (like IP2721, CH224K)
   - Pair with a very low-cost MCU for display and control logic
   - May be cheaper than integrated PD PHY MCU

2. **Software PD Implementation**:
   - Requires precise timing control (BMC encoding)
   - Typically needs SPI or high-speed GPIO
   - Comparator for voltage detection
   - This is complex and may not be cost-effective for simple projects

3. **Pre-certified Modules**:
   - Some vendors offer pre-certified PD trigger modules
   - Can simplify development and compliance

---

## About This Repository / 关于本仓库

**perf_counter** is for:
- Measuring CPU cycle counts in embedded applications
- Profiling code performance
- Timestamp and timing utilities
- Performance optimization

**perf_counter** 用于:
- 测量嵌入式应用中的CPU周期数
- 分析代码性能
- 时间戳和计时工具
- 性能优化

For performance measurement in your PD trigger device project, you're welcome to use this library to optimize your code!

如果您在PD诱骗器项目中需要性能测量，欢迎使用本库来优化您的代码！

---

## Disclaimer / 免责声明

This document is provided for informational purposes only. No specific hardware recommendations or pricing information is provided, as this is outside the scope of this software library project.

本文档仅供参考。由于超出本软件库项目的范围，不提供具体的硬件推荐或价格信息。
