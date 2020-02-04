# Курсовая работа
__Тема ВКР:__ Разработка системы сбора персональных данных в дисконтной программе лояльности

__Тема курсового проекта:__ Сбор анкет и мониторинг легальности обработки ПДн

__Объект исследования:__ Дисконтная программа лояльности

__Предмет исследования:__ Система сбора персональных данных в дисконтной программе лояльности

__Процессы верхнего уровня:__

А1 Управлять (относится к внешней среде; обеспечивает соответствие требованиям к форме анкетирования и персоналу для проведения анкетирования; поддерживается внешней системой электронного документооборота)

А2 Подготавливать (относится к внешней среде; обеспечивает наличие формы анкетирования и квалифицированного персонала; поддерживается внешними системами электронного документооборота и дистанционного обучения персонала соответственно)

А3 Обрабатывать (относится к внутренней среде; поддерживается системой сбора и хранения ПДн)

А4 Контролировать (относится к внешней среде; обеспечивает оперативное обновление согласий на обработку ПДн согласно законодательству (ФЗ-152); поддерживается внешней базой данных и ответственными за процесс менеджерами)

__Цель моделирования:__ Определение автоматизируемых функций

__Точка зрения:__ Менеджер по продажам

## Контекстная диаграмма А0 "Обработка ПДн":
![Image alt](https://github.com/Hoshi089/VeronikaYakubova.github.io/blob/master/A00.png)

## Декомпозиция блока А0 "Обработка ПДн":
![Image alt](https://github.com/Hoshi089/VeronikaYakubova.github.io/blob/master/A0.png)

## Декомпозиция блока А1 "Определение требований к форме анкетирования и персоналу:
![Image alt](https://github.com/Hoshi089/VeronikaYakubova.github.io/blob/master/A1.png)

## Декомпозиция блока А3 "Загрузка ПДн":
![Image alt](https://github.com/Hoshi089/VeronikaYakubova.github.io/blob/master/A3n.png)

## Определение основных средств автоматизации:

-Определение конфигурации технических средств - SQL сервер, пк.

-Определение конфигурации программных средств - двухуровневая.

-Определение допустимых видов хранилищ и их размещения - база данных на SQL сервере, память устройства.

## Декомпозиция блока А33 "Обработка полученных данных" в DFD:
![Image alt](https://github.com/Hoshi089/VeronikaYakubova.github.io/blob/master/A33.png)

## Декомпозиция блока А4 "Контроль правомерности действий" в DFD:
![Image alt](https://github.com/Hoshi089/VeronikaYakubova.github.io/blob/master/A4.png)
[Проект RAMUS](https://github.com/Hoshi089/VeronikaYakubova.github.io/blob/master/Lab4.rsf)

# ER-Диаграмма (диаграммы классов без атрибутов) для всех потоков
![Image alt](https://github.com/Hoshi089/VeronikaYakubova.github.io/blob/master/Potoki1.png)

[код ее построения](https://github.com/Hoshi089/VeronikaYakubova.github.io/blob/master/Potoki.txt)

# ER-Диаграмма (диаграммы классов без атрибутов) для всех ролей
![Image alt](https://github.com/Hoshi089/VeronikaYakubova.github.io/blob/master/Roles2.png)

[код ее построения](https://github.com/Hoshi089/VeronikaYakubova.github.io/blob/master/Roles.txt)

# ER-Диаграмма (диаграммы классов без атрибутов) для всех модулей
![Image alt](https://github.com/Hoshi089/VeronikaYakubova.github.io/blob/master/Modules1.png)

[код ее построения](https://github.com/Hoshi089/VeronikaYakubova.github.io/blob/master/Modules1.txt)

# Расчетная часть

## Определение числовых показателей для цели потенциального проекта автоматизации

Данная система предназначена для компании по продаже мебели, желающей ввести программу лояльности для постоянных клиентов. Данная система позволит не только автоматизировать процесс хранения персональных данных клиентов (ФИО, номер мобильного телефона, электронная почта и т.д.), но и избежать непредвиденных расходов (а если быть конкретнее - штрафов) в случае продолжения хранения ПДн клиентов после истечения допустимого срока, предусмотренного законодательством, в размере 75 000 рублей единоразово. 

_Без системы:_ 

Предположим, что компании поступает 50 заполненных клиентами анкет в месяц. В случае отсутствия автоматизированного контроля сотрудник может допустить 4% ошибок - 2 ошибки в месяц. Одна такая ошибка может стоить 75 000 рублей, следовательно за 1 год это повлечет за собой финансовые потери в размере 2 * 75 000 * 12 = 1 800 000 рублей.

Если же ошибки не произошло, сотруднику необходимо повторно собрать с клиента согласие на обработку ПДн. Заполнение анкеты вручную у 1 клиента занимает в среднем 7 минут. При вышеупомянутом количестве клиентов в месяц получим 50 * 7 * 12 = 4200 минут = 70 часов за 1 год.

_С системой:_ 

Вероятность ошибки сокращается до 0%, следовательно финансовые потери упраздняются.

При повторном сборе согласий на обработку ПДн система формирует печатную форму анкеты с автозаполненными полями, в которой клиенту необходимо только поставить свою подпись. Проверка правильности данных в сформированной анкете и ее подписание занимает в среднем 2 минуты. При вышеупомянутом количестве клиентов в месяц получим 50 * 2 * 12 = 1200 минут = 20 часов за 1 год.

_Вывод:_

Проектируемая система поможет упразднить финансовые потери для компании, а так же потенциальный эффект от введения автоматизированного контроля составит 50 ч/час в год. 

## Определение числовых показателей для трудозатрат на разработку программных средств

Расчет невыровненных функциональных точек:

![Image alt](https://github.com/Hoshi089/VeronikaYakubova.github.io/blob/master/Ras1.PNG)

Определение числовых показателей для трудозатрат на разработку программных средств:

_Методом FPA/IFPUG_

![Image alt](https://github.com/Hoshi089/VeronikaYakubova.github.io/blob/master/Ras2.PNG)

Расчеты, выполненные первым методом FPA IFPUG, позволяют оценить сложность требуемых для создания информационной системы программных средств в 67 выровненных функциональных точек, а объем программного кода на языках программирования высокого уровня – 3283 строк кода.

_Методом COCOMO II_

![Image alt](https://github.com/Hoshi089/VeronikaYakubova.github.io/blob/master/Ras3.PNG)

Расчеты, выполненные вторым методом COCOMO II, позволяют оценить общие трудозатраты проекта разработки программных средств в 13 человеко-месяцев, а ожидаемую продолжительность проекта, создаваемого с нуля – в 8 месяцев. Решением этого ограничения является то, что проект находится в разработке с сентября этого года, а значит будет выполнен вовремя.
