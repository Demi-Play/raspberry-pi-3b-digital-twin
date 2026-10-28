# Sources / Перечень использованных источников

Дата обращения ко всем источникам: **28.10.2026**.
Сформировано ИСИТ (команда № 4, ИСТ-231) для раздела 1.3 «Анализ электронной компонентной базы».

## 1. Официальная документация Raspberry Pi Foundation (pip.raspberrypi.com)

| # | Документ | URL | Доступ | Статус |
|---|---|---|---|---|
| 1 | Электрическая схема Raspberry Pi 3 Model B (RP-008340-DS, reduced schematics, RPI-3B v1.2) | https://pip.raspberrypi.com/documents/RP-008340-DS | PDF открыт | Использован как первичный источник маркировок; скачан в `datasheets/power_management/` |
| 2 | Механический чертёж Raspberry Pi 3B, PDF (RP-008335-DS) | https://pip.raspberrypi.com/documents/RP-008335-DS | PDF открыт | Использован для `measurements/dimensions.csv` |
| 3 | Механический чертёж Raspberry Pi 3B, DXF (RP-008334-DS) | https://pip.raspberrypi.com/documents/RP-008334-DS | Ссылка | Для CAD (`cad/pcb/`) |
| 4 | BCM2836 Arm-local peripherals (RP-008250-DS) — применяется к BCM2837 | https://pip.raspberrypi.com/documents/RP-008250-DS | PDF открыт | Скачан в `datasheets/BCM2837/` |
| 5 | Raspberry Pi 3 Model B Product Change Notification / EoL (RP-001029-PC) | https://pip.raspberrypi.com/documents/RP-001029-PC | Ссылка | SoC BCM2837 снят с производства |
| 6 | Схема Raspberry Pi 3B (datasheets.raspberrypi.com) | https://datasheets.raspberrypi.com/rpi3/raspberry-pi-3-b-reduced-schematics.pdf | PDF открыт | Зеркало документа № 1 |
| 7 | Механический чертёж 3B (datasheets.raspberrypi.com) | https://datasheets.raspberrypi.com/rpi3/raspberry-pi-3-b-mechanical-drawing.pdf | PDF открыт | Зеркало документа № 2 |

## 2. Официальная документация Raspberry Pi (docs.raspberrypi.com)

| # | Документ | URL | Доступ | Статус |
|---|---|---|---|---|
| 8 | Страница процессора BCM2837 (описание, частоты, статус EoL) | https://www.raspberrypi.com/documentation/computers/processors/bcm2837.adoc (raw GitHub) | Открыт | Частоты ядер/GPU, статус discontinued |
| 9 | BCM2835 peripherals reference (базовая периферия BCM283x) | https://datasheets.raspberrypi.com/bcm2835/bcm2835-peripherals.pdf | PDF открыт | Скачан в `datasheets/BCM2837/` |
| 10 | Продуктовая страница Raspberry Pi 3 Model B | https://www.raspberrypi.com/products/raspberry-pi-3-model-b/ | Сайт блокирует автоматический доступ (403) | Ссылка для ручной проверки характеристик |
| 11 | Cortex-A53 MPCore Technical Reference Manual | https://developer.arm.com/documentation/ddi0500/latest/ | Ссылка | Подтверждение ядра Cortex-A53 |

## 3. Datasheets производителей

| # | Компонент | Производитель | URL | Доступ | Статус |
|---|---|---|---|---|---|
| 12 | LAN9514 (DS00001691B) | Microchip (ex-SMSC) | https://ww1.microchip.com/downloads/en/DeviceDoc/00001691B.pdf | PDF открыт | Скачан в `datasheets/LAN9514/` |
| 13 | DMG1012T (DS31783 Rev. 8) | Diodes Incorporated | https://www.diodes.com/assets/Datasheets/DMG1012T.pdf | PDF открыт | Скачан в `cad/components/` |
| 14 | DMG2305UX | Diodes Incorporated | https://www.diodes.com/assets/Datasheets/DMG2305UX.pdf | PDF открыт | Скачан в `cad/components/` |
| 15 | RT8088A (DS8088A-01) | Richtek | https://www.richtek.com/assets/product_file/RT8088A/DS8088A-01.pdf | PDF открыт | Скачан в `datasheets/power_management/` |
| 16 | RT9741 (DS9741-00) | Richtek | https://www.richtek.com/assets/product_file/RT9741/DS9741-00.pdf | PDF открыт | Скачан в `datasheets/power_management/` |
| 17 | NC7WZ16 (NC7WZ16-D.PDF) | onsemi (Fairchild) | https://www.onsemi.com/pub/Collateral/NC7WZ16-D.PDF | 403 (bot-защита) | **Требует проверки** — ручная загрузка datasheet |
| 18 | MMBT3904 | onsemi | https://www.onsemi.com (страница MMBT3904) | 403 (bot-защита) | **Требует проверки** |
| 19 | BCM857BS | Infineon | https://www.infineon.com (страница BCM857BS) | Прямая ссылка не найдена | **Требует проверки** |
| 20 | APX803-46SAG | Anpec | https://www.anpec.com.tw | 403 (bot-защита) | **Требует проверки** |
| 21 | PAM2306 | Anpec | https://www.anpec.com.tw (страница PAM2306) | 403 (bot-защита) | **Требует проверки** — datasheet не получен автоматически |
| 22 | MxL7704 (только Pi 3B+ / Pi 4, в BOM 3B не включается) | MaxLinear | https://www.maxlinear.com (страница MXL7704) | 403 (bot-защита) | **Требует проверки**; зафиксировано ограничение доступа |
| 23 | SRN4018 (дроссель 4,7 мкГн) | Bourns | https://www.bourns.com (страница SRN4018) | Не проверено автоматически | **Требует проверки** |
| 24 | MF-MSMF (полифьюзы) | Bourns | https://www.bourns.com (страница MF-MSMF) | Не проверено автоматически | **Требует проверки** |

## 4. Замечания

1. Полные datasheets **BCM2837** и **BCM43438** не опубликованы в открытом доступе; вместо них использованы официальные документы Raspberry Pi Foundation (№ 1, 4, 8, 9) и схема платы (№ 1).
2. Ссылки на документацию LAN9514 (Microchip) и NC7WZ16 (onsemi) ведут непосредственно к техническим описаниям производителей.
3. Все позиции BOM со статусом «Требует проверки» подлежат уточнению по фотографиям исследуемой платы и ручной загрузке datasheets.
