# `thumbv7m-none-eabi`

**Tier: 2**

Bare-metal target for CPUs in the [ARMv7-M] architecture family, supporting a subset of the [T32 ISA][t32-isa].

Processors in this family include the:

* [Arm Cortex-M3][cortex-m3]

See [`arm-none-eabi`](arm-none-eabi.md) for information applicable to all `arm-none-eabi` targets.

This target uses the soft-float ABI: functions which take `f32` or `f64` as arguments will have those values packed into an integer registers. This is the only option because there is no FPU support in [ARMv7-M].

[t32-isa]: https://developer.arm.com/Architectures/T32%20Instruction%20Set%20Architecture
[ARMv7-M]: https://developer.arm.com/documentation/ddi0403/latest/
[cortex-m3]: https://developer.arm.com/Processors/Cortex-M3

## Target maintainers

* [Rust Embedded Devices Working Group Cortex-M Team](https://github.com/rust-embedded), `cortex-m@teams.rust-embedded.org`

## Target CPU and Target Feature options

TODO

## Cross-compilation toolchains and C code

This target supports C code compiled with the `arm-none-eabi` target triple and `-march=armv6-m` or a suitable `-mcpu` flag.
