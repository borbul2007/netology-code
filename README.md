Задача 2
Высоконагруженная база данных MySql, критичная к отказу
физические сервера
необходима высокая производительность

Различные web-приложения
паравиртуализация или виртуализация уровня ОС (если приложения под один тип ОС)
  
Windows-системы для использования бухгалтерским отделом
паравиртуализация 

Системы, выполняющие высокопроизводительные расчёты на GPU.
физические сервера
необходима высокая производительность

Задача 3
100 виртуальных машин на базе Linux и Windows, общие задачи, нет особых требований. Преимущественно Windows based-инфраструктура, требуется реализация программных балансировщиков нагрузки, репликации данных и автоматизированного механизма создания резервных копий.
Hyper-V
Не требуется Open-Source решение, преимущественно Windows based-инфраструктура (скорее всего есть специалисты), все остальное присутствует либо в составе либо на рынке

Требуется наиболее производительное бесплатное open source-решение для виртуализации небольшой (20-30 серверов) инфраструктуры на базе Linux и Windows виртуальных машин.
Xen
Требуется производительное (скорее всего и надёжное) Open-Source решение

Необходимо бесплатное, максимально совместимое и производительное решение для виртуализации Windows-инфраструктуры.
ESXi

Необходимо рабочее окружение для тестирования программного продукта на нескольких дистрибутивах Linux.
KVM

Задача 4
Опишите возможные проблемы и недостатки гетерогенной среды виртуализации (использования нескольких систем управления виртуализацией одновременно) и что необходимо сделать для минимизации этих рисков и проблем. Если бы у вас был выбор, создавали бы вы гетерогенную среду или нет?
Почти всегда плохо (поддержка разного железа и разных специалистов), если только не разрабатывается продукт, у которого наличие в требованиях
