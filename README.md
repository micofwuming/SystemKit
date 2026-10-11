SystemKit (adpated)
=========

A fork of [gao-sun/SystemKit](https://github.com/gao-sun/SystemKit) with bug
fixes, used by [eul](https://github.com/micofwuming/eul).

A macOS system library in Swift based off of
[libtop](https://github.com/apple-oss-distributions/top/blob/top-100.1.2/libtop.c), from
Apple's top implementation.

- For an example usage of this library, see
  [dshb](https://github.com/beltex/dshb), a macOS system monitor in Swift
- For other system related statistics in Swift for macOS, see
  [SMCKit](https://github.com/beltex/SMCKit)


### Requirements

- [Latest Xcode](https://developer.apple.com/xcode/resources/)
- macOS 12.0+

### Installation

#### Swift Package Manager

To integrate SystemKit using [Swift Package Manager](https://github.com/swiftlang/swift-package-manager), add it to the dependencies in your Package.swift:

    .package(url: "https://github.com/micofwuming/SystemKit", from: "0.0.13")

### Example

Sample ouput from
[example](https://github.com/beltex/SystemKit/blob/master/Example/main.swift).

```
// MACHINE STATUS

-- CPU --
  PHYSICAL CORES:  2
  LOGICAL CORES:   2
  SYSTEM:          10%
  USER:            17%
  IDLE:            71%
  NICE:            0%

-- MEMORY --
  PHYSICAL SIZE:   7.75GB
  FREE:            1.33GB
  WIRED:           866MB
  ACTIVE:          5.04GB
  INACTIVE:        516MB
  COMPRESSED:      0MB

-- SYSTEM --
  MODEL:           MacBookPro7,1
  SYSNAME:         Darwin
  NODENAME:        beltex.local
  RELEASE:         13.4.0
  VERSION:         Darwin Kernel Version 13.4.0: Sun Aug 17 19:50:11 PDT 2014...
  MACHINE:         x86_64
  UPTIME:          6d 21h 4m 38s
  PROCESSES:       197
  THREADS:         967
  LOAD AVERAGE:    [3.18, 3.89, 3.99]
  MACH FACTOR:     [0.436, 0.385, 0.322]

-- POWER --
  CPU SPEED LIMIT: 100.0%
  CPUs AVAILABLE:  2
  SCHEDULER LIMIT: 100.0%
  THERMAL LEVEL:   Not Published

-- BATTERY --
  AC POWERED:      true
  CHARGED:         true
  CHARGING:        false
  CHARGE:          100.0%
  CAPACITY:        1675 mAh
  MAX CAPACITY:    1675 mAh
  DESGIN CAPACITY: 5450 mAh
  CYCLES:          646
  MAX CYCLES:      1000
  TEMPERATURE:     30.0°C
  TIME REMAINING:  0:45
```


### References

- [top](https://github.com/apple-oss-distributions/top)
- [hostinfo](https://github.com/apple-oss-distributions/system_cmds)
- [vm_stat](https://github.com/apple-oss-distributions/system_cmds)
- [PowerManagement](https://github.com/apple-oss-distributions/PowerManagement)
- iStat Pro


### License

This project is under the **MIT License**.
