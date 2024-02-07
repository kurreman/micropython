This directory contains C drivers for specific hardware.  The drivers are
intended to work across multiple ports.


## Adding a new driver
Example: 

[processor] = stm32

[board] = OPENMV4P (H7 Plus)

[driver] = can

## Files to alter
- src/micropython/ports/[processor]/Makefile
- src/micropython/ports/[processor]/README.md
- src/micropython/ports/[processor]/boards/[board]/mpconfigboard.h
- src/micropython/ports/[processor]/machine_[driver].c
- src/micropython/ports/[processor]/main.c
- src/micropython/ports/[processor]/modmachine.c
- src/micropython/ports/[processor]/modmachine.h
- src/micropython/ports/[processor]/mpconfigport.h

- src/omv/ports/[processor]/main.c
- src/omv/ports/[processor]/omv_portconfig.mk