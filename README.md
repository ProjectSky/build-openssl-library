# build-openssl-library

Building Windows & Linux Static Libraries for OpenSSL

## Overview

This project automates the process of building OpenSSL static libraries for both Windows and Linux platforms, supporting both 32-bit and 64-bit architectures.

## Features

- Builds OpenSSL static libraries for:
  - Windows (x86, x86_64)
  - Linux (x86, x86_64)
- Automated builds via GitHub Actions
- Customizable library names
- Release packaging with documentation

### Build Options
- Disabled features: shared libs, apps, docs, tests, TLS 1.0, TLS 1.1
- Build flags: `no-shared no-apps no-docs no-tests no-tls1 no-tls1_1`

## Output Files

### Windows
```
lib/
├── libcrypto_static_x86.lib
├── libcrypto_static_x86_64.lib
├── libssl_static_x86.lib
└── libssl_static_x86_64.lib
include/
└── openssl/
```

### Linux
```
lib/
├── libcrypto_static_x86.a
├── libcrypto_static_x86_64.a
├── libssl_static_x86.a
└── libssl_static_x86_64.a
include/
└── openssl/
```