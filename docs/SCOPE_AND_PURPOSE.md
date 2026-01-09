# Repository Scope and Purpose

## About This Repository

The **perf_counter** repository is a performance measurement library for microcontrollers, specifically designed for:

- **Measuring CPU cycles** for code segments
- **Performance analysis** (CPU usage, CPI, cache miss rates)
- **Timestamp services** for embedded applications
- **Timer utilities** for ARM Cortex-M processors

This library does **NOT** provide:
- Hardware recommendations or procurement advice
- MCU selection guidance
- Pricing information for microcontrollers
- USB Power Delivery (PD) PHY implementation
- Protocol implementation guidance

## Common Misconceptions

### This is NOT a Hardware Recommendation Forum

If you're looking for:
- MCU recommendations with specific peripherals (like PD PHY)
- Pricing information for microcontrollers
- Alternative chip suggestions
- Hardware procurement advice

Please consider these resources instead:
- **Electronic Design Forums**: EEVblog, Electronics Stack Exchange
- **Chinese Electronics Communities**: EEWorld (电子工程世界), 21ic论坛
- **Manufacturer Communities**: WCH (沁恒) official forums, Silicon Labs forums
- **Distributor Resources**: LCSC, Mouser, DigiKey product selection guides

## What This Library Does

perf_counter is a **software library** that helps you:
1. Measure performance of your embedded code
2. Analyze CPU usage in real-time
3. Profile execution time of functions
4. Get accurate timestamps in embedded systems

## For USB PD PHY MCU Inquiries

If you're specifically looking for:
- **PD PHY MCU recommendations**
- **Pricing for CHX032 or similar chips**
- **Alternatives to Sinowealth 34P16**
- **Software PD protocol implementation**

These questions should be directed to:
1. Manufacturer application engineers
2. Electronic design communities (see resources above)
3. Your local distributors or representatives
4. Specialized forums for power electronics

## Contributing to This Repository

If you want to contribute to perf_counter:
- Report bugs in the performance measurement code
- Suggest improvements to timing accuracy
- Add support for new processor architectures
- Improve documentation for the library features

Please ensure your contributions align with the repository's purpose: **performance measurement for embedded systems**.
