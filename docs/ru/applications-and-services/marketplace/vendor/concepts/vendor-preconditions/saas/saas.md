# {heading(Требования к API SaaS-приложений)[id=saas]}

Чтобы SaaS-приложение можно было добавить в {var(sys1)}, API SaaS-приложения должен позволять выполнять следующие действия:

* Управлять жизненным циклом инстанса сервиса:

   * Создать. {var(sys1)} должен иметь возможность получить все тарифные планы и опции SaaS-приложения.
   * Обновить (поменять тарифный план или опции).
   * Получить информацию (текущий тарифный план и опции).
   * Удалить.

* Если для работы с сервисом используются сервисные привязки — управлять их жизненным циклом:

   * Создать.
   * Получить информацию.
   * Удалить.

* Если операции с инстансом сервиса выполняются асинхронно — получать статус следующих операций:

   * С инстансом сервиса:

      * Создания.
      * Обновления.
      * Удаления.

   * С сервисной привязкой (если для работы сервиса используются сервисные привязки):

      * Создания.
      * Удаления.

* Если для SaaS-приложения используется предоплатный тип тарификации и нет бесплатного тарифного плана — выполнять следующие операции:

   * Приостановить инстанс сервиса. Это позволит избежать удаления данных в случае деактивации инстанса сервиса.
   * Возобновить работу инстанса сервиса.

* Если для SaaS-приложения используется постоплатный тип тарификации — выполнять следующие операции:

   * Передавать информацию о потреблении сервиса по его инстансам за отчетный период (например, за месяц).
   * Приостановить инстанс сервиса. Это позволит избежать удаления данных в случае деактивации инстанса сервиса.
   * Возобновить работу инстанса сервиса.

<warn>

Взаимодействие между {var(sys5)} и SaaS-приложением должно быть автоматизировано. Ручные операции не допускаются.

</warn>