# Исследование надёжности заёмщиков
## Задача проекта
Заказчик — кредитный отдел банка. Нужно разобраться, влияет ли семейное положение и количество детей клиента на факт погашения кредита в срок. Входные данные от банка — статистика о платёжеспособности клиентов.
## Цель
На основе статистики о платёжеспособности клиентов исследовать влияет ли семейное положение и количество детей клиента на факт возврата кредита в срок

Результаты исследования будут учтены при построении модели кредитного скоринга — специальной системы, которая оценивает способность потенциального заёмщика вернуть кредит банку.
## Инструменты
<code>предобработка данных</code> <code>python</code> <code>pandas</code> <code>PyMystem3</code>
## Краткое описание проекта
Входные данные от кредитного отдела банка — статистика о платёжеспособности клиентов. Очищены данные от выбросов, пропусков и дубликатов, а также преобразованы разные форматы данных. Заменены типы данных на соответствующие хранящимся данным. Удалены дубликаты. Выделены леммы в значениях столбца и категоризированны данные. Определена доля кредитоспособных клиентов. Проанализировано влияние семейного положения и количества детей клиента на факт возврата кредита в срок. Построена модель кредитного скоринга — специальной системы, которая оценивает способность потенциального заёмщика вернуть кредит банку.
## Выводы
* Чем больше у заёмщика детей, тем выше вероятность просрочки. Наибольшая вероятность просрочки у заёмщиков с 1, 2-мя и 4-мя детьми
* Заёмщики, состоявшие или состоящие в браке реже допускают просрочку. Наиболее часто просрочку допускают заёмщики из категории "не женат/не замужем" и "гражданский брак"
* Заёмщики с более высоким уровнем дохода реже допускают просрочку. Заёмщики с доходом меньше 30 тысяч рублей имеют самую высокую вероятность просрочки кредита.
* Кредиты взятые для операций с недвижимостью имеют наименьшую вероятность просрочки. Наибольшую имеют кредиты на образование и на операции с автомобилем.

**Важно:**

Описанные выше выводы по отдельности имеют достаточно слабую взаимосвязь с вероятностью просрочки кредита, однако при сочетании нескольких факторов, эта взаимосвязь растёт. Например, если заёмщик состоял или состоит в браке, имеет доход от 30 тысяч рублей и не имеет детей, то риски просрочек по кредиту не высоки, и наоборот: если заёмщик не состоит в браке, имеет доход меньше 30 тысяч, а также у него есть дети, то риски просрочки кредита будут высоки.
