# DebugTool

Утилита DebugTool предназначена для чтения и записи регистров МК в проекте STM8S-VUSB-KEYBOARD.

Среда разработки и компилятор - Microsoft Visual Studio 2015 + Windows Driver Kit 10

Использование:

DebugTool.exe read/r/write/w width(8/16bit) register_addr register_data

Чтение регистра: DebugTool.exe read width register_addr

Пример:

=========================================

: DebugTool.exe read 8 0x5005

Device found: VID: 0x043B  PID: 0x0325  UsagePage: 0xFF00  Usage: 0x3

Reading register 0x5005 (8 bit)... OK!

Register addr: 0x5005

Width: 8 bit

Register data: 0x10

=========================================

Запись регистра: DebugTool.exe read width register_addr register_data

Пример:

=========================================

: DebugTool.exe write 8 0x5005 0

Device found: VID: 0x043B  PID: 0x0325  UsagePage: 0xFF00  Usage: 0x3

Register addr: 0x5005

Width: 8 bit

Register data: 0x0

Writing register... OK!

=========================================
