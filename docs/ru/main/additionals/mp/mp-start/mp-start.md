## Установка

<warn>

Инструкция распространяется на приложения, не относящиеся к SaaS.

</warn>

1. Откройте [личный кабинет](https://mcs.mail.ru/app/) VK Cloud.
1. Перейдите в раздел **Магазин приложений**.
1. В блоке с целевым приложением нажмите кнопку **Установить**.
1. Задайте параметры разворачиваемой ВМ:

    - **Имя приложения**: используйте только латинские буквы, цифры или символы `-`, `_` и `.`.
    - **Сеть**: выберите существующую сеть или создайте новую. Если выбран пункт `Создать новую сеть`, задайте **Адрес подсети**. Подробнее в разделе [Управление сетями и подсетями](/ru/networks/vnet/operations/manage-net).
    - **Ключ для доступа по SSH**: выберите ключ для подключения по SSH или создайте новый.

        При выборе `Создать новый ключ` сохраните предложенный файл ключа `.pem` после завершения создания виртуальной машины.

    - **Тип виртуальной машины**: выберите предустановленную конфигурацию ВМ (CPU и RAM).
    - **Тип диска**: выберите одно из значений — HDD, SSD или High-IOPS SSD.
    - **Размер диска**: укажите нужный размер диска ВМ в гигабайтах.
    - **Зона доступности**: выберите дата-центр, где будет запущена ВМ.

1. Нажмите кнопку **Установить**.
1. Дождитесь создания ВМ. Этот процесс может занять некоторое время. Когда создание будет завершено, откроется страница с инструкцией по подключению к ВМ и началом работы с приложением.

Список доступных для установки приложений, а также их дальнейшая настройка описана в разделе [Приложения](../mp-apps/).

## Просмотр списка приложений

Список установленных приложений отображается в разделе **Магазин приложений** → **Мои приложения на ВМ**.

## Подключение к ВМ

Подключение к ВМ, на котором было развернуто приложение, выполняется [по аналогии](/ru/base/iaas/vm-start/vm-connect) с вычислительными машинами, созданными в разделе **Облачные вычисления**.