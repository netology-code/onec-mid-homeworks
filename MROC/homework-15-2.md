# Домашнее задание к занятию «Обмен с центральной базой и использование возможностей мобильного устройства»

## Цель задания

Изучить возможности и технологические особенности мобильной платформы фирмы 1С.

## Чеклист готовности к домашнему заданию

- [ ] подготовить информационную базу, полученную по итогу выполнения [домашнего задания к занятию 15-1, 2 задачи](homework-15-1.md);
- [ ] подготовить информационную базу, полученную по итогу выполнения [домашнего задания к занятию 12-3](../BSP/homework-12-3.md) или более позднего.

## Инструкция к заданию

1. Решите описанные задачи в конфигураторе.
2. Протестируйте решение в пользовательском режиме.
3. В личном кабинете Нетологии отправьте на проверку ссылку на файл dt с выгрузкой десктопной информационной базы и файл cf с конфигурацией мобильного приложения.

## Задание 1

Установка связи с центральной базой

### Процесс выполнения
1. В десктопном приложении на базе БСП, полученной из [домашнего задания к занятию 12-3](../BSP/homework-12-3.md), реализуйте HTTP сервис для обмена с мобильным приложением. Создайте роль для работы с сервисом и пользователя с логином **Курьер**. Сервис должен:
    - позволять проверить соединение с центральной базой с помощью метода ping,
    - позволять посмотреть количество заказов текущего пользователя - При нажатии на кнопку обмена, приложение должно получить от центральной базы количество заказов, в которых пользователь, под которым выполняется обмен, указан как ответственный. И вывести это число в удобном для пользователя сообщении. Сами документы или справочники передавать в мобильное приложение не нужно
2. В мобильном приложении из [2 задачи домашнего задания к занятию 15-1](homework-15-1.md) (ВАЖНО! Это должна быть новая конфигурация, а не конфигурация "Торговое предприятие", содержащая БСП) реализуйте механизм для вызова центральной базы:

    - создайте константы для хранения адреса подключения к базе, логина и пароля;
    - создайте обработку с командами проверки связи и получения количества заказов;
    - в рамках выполнения команд выполните вызовы методов сервиса, созданного на предыдущем шаге, и выведите пользователю в виде сообщения полученные из центральной базы данные.

3. Протестируйте обмен.

*Результат задания:* 
Мобильное приложение может проверять доступность центральной базы и получать количество заказов текущего курьера.

## Задание 2

Использование средств мобильной платформы

### Процесс выполнения
1. Проанализируйте синтакс-помощник на предмет возможностей мобильной платформы.
2. Реализуйте обработку, в ней продемонстрируйте работу 2 или более функций, специфических именно для мобильной платформы: фото, телефонные звонки, геопозиционирование и т. д.
3. В пояснительной записке к заданию опишите реализованные функции.

Постарайтесь органично включить возможности мобильной платформы в функционал приложения - например, сделать справочник сотрудников, в нем хранить фото сотрудника и номер телефона с возможностью сразу позвонить ему, или реализовать отправку уведомления клиентам о задержке доставки клиенту при помощи SMS.. Это творческое задание на креатив, посмотрите какие в принципе есть функции в платформе, подумайте, как они могли бы быть использованы.
 
*Результат задания:* 
В мобильном приложении присутствует функционал для демонстрации возможностей мобильной платформы.

------

## Правила приёма работы

В личном кабинете студента отправьте ссылку на файл dt с выгрузкой десктопной информационной базы и файл cf с конфигурацией мобильного приложения, которые соответствуют описанным функциональным требованиям. В пояснительной записке перечислите, какие возможности мобильной платформы продемонстрированы в демообработке.

------
## Критерии оценки

1. Зачёт: выполнены все задания, в них нет противоречий и нарушения логики. 
2. На доработку: задание выполнено частично или не выполнено, в логике выполнения заданий есть противоречия, существенные недостатки.

Все задачи обязательны к выполнению. Пожалуйста, присылайте на проверку все задачи сразу.

Любые вопросы по решению задач вы можете задать в чате учебной группы.

*Примерное время выполнения: до 180 минут*
