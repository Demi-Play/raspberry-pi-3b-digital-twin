# datasheets/BCM2837/

**Компонент:** Broadcom BCM2837 — SoC Raspberry Pi 3 Model B
**Статус полного datasheet:** Broadcom BCM2837 **не опубликован** в открытом доступе (требует проверки / зафиксировано ограничение доступа).

## Файлы

| Файл | Описание | Источник |
|---|---|---|
| `RP-008250-DS_BCM2836-ARM-local-peripherals.pdf` | Официальный документ Raspberry Pi Foundation «BCM2836 Arm-local peripherals» (Gert van Loo, Rev 3.4, 18.08.2014). Применяется и к BCM2837 (архитектура периферии идентична BCM2836, отличается только кластером ядер Arm). | https://pip.raspberrypi.com/documents/RP-008250-DS |
| `BCM2835-peripherals-reference.pdf` | Официальный справочник периферии BCM2835 (базовая документация по периферийным блокам GPIO/UART/I2C/SPI и т. д.). | https://datasheets.raspberrypi.com/bcm2835/bcm2835-peripherals.pdf |

## Официальные сведения о BCM2837 (docs.raspberrypi.com, processors/bcm2837)

- Используется в Raspberry Pi 3 Model B (ранние ревизии), части Pi 2 Model B и Compute Module 3.
- Архитектура идентична BCM2836; отличие — 4 ядра **ARM Cortex-A53** (Armv8) вместо Armv7, частота ядер **1,2 ГГц**.
- GPU **VideoCore IV** — 400 МГц.
- SoC снят с производства: PCN `RP-001029-PC` (Raspberry Pi 3 Model B Product Change Notification), EoL.

## Дополнительные источники

- ARM Cortex-A53 MPCore TRM: https://developer.arm.com/documentation/ddi0500/latest/
- Схема платы: https://pip.raspberrypi.com/documents/RP-008340-DS
