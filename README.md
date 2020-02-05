# Курсовая работа
__Тема ВКР:__ Разработка программного продукта для исследования методов сортировки массивов и их сравнительного анализа

__Тема курсового проекта:__ Автоматизация сортировки массивов

__Объект исследования:__ Методы сортировки массивов

__Предмет исследования:__ Программный продукт, способный доказать преимущество того или иного метода сортировки массивов

__Процессы верхнего уровня:__

А1 Определение требований к проекту

А2 Подготовка программного обеспечения

А3 Сортировка массива

А4 Выдача результатов обработки

__Цель моделирования:__ Определение автоматизируемых функций

__Точка зрения:__ Программист

## Контекстная диаграмма А0 "Автоматизация сортировки массивов":
![Image alt](https://github.com/Hoshi089/Rudov.Ilya.github.io/blob/master/A0q.png)

## Декомпозиция блока А0 "Автоматизация сортировки массивов":
![Image alt](https://github.com/Hoshi089/Rudov.Ilya.github.io/blob/master/A0idef0q.png)

## Декомпозиция блока А2 "Подготовка ПО":
![Image alt](https://github.com/Hoshi089/Rudov.Ilya.github.io/blob/master/A2idef0q.png)

## Декомпозиция блока А3 "Сортировка массива":
![Image alt](https://github.com/Hoshi089/Rudov.Ilya.github.io/blob/master/A3idef0q.png)

## Определение основных средств автоматизации:

-Определение конфигурации технических средств - пк.

-Определение конфигурации программных средств - одноуровневая.

-Определение допустимых видов хранилищ и их размещения - база данных в памяти устройства, память устройства.

## Декомпозиция блока А31 "Выбор одного из методов сортировки" в DFD:
![Image alt](https://github.com/Hoshi089/Rudov.Ilya.github.io/blob/master/A31dfd.png)

## Декомпозиция блока А32 "Сортировка массива" в DFD:
![Image alt](https://github.com/Hoshi089/Rudov.Ilya.github.io/blob/master/A32dfd.png)

## Декомпозиция блока А33 "Обработка данных" в DFD:
![Image alt](https://github.com/Hoshi089/Rudov.Ilya.github.io/blob/master/A33dfd.png)
[Проект RAMUS](https://github.com/Hoshi089/Rudov.Ilya.github.io/blob/master/%D0%A0%D1%83%D0%B4%D0%BE%D0%B2.rsf)

# ER-Диаграмма (диаграммы классов без атрибутов) для всех потоков
![Image alt](https://github.com/Hoshi089/Rudov.Ilya.github.io/blob/master/uml4.png)

[код ее построения](https://github.com/Hoshi089/Rudov.Ilya.github.io/blob/master/uml2.txt)

# ER-Диаграмма (диаграммы классов без атрибутов) для всех ролей
![Image alt](https://github.com/Hoshi089/Rudov.Ilya.github.io/blob/master/uml3.png)

[код ее построения](https://github.com/Hoshi089/Rudov.Ilya.github.io/blob/master/uml3.txt)

# ER-Диаграмма (диаграммы классов без атрибутов) для всех модулей
![Image alt](https://github.com/Hoshi089/Rudov.Ilya.github.io/blob/master/uml1.png)

[код ее построения](https://github.com/Hoshi089/Rudov.Ilya.github.io/blob/master/uml1.txt)

# Расчетная часть

## Определение числовых показателей для цели потенциального проекта автоматизации

Данная программа позволит пользователю отсортировать массив без применения ручного труда, просчитает время сортировки и ее этапы, и выдаст конечный результат. На основе полученных результатов можно будет оценить эффективность каждого из методов, сравнив их с другими показателями. 

_Без системы:_ 

Предположим, что массив из 10 символов нужно отсортировать четырьмя способами. В случае отсутствия средств информационной поддрежки человек может совершить в среднем 2 ошибки. Даже одна ошибка может повлечь за собой искаженные данные во всем анализе эффективности методов сортировки.

Если же ошибки не произошло, на сортировку массива из 10 символов четырьмя способами без использования средств информационной поддержки уйдет в среднем 25 минут.

_С системой:_ 

Вероятность ошибки сокращается до 0%, следовательно искажение анализа упраздняется.

Сортировка массива из 10 символов одним способом уйдет в среднем 1,5 секунды. При вышеупомянутом количестве методов получим 1,5 * 4 = 6 с = 0,1 мин.

_Вывод:_

Проектируемое программное обеспечение поможет упразднить искаженные данные в анализе эффективности методов сортировки массивов, а так же потенциальный эффект от введения автоматизированного контроля составит 24,9 человекоминут за проведение одного анализа. 

## Определение числовых показателей для трудозатрат на разработку программных средств

Расчет невыровненных функциональных точек:

![Image alt](https://github.com/Hoshi089/Rudov.Ilya.github.io/blob/master/u1.PNG)

Определение числовых показателей для трудозатрат на разработку программных средств:

_Методом FPA/IFPUG_

![Image alt](https://github.com/Hoshi089/Rudov.Ilya.github.io/blob/master/u2.PNG)

Расчеты, выполненные первым методом FPA IFPUG, позволяют оценить сложность требуемых для создания информационной системы программных средств в 41 выровненных функциональных точек, а объем программного кода на языках программирования высокого уровня – 1784 строк кода.

_Методом COCOMO II_

![Image alt](https://github.com/Hoshi089/Rudov.Ilya.github.io/blob/master/u3.PNG)

Расчеты, выполненные вторым методом COCOMO II, позволяют оценить общие трудозатраты проекта разработки программных средств в 1 человеко-месяц, а ожидаемую продолжительность проекта, создаваемого с нуля – в 4 месяца. Решением этого ограничения является то, что проект находится в разработке с ноября этого года, а значит будет выполнен вовремя.
