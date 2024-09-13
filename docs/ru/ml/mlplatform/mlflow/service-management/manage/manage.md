Управление инстансом MLflow доступно через личный кабинет VK Cloud. Удалить инстанс можно также с помощью [библиотеки Cloud ML Platform](../../../mlplatform-lib/lib-reference).

## {heading(Изменение типа виртуальной машины)[id=change-vm-type]}

1. [Перейдите](https://msk.cloud.vk.com/app/) в личный кабинет VK Cloud.
1. Перейдите в раздел **ML Platform** → **Инстансы**.
1. Нажмите ![ ](/ru/assets/more-icon.svg "inline") для нужного инстанса и выберите пункт **Изменить тип виртуальной машины**.
1. В открывшемся окне выберите категорию виртуальных машин, чтобы отфильтровать список конфигураций ВМ. Подробнее в [обзоре сервиса Cloud Servers](/ru/computing/iaas/concepts/about#shablony_konfiguraciy).
1. В поле **Тип виртуальной машины** выберите предустановленную конфигурацию ВМ (CPU и RAM).
1. Нажмите кнопку **Сохранить**.

## {heading(Изменение размера диска)[id=change-disk-size]}

1. [Перейдите](https://msk.cloud.vk.com/app/) в личный кабинет VK Cloud.
1. Перейдите в раздел **ML Platform** → **Инстансы**.
1. Нажмите ![ ](/ru/assets/more-icon.svg "inline") для нужного инстанса и выберите пункт **Изменить размер диска**.
1. В открывшемся окне измените размер диска. Минимальное значение — 30 ГБ.
1. Нажмите кнопку **Сохранить**.

## {heading(Остановка и запуск инстанса)[id=pause]}

Это групповая операция: при необходимости можно остановить или запустить сразу несколько инстансов, выбрав их с помощью флажков.

Чтобы остановить инстанс:

1. [Перейдите](https://msk.cloud.vk.com/app/) в личный кабинет VK Cloud.
1. Перейдите в раздел **ML Platform** → **Инстансы**.
1. Остановите инстанс одним из способов:

    - Нажмите ![ ](/ru/assets/more-icon.svg "inline") для нужного инстанса и выберите пункт **Остановить**.
    - Выберите инстанс с помощью флажка, затем нажмите кнопку **Остановить**.
1. Подтвердите действие.

Чтобы запустить инстанс:

1. [Перейдите](https://msk.cloud.vk.com/app/) в личный кабинет VK Cloud.
1. Перейдите в раздел **ML Platform** → **Инстансы**.
1. Запустите инстанс одним из способов:

    - Нажмите ![ ](/ru/assets/more-icon.svg "inline") для нужного инстанса и выберите пункт **Запустить**.
    - Выберите инстанс с помощью флажка, затем нажмите кнопку **Запустить**.
1. Подтвердите действие.

## {heading(Перезагрузка инстанса)[id=reload]}

<info>
Перезагрузка предполагает корректное завершение работы операционной системы ВМ инстанса (graceful shutdown).
</info>

Это групповая операция: при необходимости можно перезагрузить сразу несколько инстансов, выбрав их с помощью флажков.

Чтобы перезагрузить инстанс:

1. [Перейдите](https://msk.cloud.vk.com/app/) в личный кабинет VK Cloud.
1. Перейдите в раздел **ML Platform** → **Инстансы**.
1. Перезагрузите инстанс одним из способов:

    - Нажмите ![ ](/ru/assets/more-icon.svg "inline") для нужного инстанса и выберите пункт **Перезагрузить**.
    - Выберите инстанс с помощью флажка, затем нажмите кнопку **Перезагрузить**.
1. Подтвердите действие.

## {heading(Принудительный перезапуск инстанса)[id=force-reload]}

Если инстанс не отвечает, используйте принудительный перезапуск.

<warn>

Принудительный перезапуск инстанса соответствует выключению и включению питания (power cycling). Несохраненные данные могут быть потеряны.

</warn>

Чтобы принудительно перезапустить инстанс:

1. [Перейдите](https://msk.cloud.vk.com/app/) в личный кабинет VK Cloud.
1. Перейдите в раздел **ML Platform** → **Инстансы**.
1. Нажмите ![ ](/ru/assets/more-icon.svg "inline") для нужного инстанса и выберите пункт **Перезапустить принудительно**.
1. Подтвердите действие.

## {heading(Копирование ссылки на инстанс)[id=copy-link]}

Вы можете поделиться ссылкой на инстанс с другими пользователями. По этой ссылке пользователи смогут открыть консоль инстанса и работать с ним.

Чтобы поделиться ссылкой на инстанс:

1. [Перейдите](https://msk.cloud.vk.com/app/) в личный кабинет VK Cloud.
1. Перейдите в раздел **ML Platform** → **Инстансы**.
1. Нажмите ![ ](/ru/assets/more-icon.svg "inline") для нужного инстанса и выберите пункт **Копировать ссылку на MLflow**.

Ссылка будет скопирована в буфер обмена, она соответствует DNS-имени инстанса.

## {heading(Удаление инстанса)[id=delete]}

<info>

Если инстанс MLflow связан с MLflow Deploy, сначала [удалите инстанс MLflow Deploy](../../../deploymlflow/service-management/delete).

</info>

<tabs>
<tablist>
<tab>Личный кабинет</tab>
<tab>Библиотека Cloud ML Platform</tab>
</tablist>
<tabpanel>

Это групповая операция: при необходимости можно удалить сразу несколько инстансов, выбрав их с помощью флажков.

1. [Перейдите](https://msk.cloud.vk.com/app/) в личный кабинет VK Cloud.
1. Перейдите в раздел **ML Platform** → **Инстансы**.
1. Удалите инстанс одним из способов:

    - Нажмите ![ ](/ru/assets/more-icon.svg "inline") для нужного инстанса и выберите пункт **Удалить**.
    - Выберите инстанс с помощью флажка, затем нажмите кнопку **Удалить**.
1. Подтвердите действие.

</tabpanel>
<tabpanel>

Используйте метод [delete_instance](../../../mlplatform-lib/lib-reference#delete_instance).

</tabpanel>
</tabs>