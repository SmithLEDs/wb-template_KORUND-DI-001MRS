# Шаблон для датчика избыточного давления с выходом RS-485 КОРУНД-ДИ-001MRS
Данный шаблон написан для контроллера Wiren Board. Инструкция по установке шаблона смотри на [главной странице](https://github.com/SmithLEDs/wirenboard#установка-шаблонов-в-контроллер).
* [Официальный сайт производителя](https://stenli.ru/korund-di-001mrs?ysclid=mgf6fkn7bn85177845#shop2-tabs-2)
* [modbus_config_setup.zip](https://stenli.ru/f/modbus_config_setup.zip) - официальный сайт
* [modbus_config_setup.zip](https://github.com/SmithLEDs/wb-template_KORUND-DI-001MRS/blob/main/modbus_config_setup.zip) - сохраненная версия на GitHub
* [Руководство по эксплуатации](https://github.com/SmithLEDs/wb-template_KORUND-DI-001MRS/blob/main/0rukovodstvo_po_ekspluatatsii_korund_dkh_mrs.pdf)

## Настройки подключения RS-485 по умолчанию
| Параметр      | Значение по умолчанию |
| ------------- | --------------------- |
| Адрес         | `1`                   |
| Подключение   | `9600 8E1`            |

## Изменить настройки подключения на `115200 8N1`
Функция 06. Регистр `0x0A (10)` записать `0x0107 (263)`
> [!NOTE]
> После изменения отключить и включить питание датчика!!!

## Изменить адрес датчика на `2`
Функция 06. Регистр `0x0C (12)` записать `0x0002 (2)`

## Измеренное значение
Функция 03. Регистр `0x08 (8)` float 32
