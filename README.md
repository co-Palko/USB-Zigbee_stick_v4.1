# USB-Zigbee_stick_v4.1
Zigbee ztick for z2m. CC2652P1 module from RFStar 

В связи с выходом на рынок предсобранных беспроводных модулей от Уважаемой компании RFStar (RF-BM-2652P1) https://szrfstar.com/product/252-cn.html появилась возможность упростить самостоятельную сборку устройства.
В итоге схема, как с прежде повторяет топологию плат семейства LAUNCHXL и документации от TI. Что позволяет использовать FW отлаженное на указанной devboard.

В остальном описание почти совпадает с описанием платы под чип CC1352P https://github.com/co-Palko/USB-Zigbee_stick_v4:

Оснащена по подобию отладочной платы кнопками BTN-1, BTN-2, Reset. Кроме того четырьмя LED индикаторами Power, активности UART, RedLED и GrnLED.

На плате присутствует радиоканал 2.4 GHz (+PA 2.4 Ghz). Производитель заявляет поддержку чипом Thread, Zigbee®, Bluetooth® 5.1 Low Energy, IEEE 802.15.4g, IPv6-enabled smart objects (6LoWPAN) proprietary systems, and Dynamic Multiprotocol Manager (DMM) driver. 
Отличие чипа СС2652 от СС1352 - в отсутствии передатчика субгигерцового диапазона то есть работа только в диапазоне 2,4 ГГц. 

Плата снабжена полноценным разъемом ARM Cortex debug 10pin для прошивки и отладки (при необходимости). Прошивка осуществляется посредством J-Link либо XDS110. Проверено с J-Link и пакетами Uniflash и J-Flash. Кроме того возможна прошивка через встроенный UART посредством Bootloader, в режим которого можно войти при запуске с помощью кнопки BTN-1.

Прошивка стандартная от уважемого @Koen Kanters (https://github.com/Koenkk) https://github.com/Koenkk/Z-Stack-firmware/tree/master/coordinator/Z-Stack_3.x.0 разработанная для платы LAUNCHXL. Она одинаковая как для СС1352Р, так и для СС2652Р.

Обсудить (на русском) можно здесь: https://t.me/zigbeer

In English
In connection with the entry to the market of pre-assembled wireless modules from the reputable company RFStar (RF-BM-2652P1) https://szrfstar.com/product/252-cn.html, it became possible to simplify the self-assembly of the device.
As a result, the circuit, as before, repeats the topology of boards of the LAUNCHXL family and documentation from TI. That allows you to use FW debugged on the specified devboard.

For the rest, the description almost coincides with the description of the board for the CC1352P chip https://github.com/co-Palko/USB-Zigbee_stick_v4:

Equipped with BTN-1, BTN-2, Reset buttons similar to a debug board. In addition, four LED indicators for Power, UART activity, RedLED and GrnLED.

The board has a 2.4 GHz radio channel (+ PA 2.4 Ghz). The manufacturer claims support for Thread, Zigbee®, Bluetooth® 5.1 Low Energy, IEEE 802.15.4g, IPv6-enabled smart objects (6LoWPAN) proprietary systems, and Dynamic Multiprotocol Manager (DMM) driver.
The difference between the CC2652 chip and the CC1352 is in the absence of a sub-GHz transmitter, that is, it works only in the 2.4 GHz range.

The board is equipped with a full ARM Cortex debug 10pin connector for firmware and debugging (if necessary). The firmware is carried out via J-Link or XDS110. Tested with J-Link and Uniflash and J-Flash packages. In addition, it is possible to flash through the built-in UART using the Bootloader, which can be entered at startup using the BTN-1 button.

Standard firmware from the respected @Koen Kanters (https://github.com/Koenkk) https://github.com/Koenkk/Z-Stack-firmware/tree/master/coordinator/Z-Stack_3.x.0 developed for the board LAUNCHXL. It is the same for both the CC1352R and the CC2652R.

You can discuss (in Russian) here: https://t.me/zigbeer
