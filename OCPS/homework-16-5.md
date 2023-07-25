# Домашнее задание к занятию «Решение задач оперативного учета. Часть 4»

## Цель задания

1. Закрепить полученные знания.
2. Научиться самостоятельно решать задачи оперативного учета из экзамена "1С:Специалист по Платформе".

Эта практика позволит вам определить свои сильные и слабые стороны в решении задач оперативного учета и пригодятся для самостоятельной подготовки к экзамену.

## Чеклист готовности к домашнему заданию

- Скачать каркасную конфигурацию [файл new_carcass_8_3_17_1496.dt](https://github.com/Bofh82/onec-mid-homeworks/blob/main/OCPS/new_carcass_8_3_17_1496.dt)
- Создать пустую информационную базу
- Загрузить в нее каркасную конфигурацию
- Просмотреть материал занятия

## Инструкция к заданию

1. Решите описанную задачу в конфигураторе
2. Протестируйте решение в пользовательском режиме
3. Отправьте на проверку в личном кабинете Нетологии один файл выгрузки базы данных (.dt), содержащий решение задачи. Файл прикрепите в раздел «решение» в практическом задании. Имя файла должно быть в формате "ФамилияИО_ОУ2.dt".

## Описание задачи

Необходимо создать интерфейс решения учебной задачи. В интерфейсе должно быть создано три раздела (Главное, Оперативный учет, Сервис). Панель навигации вместе с Панелью действий на закладке «Оперативный учет» должна обеспечивать доступ ко всем объектам данного раздела, которые используются при решении конкретной учебной задачи, в том числе и к регистрам.

Объекты должны быть сгруппированы по своему виду: справочники, документы, прочие объекты. Содержание остальных разделов определяется самостоятельно.
Примерный вид интерфейса показан ниже*

![Рисунок_ОУ1_1](https://user-images.githubusercontent.com/44517817/235097115-95c20495-6d40-4531-9a93-d9e5cbec9098.png)

*картинки для оформления можно взять из Библиотеки картинок [файл piclib.dt](https://github.com/netology-code/onec-mid-homeworks/blob/main/OCPS/piclib.dt)

Компания занимается оптовой торговлей. Взаиморасчеты с поставщиками ведутся в разрезе соглашений об условиях закупок. Поступление денежных средств поставщику отражается документом «Расход денег», приход товаров - документом «Приходная накладная». И в документе «Расход денег» и в документе «Приходная накладная» может быть указано только одно соглашение (в реквизите шапки).

В том случае, когда в документе «Расход денег» указано соглашение, необходимо проверить сумму поставок по этому соглашению. Если была поставка, то происходит погашение задолженности. Если сумма платежа превышает сумму поставки, то оставшиеся деньги должны быть зачтены как аванс. Аванс числится просто за контрагентом, без учета соглашения. Если соглашение в документе «Расход денег» не указано, то погашаются задолженности по соглашениям в порядке их даты оплаты (дата оплаты указывается в соглашении). В случае, когда сумма платежа больше всех долгов по поставке, оставшаяся сумма также зачитывается как аванс.

При проведении документа «Приходная накладная» необходимо производить проверку авансов. В том случае, если аванс есть, необходимо его погасить. Оставшаяся сумма должна быть учтена как долг по соглашению по поставке.
Весь учет ведется одновременно в 3-х валютах: рубли, доллары и евро. При проведении документов курс указывается непосредственно в самом документе. **Возникновение курсовых разниц при поставке и оплате не предполагается**.

Учет остатков номенклатуры не ведется.

Необходимо предоставить пользователю возможность самостоятельно добавлять к поставщикам произвольный набор дополнительных характеристик. Данный механизм должен быть реализован с помощью плана видов характеристик. Сами характеристики в настройках отчета должны быть отображены как реквизиты поставщика.

Необходимо создать отчет по состоянию взаиморасчетов по регионам на дату, где регион – это характеристика.
![image](https://github.com/netology-code/onec-mid-homeworks/assets/44517817/3f87eed8-be9a-444c-b4c3-310a73755250)

Дата отчета должна задаваться пользователем напрямую в форме отчета. В печатной форме заголовок и шапка отчета должны соответствовать заданию.

ОБЯЗАТЕЛЬНО! В пользовательском режиме заведите тестовый пример, приведенный в [файле «16.5 Исходные данные_ОУ3 к домашнему заданию.xlsx»](https://docs.google.com/spreadsheets/d/1HUY9wSDzpcMbkavgbQaG7iMTlr-GVmeM/edit?usp=share_link&ouid=116056574301476264521&rtpof=true&sd=true)

------

### Критерии оценки 

1. Зачёт — реализован весь требуемый функционал, нет критичных ошибок и нарушения логики. Полный перечень ошибок можно найти в [документе на сайте 1С, 3 стр.](https://static.1c.ru/rus/partners/training/files/ATT83PL.rtf?356jhteyner67j340)
2. Введены тестовые данные в пользовательском режиме.
3. На доработку — задание выполнено частично или не выполнено, в логике выполнения заданий есть противоречия, критичные ошибки.
Любые вопросы по решению задач задавайте в чате учебной группы.

*Примерное время выполнения: 45–180 минут*