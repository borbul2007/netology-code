# Домашнее задание к занятию 1.  «Введение в виртуализацию»

## Задача 2
#### Выберите один из вариантов платформы в зависимости от задачи. Здесь нет однозначно верного ответа так как все зависит от конкретных условий: финансирование, компетенции специалистов, удобство использования, надежность, требования ИБ и законодательства, фазы луны. Тип платформы: - физические сервера; - паравиртуализация; - виртуализация уровня ОС.

#### Высоконагруженная база данных MySql, критичная к отказу.
_паравиртуализация_ или _физические сервера_ - Нет требований по производительности. Отказоустойчивоть решается кластеризацией. _физические сервера_ может быть дешевле дешевле

#### Различные web-приложения.
_паравиртуализация_ или _виртуализация уровня ОС_ (если приложения под один тип ОС)
  
#### Windows-системы для использования бухгалтерским отделом.
_паравиртуализация_ - Нет требований по производительности + Windows-системы

#### Системы, выполняющие высокопроизводительные расчёты на GPU.
_физические сервера_ - Необходима высокая производительность

## Задача 3
#### Выберите подходящую систему управления виртуализацией для предложенного сценария. Опишите ваш выбор.

####  100 виртуальных машин на базе Linux и Windows, общие задачи, нет особых требований. Преимущественно Windows based-инфраструктура, требуется реализация программных балансировщиков нагрузки, репликации данных и автоматизированного механизма создания резервных копий.
_Hyper-V_ или _VMware_ - Не требуется Open-Source решение, преимущественно Windows based-инфраструктура (скорее всего есть специалисты), все остальное присутствует либо в составе, либо на рынке

#### Требуется наиболее производительное бесплатное open source-решение для виртуализации небольшой (20-30 серверов) инфраструктуры на базе Linux и Windows виртуальных машин.
_KVM_ - Требуется производительное (скорее всего и надёжное) Open-Source решение 

#### Необходимо бесплатное, максимально совместимое и производительное решение для виртуализации Windows-инфраструктуры.
После того, как пропал _ESXi_ - такого не знаю. Раз уже есть Windows, то наверное, можно как-то задействовать _Hyper-V_, но надо разбираться с количеством включенных бесплатных лицензий в дистрибутивы. Ну или _Xen_

#### Необходимо рабочее окружение для тестирования программного продукта на нескольких дистрибутивах Linux.
_KVM_ - Нет особых требований и только Linux

## Задача 4
#### Опишите возможные проблемы и недостатки гетерогенной среды виртуализации (использования нескольких систем управления виртуализацией одновременно) и что необходимо сделать для минимизации этих рисков и проблем. Если бы у вас был выбор, создавали бы вы гетерогенную среду или нет?
Почти всегда плохо (поддержка разного железа и разных специалистов), если только не разрабатывается продукт, у которого это в требованиях.
