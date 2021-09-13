## Instructions

To build a new toolchain, clone [esp-open-sdk](https://github.com/pfalcon/esp-open-sdk)
Use a configuration from the `esp-open-sdk-overrides` folder and follow build instructions in the esp-open-sdk repository.

## Build errors

1. Installing pass-2 core C gcc compiler - syntax errors in /esp-open-sdk/crosstool-NG/.build/src/gcc-11.2.0/libgcc/libgcov.h

Add #include <stdint.h> to the file.

2. Installing final gcc compiler: can't find Guile executable.

Install Guile 2.0 (Arch Linux):

```bash
pacman -Syu guile2.0
alias guile2.0 guile
```
