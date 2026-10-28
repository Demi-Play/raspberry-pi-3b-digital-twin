# datasheets/BCM43438/

**Компонент:** Broadcom BCM43438 — комбинированный модуль Wi-Fi / Bluetooth Raspberry Pi 3 Model B
**Позиция на схеме:** отдельный чип у антенны (тактирование от кварца X1 19,2 МГц)

## Статус datasheet

Полный datasheet Broadcom BCM43438 **не опубликован** в открытом доступе —
зафиксировано ограничение доступа. Статус позиции в BOM: **Требует проверки**
(подтверждение по фотографиям исследуемой платы и официальным материалам Raspberry Pi).

## Официально подтверждённые характеристики (Raspberry Pi 3 Model B)

- Wi-Fi **802.11n**, диапазон **2,4 ГГц** (single-band).
- Bluetooth **4.1 Classic + Bluetooth Low Energy (BLE)**.
- Интерфейс Wi-Fi: **SDIO**; интерфейс Bluetooth: **UART/HCI** (в схеме RPI-3B v1.2 — связь с SoC).
- Тактирование: кварцевый резонатор **19,2 МГц** (X1) через ключевые цепи на MOSFET (Q3/Q7 DMG2305UX).
- Антенна: печатная (chip antenna) на верхней стороне платы.

## Источники

- Официальная страница Raspberry Pi 3 Model B: https://www.raspberrypi.com/products/raspberry-pi-3-model-b/
- Электрическая схема: https://pip.raspberrypi.com/documents/RP-008340-DS
- Замечание: на Raspberry Pi 3 Model **B+** используется другой модуль (CYW43430 / Murata) — не путать с 3B.
