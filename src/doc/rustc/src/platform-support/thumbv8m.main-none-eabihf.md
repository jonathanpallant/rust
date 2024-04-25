# `thumbv8m.main-none-eabihf`

**Tier: 2**

Bare-metal target for CPUs in the Mainline [ARMv8-M] architecture family, supporting a subset of the [T32 ISA][t32-isa].

Processors in this family include the:

* [Arm Cortex-M33F][cortex-m33]
* [Arm Cortex-M55F][cortex-m55]
* [Arm Cortex-M85F][cortex-m85]

See [`arm-none-eabi`](arm-none-eabi.md) for information applicable to all `arm-none-eabi` targets.

This target uses the hard-float ABI: functions which take `f32` or `f64` as arguments will have them passed via FPU registers. This target therefore requires the use of an FPU (which is optional on Cortex-M33, Cortex-M55 and Cortex-M85). See also the soft-float ABI version of this target [`thumbv8m.main-none-eabi`](thumbv8m.main-none-eabi.md).

[t32-isa]: https://developer.arm.com/Architectures/T32%20Instruction%20Set%20Architecture
[ARMv8-M]: https://developer.arm.com/documentation/ddi0553/latest/
[cortex-m33]: https://developer.arm.com/Processors/Cortex-M33
[cortex-m55]: https://developer.arm.com/Processors/Cortex-M55
[cortex-m85]: https://developer.arm.com/Processors/Cortex-M85

## Target maintainers

* [Rust Embedded Devices Working Group Cortex-M Team](https://github.com/rust-embedded), `cortex-m@teams.rust-embedded.org`

## Target CPU and Target Feature options

TODO

## Cross-compilation toolchains and C code

This target supports C code compiled with the `arm-none-eabi` target triple and `-march=armv6-m` or a suitable `-mcpu` flag.
