В статье описано, как создать инстанс JupyterHub через личный кабинет VK Cloud.

Создать инстанс можно также с помощью следующих инструментов:

- [Terraform](/ru/tools-for-using-services/terraform/how-to-guides/mlplatform/jupyterhub);
- библиотека Cloud ML Platform, метод [create_jupyter_hub](../../../mlplatform-lib/lib-reference#create_jupyter_hub).

Чтобы создать инстанс JupyterHub:

1. [Перейдите](https://msk.cloud.vk.com/app/) в личный кабинет VK Cloud.
1. Перейдите в раздел **ML Platform**.
1. Выберите тип создаваемого инстанса одним из способов:

    - Нажмите кнопку **Создать инстанс** в карточке **JupyterHub**.
    - Перейдите в раздел **Инстансы** и выполните действия:

        1. Нажмите кнопку **Добавить** над списком инстансов.
        1. Выберите карточку **Инстанс JupyterHub**.
        1. Нажмите кнопку **Следующий шаг**.
1. На шаге «Конфигурация» укажите параметры инстанса:

    - **Имя инстанса**: отображаемое имя инстанса, также задает hostname в ОС. Имя может содержать только латинские буквы, цифры и спецсимволы `-`, `_` и `.`.
    - **Категория виртуальной машины**: определяет список предустановленных конфигураций ВМ в поле **Тип виртуальной машины**. Подробнее в [обзоре сервиса Cloud Servers](/ru/computing/iaas/concepts/about#shablony_konfiguraciy).
    - **Тип виртуальной машины**: предустановленная конфигурация ВМ (CPU и RAM).
    - **Зона доступности**: выбор [дата-центра](/ru/intro/start/concepts/architecture#az), где будет запущен инстанс.
    - **Размер диска**: задает размер диска данных ВМ в ГБ. Минимальное значение — 50 ГБ. При создании инстанса ему подключается основной (root disk) и дополнительный диск данных (data disk). Размер основного диска фиксированный — 50 ГБ. Вы можете изменить только размер диска данных.
    - **Тип диска**: [тип](/computing/iaas/concepts/volume-sla/) создаваемого диска.
    - **Выбор доменного имени**: задает DNS-имя инстанса.
    - **Подключить S3 бакет как диск**: включите опцию, чтобы добавить к инстансу бакет S3 для хранения в нем данных. Бакет будет доступен внутри инстанса как директория, а хранимые в нем данные будут доступны в [Cloud Storage](/ru/storage/s3) даже после удаления инстанса.
    - **Бакет**: если включена опция **Подключить S3 бакет как диск**, в списке выберите бакет, который нужно подключить к инстансу. Если подходящих бакетов нет, выберите **Создать новый бакет** — при создании инстанса будет создан новый бакет Cloud Storage.  
    - **Имя пользователя**: имя администратора для авторизации в ОС инстанса. Только администратор сможет [создавать другие учетные записи](../manage#create-users) для работы на инстансе.

        <err>
        Не работайте на инстансе под учетной записью администратора. Если администратор приведет инстанс в нерабочее состояние, восстановить инстанс будет невозможно.
        </err>

    - **Пароль пользователя**: пароль администратора для авторизации в ОС инстанса. Пароль должен содержать:

        - 8 символов и более;
        - одну или более заглавную букву латинского алфавита;
        - одну или более строчную букву латинского алфавита;
        - одну или более цифру;
        - один или более спецсимвол из диапазона: `!`, `#`, `$`, `%`, `&`, `(`, `)`, `*`, `+`, `,`, `.`, `:`, `;`, `<`, `=`, `>`, `?`, `@`, `[`, `]`, `^`,`_`, `{`,`|`, `}`,`~`,`-`.

        <err>

        Сохраните пароль. Восстановить пароль невозможно.

        </err>

1. Нажмите кнопку **Следующий шаг**.

1. На шаге «Выбор сети» укажите параметры сети, в которой будет размещен инстанс:

    - **Сеть**: выберите сеть или создайте новую.
    - **Адрес подсети**: укажите CIDR подсети, если выбрано создание новой сети.

1. Нажмите кнопку **Создать инстанс**.

Создание инстанса обычно занимает 10–15 минут. За это время на диске инстанса будет развернута операционная система и ВМ инстанса будет настроена в соответствии с выбранными параметрами.

Когда инстанс будет создан, откроется страница с его характеристиками.