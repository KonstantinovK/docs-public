# FAQ - Часто Задаваемые Вопросы
##  Общие вопросы

### Мне пришло письмо от VK Cloud про миграцию на новый SDN. Что это значит?
В феврале 2024 года VK Cloud выпустила SDN собственной разработки. В августе 2024 это решение стало доступно по-умолчанию для всех клиентов. 
По нашим планам, SDN Neutron будет отключен и выведен из продуктивного контура VK Cloud в 2025 году. Сейчас мы запустили процедуру миграции клиентов, что бы этот процесс был максимально безопасным.

### Я исполнитель, что мне сказать руководству по поводу этой вашей миграции?
Мы подготовили две презентации https://github.com/vk-cs/neutron-2-sprut/tree/main/presentations
- **Миграция на SDN Sprut. Short** — короткая версия презентации. Содержит в себе основные слайды о SDN, преимуществах Sprut, планы развития. Хорошо подходит для людей из бизнеса, которые не готовы погружаться в технику, но необходимо понять основную суть и необходимость в миграции;
- **Миграция на SDN Sprut. Full** — полная версия презентации. Содержит в себе технические подробности реализации, особенности архитектуры и тд. Создана для инженеров и руководителей команд, которым надо не только понимать, что такое SDN Sprut, но и глубокие технические детали реализации, сравнения, функциональные преимущества.

Также, доступно [Полное руководство по миграции на Sprut](/docs/Complete_migration_guide_to_Sprut.md), которое содержит в себе ответы на многие вопросы и является текстовым описанием презентаций.

### Что такое SDN?
Software Defined Network - Основа облачной инфраструктуры, которая обеспечивает сетевую связаность облачных сервисов
Болле подробно мы описали в [Полном руководстве по миграции](/docs/Complete_migration_guide_to_Sprut.md#что-такое-sdn)

### В чем разница между Sprut и Neutron?
SDN Sprut имеет существенные архитектурные отличия, что дает ряд функциональных и нефункционльных преимуществ.
Мы подробно описали все различия и преимущества SDN Sprut в [Полном руководстве по миграции](/docs/Complete_migration_guide_to_Sprut.md#сравнение-sdn-neutron-и-sdn-sprut)

### Зачем мне нужно мигрировать?
В начале 2024 года была выпущена стабильная версия SDN Sprut. Начиная с этого момента, разработка новых функицональных возможностей SDN Neutron была приостановлена. В первом полугудии 2025 года VK Cloud прекращает поддержку SDN Neutron. Это означает, что команды разработки и саппорта прекращают осуществлять работу с проблемами, связанные с сетевой ифнаструкторой на SDN Neutron.

### Что будет, если я не захочу мигрировать?
В H1 2025 VK Cloud прекращает поддержку SDN Neutron. Это означает, что команды разработки и саппорта прекращают осуществлять работу с проблемами, связанные с сетевой ифнаструкторой на SDN Neutron. 
Начиная с 2025 года
В 2025 году SDN Neutron будет полностью отключен.

### Что потребуется с моей стороны для проведения миграции? 

### Как выглядит трек миграции? 
Сформирована общая схема последовательности действий при миграции IaaS и описана в [алгоритма](/docs/images/(IaaS)_алгоритм_миграции_нейтрон_спрут.png)

### Какая поддержка у меня будет по ходу миграции?
Мы описали
Также, вы можете обратиться в техническую поддержку VK Cloud

### С чего начать? 
Существует предварительный [чеклист](/docs/questions_before_migration.md), с которым необходимо ознакомится перед началом миграции и сформировать план по переключению.

### На какое время моя инфраструктура будет недоступна при миграции? 

### Какие риски у меня есть при миграции, что может пойти не так и что могу потерять? 

### Есть ли какое то обучение/курсы/ответы на вопросы по миграции?
Всю информацию о SDN Sprut и процессе миграции мы описали в [Полном руководстве по миграции](/docs/Complete_migration_guide_to_Sprut.md)

Если у вас есть дополнительные вопросы, то мы рекомендуем создать [Issue](https://github.com/vk-cs/neutron-2-sprut/issues) и описать ваш вопрос, проблему или запрос на функционал. Это стандартный механизм Github, который позволит нам не только ответить на вам, но и дополнить существующую документацию.

## Инфраструктура
### Что такое проект в VK Cloud Может ли быть сетевая связанность между двумя и более проектами? 

### Может ли быть связанность между проектами на разных SDN Можно ли мигрировать проект по частям? 

### Обратима ли миграция, если что-то пошло не так?

### Разница между Iaas и Paas инфраструктоурой в проекте 

### Я хочу сохранить свои белые IP при миграции, у меня это получится? 

### Что нужно сделать, что бы узнать архитектуру/топологию своего проекта/ проектов 

### Какие объекты могут быть в проекте

fip 

...

### У меня лютый кастом в проекте, что мне делать? 

## Подготовка к миграции
### Инструменты и подготовка системного окружения для миграции 

### Насколько безопасны ваши скрипты? 

### Как и в какой роли их нужно запускать? 

### Нужно одобрение СИБ на запуск этих скриптов? 

### Какой алгоритм работы скриптов, что он делает при запуске?
Каталог всех скриптов для миграции собрали в [Полном руководстве по миграции](/docs/Complete_migration_guide_to_Sprut.md#инструменты-миграции)

Каждый скрипт имеет подробную документацию, котороя содержит в себе
- Описание скрипта
- Алгоритм работы
- Схема данных
- Примеры запуска
- Миграция terraform-state

Если у вас есть дополнительные вопросы, то мы рекомендуем создать [Issue](https://github.com/vk-cs/neutron-2-sprut/issues) и описать ваш вопрос, проблему или запрос на функционал. Это стандартный механизм Github, который позволит нам не только ответить на вам, но и дополнить существующую документацию.

### Оптимальная стратегия миграции 
Мы описали [Базовый кейс миграции проекта на IaaS](/docs/Complete_migration_guide_to_Sprut.md#базовый-кейс-миграции-проекта-на-iaas), который иллюстрирует последовательность действий, а также примеры запуска скриптов и их параметров.

### Я хочу смигрировать несколько тестовых ВМ, так можно? 
да

### Какой размер даунтайма нужно закладывать? 

### Какие требования к квалификации (стеку навыков) моего персонала, который будет проводить миграцию? 

### Как запросить/получить поддержку команды VK Cloud во время миграции 

### Я хочу мигрировать проекты с PaaS, что мне для этого нужно сделать? 

### Что мне нужно сделать перед началом работ по миграции? 

## Психология миграции
### А у вас уже есть практика успешныых миграций?

### Насколько сложные проекты вы уже мигрировали?

### Сколько по времени заняла миграция?

### Какие факторы осложняли работы по миграции?

### Какие факторы позволили провести и удачно закончить миграцию?

### Были ли случаи неудачной миграции, когда ничего не удалось восстановить/ откатить?

### Дайте мне аргументы для моего начальника, который перестраховщик и не хочет ничего мигрировать

### До когда мне можно подумать насчет миграции, сейчас других дел полно

## Примеры юзеркейсов (хоть модельные, хоть реальные)

### У меня есть вот такие люъекты в проекте, в какой очередности и последовательности запускать скрипты, как использовать вывод, что отвечать на вопросы?

### Несколько примеров миграции