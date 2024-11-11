<warn>

Функциональность доступна только для СУБД PostgreSQL.

</warn>

## Создание расписания

При создании расписания PITR будут скопированы журналы СУБД.

<tabs>
<tablist>
<tab>Личный кабинет</tab>
</tablist>
<tabpanel>

1. [Перейдите](https://msk.cloud.vk.com/app/) в личный кабинет VK Cloud.
1. Перейдите в раздел **Cloud Backup → Резервное копирование**.
1. Перейдите на вкладку **Point-in-time recovery**.
1. Нажмите кнопку **Добавить**.
1. В открывшемся окне укажите:

   - **Название расписания**: введите название для создаваемого расписания.
   - **Время начала**: укажите время начала резервного копирования в часовом поясе, указанном ниже в окне.
   - **Хранить, кол-во копий**: укажите количество хранимых резервных копий.
   - **Интервал резервного копирования**: выберите подходящий интервал между запусками резервного копирования.
   - **База данных**: выберите развернутый инстанс с СУБД PostgreSQL.

1. Нажмите кнопку **Сохранить расписание**.

</tabpanel>
</tabs>

## Редактирование существующего расписания

<tabs>
<tablist>
<tab>Личный кабинет</tab>
</tablist>
<tabpanel>

1. [Перейдите](https://msk.cloud.vk.com/app/) в личный кабинет VK Cloud.
1. Перейдите в раздел **Cloud Backup → Резервное копирование**.
1. Перейдите на вкладку **Point-in-time recovery**.
1. Нажмите ![ ](/ru/assets/more-icon.svg "inline") для нужного расписания и выберите пункт **Редактировать расписание**.
1. Внесите нужные изменения и нажмите кнопку **Сохранить расписание**.

</tabpanel>
</tabs>

## Просмотр резервных копий расписания

<tabs>
<tablist>
<tab>Личный кабинет</tab>
</tablist>
<tabpanel>

1. [Перейдите](https://msk.cloud.vk.com/app/) в личный кабинет VK Cloud.
1. Перейдите в раздел **Cloud Backup → Резервное копирование**.
1. Перейдите на вкладку **Point-in-time recovery**.
1. Нажмите на название нужного расписания.

Будет отображен список резервных копий для выбранного расписания.

</tabpanel>
</tabs>

## Создание инстанса базы данных из резервной копии

<tabs>
<tablist>
<tab>Личный кабинет</tab>
</tablist>
<tabpanel>

1. [Перейдите](https://msk.cloud.vk.com/app/) в личный кабинет VK Cloud.
1. Перейдите в раздел **Cloud Backup → Резервное копирование**.
1. Перейдите на вкладку **Point-in-time recovery**.
1. Нажмите на название нужного расписания.
1. Нажмите ![ ](/ru/assets/more-icon.svg "inline") для нужной резервной копии и выберите пункт **Восстановить из бэкапа**.
1. На шаге «Создание инстанса» укажите нужные параметры и нажмите кнопку **Следующий шаг**.
1. (Опционально) Укажите дату и время нужной резервной копии в одноименном поле. Если оставить поле пустым, автоматически будет выбрана последняя созданная резервная копия.
1. Нажмите кнопку **Создать базу данных**.

</tabpanel>
</tabs>