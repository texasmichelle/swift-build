# **//swift/build**

The `//swift/build` project provides a CI configuration for [Azure 
Pipelines](https://azure.microsoft.com/en-us/services/devops/pipelines/) that allows 
building Swift for multiple platforms. The configuration is not specific to Azure, 
and can be reused for developer builds as well. Thanks to modular packaging, with 
`//swift/build` you can easily cross-compile your Swift code for Android and Windows 
targets, or build on Windows natively without cross-compilation.

## Table of Contents

- [**//swift/build**](#--swift-build---)
  * [Getting Started (Docker)](docs/GettingStartedDocker.md)
  * [Getting Started (Native)](docs/GettingStartedWindows.md)
  * [Status](#status)
  * [Getting the latest build](#Getting-the-latest-build)

## Status

**Dependencies**

| Build | Status |
| :-: | --- |
| **CURL** | [![Build Status](https://compnerd.visualstudio.com/swift-build/_apis/build/status/CURL?branchName=main)](https://compnerd.visualstudio.com/swift-build/_build/latest?definitionId=11&branchName=main) |
| **ICU** | [![Build Status](https://compnerd.visualstudio.com/swift-build/_apis/build/status/ICU?branchName=main)](https://compnerd.visualstudio.com/swift-build/_build/latest?definitionId=9&branchName=main) |
| **SQLite3** | [![Build Status](https://compnerd.visualstudio.com/swift-build/_apis/build/status/SQLite?branchName=main)](https://compnerd.visualstudio.com/swift-build/_build/latest?definitionId=12&branchName=main) |
| **TensorFlow** | [![Build Status](https://dev.azure.com/compnerd/swift-build/_apis/build/status/tensorflow?branchName=main)](https://dev.azure.com/compnerd/swift-build/_build/latest?definitionId=44&branchName=main) |
| **XML2** | [![Build Status](https://compnerd.visualstudio.com/swift-build/_apis/build/status/XML2?branchName=main)](https://compnerd.visualstudio.com/swift-build/_build/latest?definitionId=10&branchName=main) |
| **ZLIB** | [![Build Status](https://compnerd.visualstudio.com/swift-build/_apis/build/status/zlib?branchName=main)](https://compnerd.visualstudio.com/swift-build/_build/latest?definitionId=16&branchName=main) |

**Swift 5.2**

| Build | Status |
| :-: | --- |
| **VS2019** | [![Build Status](https://compnerd.visualstudio.com/swift-build/_apis/build/status/VS2019%20Swift%205.2?branchName=main)](https://compnerd.visualstudio.com/swift-build/_build/latest?definitionId=43&branchName=main) |

<details>
  <summary>Build Contents</summary>

  - **VS2019**
    - *Toolchain (llvm, clang, lld, lldb, swift)*
      - ARM64
      - x64
    - *Swift SDK for Android (swift, libdispatch, foundation, xctest)*
      - ARM
      - ARM64
      - x64
      - x86
    - *Swift SDK for Windows (swift, libdispatch, foundation, xctest)*
      - ARM
      - ARM64
      - x64
      - x86
 </details>

**Swift 5.3**

| Build | Status |
| :-: | --- |
| **VS2019** | [![Build Status](https://dev.azure.com/compnerd/swift-build/_apis/build/status/VS2019%205.3?branchName=main)](https://dev.azure.com/compnerd/swift-build/_build/latest?definitionId=53&branchName=main) |

**Swift HEAD (Development)**

| Build | Status |
| :-: | --- |
| **macOS** | [![Build Status](https://dev.azure.com/compnerd/swift-build/_apis/build/status/macOS?branchName=main)](https://dev.azure.com/compnerd/swift-build/_build/latest?definitionId=15&branchName=main) |
| **VS2017** | [![Build Status](https://dev.azure.com/compnerd/swift-build/_apis/build/status/VS2017?branchName=main)](https://dev.azure.com/compnerd/swift-build/_build/latest?definitionId=1&branchName=main) |
| **VS2019** | [![Build Status](https://dev.azure.com/compnerd/swift-build/_apis/build/status/VS2019?branchName=main)](https://dev.azure.com/compnerd/swift-build/_build/latest?definitionId=7&branchName=main) |
| **VS2017 (Facebook)** | [![Build Status](https://compnerd.visualstudio.com/swift-build/_apis/build/status/VS2017%20Swift%20(Facebook)?branchName=main)](https://compnerd.visualstudio.com/swift-build/_build/latest?definitionId=5&branchName=main) |
| **VS2019 (Facebook)** | [![Build Status](https://compnerd.visualstudio.com/swift-build/_apis/build/status/VS2019%20Swift%20(Facebook)?branchName=main)](https://compnerd.visualstudio.com/swift-build/_build/latest?definitionId=31&branchName=main) |
| **Ubuntu 18.04 (flowkey)** | [![Build Status](https://compnerd.visualstudio.com/swift-build/_apis/build/status/Ubuntu%2018.04%20(flowkey)?branchName=main)](https://compnerd.visualstudio.com/swift-build/_build/latest?definitionId=14&branchName=main) |
| **macOS (TensorFlow)** | [![Build Status](https://dev.azure.com/compnerd/swift-build/_apis/build/status/macOS%20Swift%20TensorFlow?branchName=main)](https://dev.azure.com/compnerd/swift-build/_build/latest?definitionId=47&branchName=main) |
| **VS2019 (TensorFlow)**| [![Build Status](https://dev.azure.com/compnerd/swift-build/_apis/build/status/VS2019%20Swift%20TensorFlow%20(Google)?branchName=main)](https://dev.azure.com/compnerd/swift-build/_build/latest?definitionId=46&branchName=main) |

<details>
  <summary>Build Contents</summary>

  - **macOS**
    - *Toolchain (llvm, clang, lld, lldb, swift)*
      - x64
    - *xctoolchain*
      - x64

  - **VS2017**
    - *Toolchain (llvm, clang, lld, lldb, swift)*
      - x64
  
  - **VS2019**
    - *Toolchain (llvm, clang, lld, lldb, swift)*
      - ARM64
      - x86
    - *Swift SDK for Android (swift, libdispatch, foundation, xctest)*
      - ARM
      - ARM64
      - x64
      - x86
    - *Swift SDK for Windows (swift, libdispatch, foundation, xctest)*
      - ARM
      - ARM64
      - x64
      - x86
    - *Swift Developer Tools (llbuild)*
      - ARM64
      - x64
    - *MSI*
      - Toolchain
        - x64

  - **VS2017 (Facebook)**
    - *Toolchain (llvm, clang, lld, lldb, swift)*
      - X64
    - *Swift SDK for Windows (swift, libdispatch, foundation, xctest)*
      - ARM
      - ARM64
      - x64
      - x86

  - **VS2019 (Facebook)**
    - *Toolchain (llvm, clang, lld, lldb, swift)*
      - x64
    - *Swift SDK for Windows (libdispatch, foundation, xctest)*
      - ARM
      - ARM64
      - x64
      - x86

  - **Ubuntu 18.04 (flowkey)**
    - *Toolchain (llvm, clang, lld, lldb, swift)*
      - x64
    - *Swift SDK for Linux (swift, libdispatch, foundation, xctest)*
      - x64
    - *Swift Developer Tools (llbuild, swift-package-manager)*
      - x64
    - *debian packages*
      - toolchain
        - x64
      - ICU
        - x64
      - Developer Tools
        - x64
      - SDK
        - Linux
</details>

## Getting the latest build

### Stable builds
The latest stable build can be acuqired from the [releases](https://github.com/compnerd/swift-build/releases) page.

### Development builds
The `utilities/swift-build.py` script allows downloading of the latest build artifacts. The script requires the `azure-devops` and `tabulate` python packages. These can be installed with `pip`:
```
python3 -m pip install tabulate azure-devops
```

For example, to download the latest VS2019 build:
```
swift-build.py --download --build-id VS2019 --latest-artifacts --filter installer.exe
```
