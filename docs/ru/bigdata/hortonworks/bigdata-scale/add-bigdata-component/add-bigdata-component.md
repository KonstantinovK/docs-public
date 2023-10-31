Существующие кластеры Hadoop и Spark в VK Cloud могут быть расширены новыми компонентами. В данном разделе вы узнаете, как установить новые компоненты и сервисы экосистемы Hadoop в существующие кластеры.Рассмотрим пример с добавлением Spark2 в существующий кластер Hadoop.

- Зайдите в интерфейс [Ambari](https://ambari.apache.org/). На вкладке «Dashboard»в нижнем левом углу панели сервисов кликните «Action»→ «Add Service».

  ![](./assets/1533045021997-36a377367202f26ab2e0d0062fadb74b.png)

- Выберите сервисы, которые вы хотите установить. Например,Spark2иZeppelin Notebook. Кликните «Next»внизу страницы.

  ![](./assets/1533045042967-159256458a7b5e5743c1add9a90e25b1.png)

- В открывшемся окне выберите рабочие и головные узлы для установки основных компонентов сервисов и кликните «Next»внизу страницы.

  ![](./assets/1533045073064-b2841cc13e90d709c5de1afc4ab31aa5.png)

- ### Важно

  При установке некоторых сервисов может быть необходимо задать авторизационные данные.

- В открывшемся окне выберите рабочие и головные узлы для установки вспомогательных и клиентских компонентов сервисов.При необходимости измените рекомендуемые настройки в окне Customize Services и кликните «Next»внизу страницы.

  ![](./assets/1533045122736-42a537c04dd43b08e7bdb833db7a4df5.png)

- В окне «Dependent Configurations»просмотрите список зависимых изменений, которые рекомендуется внести в настройки сервисов во избежание возможных конфликтов. При необходимости снимите выделение с тех параметров, значение которых необходимо оставить неизменным. По умолчанию все выделенные параметры примут значения, указанные в столбце «Recommended Value».

  Установив требуемые значения, кликните «OK».

  ![](./assets/1533045137910-1c45aa460518a9fac233efcbe8b7f918.png)

- В появившемся окне «Configurations»кликните «Proceed Anyway».

  ![](./assets/1533045291593-4e912558be61534c3e8975a35628cf72.png)

- В окне «Review»внимательно изучите краткую сводку по выбранной конфигурации и кликните «Deploy»внизу страницы, чтобы начать установку указанных сервисов.

  ![](./assets/1533045312095-24129d9898b708360668a85625198b0a.png)

- Начнется установка новых компонентов. По завершении процесса кликните «Next».

  ![](./assets/1533045331250-6099349b2921ec48ab424b1fc5121a7c.png)

- В окне «Summary»появится краткое описание результатов установки. Кликните «Complete», чтобы завершить процесс.

  ![](./assets/1533045384632-81132abe60b3b99b7b7a2acdccbb9c79.png)

- Для применения изменений может потребоваться перезапуск существующих сервисов. В интерфейсе Ambari перейдите на вкладку «Services» и кликните «Restart» → «Restart All Affected», чтобы перезапустить все зависимые сервисы. После перезапуска новые сервисы начнут работать в штатном режиме и будут доступны в интерфейсе Ambari в меню слева.

  ![](./assets/1533045407373-f4a93b547e095704e5d8815d6d5839c7.png)