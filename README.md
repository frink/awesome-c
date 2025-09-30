# awesome-c-ecosystem
A survey of the smaller known C compilers and libc implementations

## Compilers

### Small/Educational Compilers
- **[xcc](https://github.com/tyfkda/xcc)** (MIT) - Full toolchain compiler/assembler/linker/libc for x86-64/aarch64/riscv64/wasm
- **[tcc](https://github.com/TinyCC/tinycc)** (LGPL v2.1+) - Tiny C Compiler, ~100KB executable, very fast compilation, supports x86/x64/ARM/RISC-V  
- **[chibicc](https://github.com/rui314/chibicc)** (MIT) - Small C11 compiler by Rui Ueyama, can compile Git/SQLite/libpng, educational focus
- **[lacc](https://github.com/larmel/lacc)** (MIT) - Simple self-hosting C compiler with rich IR and basic optimization
- **[9cc](https://github.com/rui314/9cc)** (MIT) - Rui Ueyama's earlier educational C compiler, predecessor to chibicc
- **[lcc](https://github.com/drh/lcc)** (Custom non-commercial) - Fraser & Hanson's retargetable ANSI C compiler, well-documented academic compiler
- **[kefir](https://kefir.protopopov.lv)** (GPL v3 + BSD-3 runtime) - Independent C17/C23 compiler with extensive validation, SSA optimization

### Industrial Heavyweights
- **gcc** (GPL v3) - GNU Compiler Collection, the standard Linux C compiler
- **clang** (Apache 2.0) - LLVM-based compiler, Apple's choice, excellent diagnostics  
- **msvc** (Proprietary) - Microsoft Visual C++, Windows development standard
- **icc** (Proprietary) - Intel C Compiler, optimized for Intel processors

## libc Implementations

### Full-Featured
- **[glibc](https://www.gnu.org/software/libc/)** (LGPL v2.1+) - GNU C Library, standard on most Linux distributions
- **[musl](https://musl.libc.org/)** (MIT) - Lightweight, fast, simple C library, Alpine Linux default

### Minimal/Embedded  
- **[dietlibc](http://www.fefe.de/dietlibc/)** (GPL v2) - Size-optimized libc for creating small static binaries
- **[uClibc-ng](https://uclibc-ng.org/)** (LGPL v2.1) - Small C library for embedded Linux systems, fork of original uClibc
- **[xcc libc](https://github.com/tyfkda/xcc)** (MIT) - Minimal libc implementation included with xcc toolchain
- **[newlib](https://sourceware.org/newlib/)** (Multiple BSD-style) - Standard C library for embedded systems, widely used in vendor toolchains
- **[picolibc](https://keithp.com/picolibc/)** (Multiple BSD-style) - Smaller embedded libc based on newlib, removes bloat, uses TLS
- **[AVR-libc](https://www.nongnu.org/avr-libc/)** (Modified BSD) - Optimized C library for Atmel AVR 8-bit microcontrollers
- **[Embedded Artistry libc](https://github.com/embeddedartistry/libc)** (MIT) - Stripped-down C library for microcontrollers with unit tests
- **[Zephyr minimal libc](https://docs.zephyrproject.org/latest/develop/languages/c/minimal_libc.html)** (Apache 2.0) - Ultra-minimal subset for the Zephyr RTOS kernel

### Mobile/Platform-Specific
- **[Bionic](https://android.googlesource.com/platform/bionic/)** (BSD + Apache 2.0) - Google's Android C library, BSD-licensed, smaller than glibc
- **[BSD libc](https://github.com/freebsd/freebsd-src/tree/main/lib/libc)** (BSD) - Various BSD system implementations (FreeBSD, OpenBSD, NetBSD)
- **[Microsoft UCRT](https://docs.microsoft.com/en-us/cpp/c-runtime-library/)** (Proprietary) - Universal C Runtime for Windows, C99-compliant

### Specialized
- **[cosmopolitan](https://github.com/jart/cosmopolitan)** (ISC) - Build-once run-anywhere libc, creates polyglot executables for multiple platforms
- **[klibc](https://git.kernel.org/pub/scm/libs/klibc/klibc.git/)** (GPL v2) - Minimal libc primarily for Linux early boot and initramfs
- **[LLVM libc](https://libc.llvm.org/)** (Apache 2.0) - LLVM project's new C library implementation, header-only modular design
