# module-20
# Список изменений

## В папке task_18 reworked:

1.  Применение принципа **DRY**.

    projects-list\_\_item1, 2 и 3 заменен на projects-list\_\_item

    -   Вместо объявления 3-ёх констант ссылок слайда - одно объявление массива (js 11-я строчка)
    -   Тоже самое с точками слайда (js 22-я строчка)
    -   Вместо 3-ёх прослушек ссылок - одна через массив (js 57-я строчка)
    -   Тоже самое с прослушкой точек слайдера (js 79-я строчка)
    -   Тоже самое при установке изначальных классов ссылкам (js 134-я строчка)
    -   Тоже самое при установке изначальных классов точкам (js 144-я строчка)

2.  Применение принципа **KISS**.

    -   изменение блока кода с if на switch (js 190-я строчка)
   
3.  Применение принципа **YAGNI**.
   В связи с тем что в задании необходимо было произвести верску по макету, то для реализации принципа YAGNI необходимо полностью удалить элементы JS, а так же бургер-меню из HTML и CSS.

## В папке task_19 reworked:

4. Применение принципа **SOLID**.

    - До изменения метод checkPowerConsumption класса ConsumptionType находился в нём, это не соотвествует принципу ISP. Если мне понадобится сделать потомков от классa Appliances, например разделив бытовую технику по типам использования: для пригтовления пищи, для развлечения, для работы, для уборки и т.д. То для того что бы рассчитать поттебляему мощность придётся делать потомков от класса ConsumptionType, что не совсем правильно. При переносе метода checkPowerConsumption в базовый класс, эта проблема исчезает. Всем потомкам будет доступен необходимый им метод.

# Семантика и валидность

Проверил на сайте https://validator.w3.org/

Результат проверки: Document checking completed. No errors or warnings to show.

# БЭМ и линтеры

Я использую линтеры HTMLHint и Prettier.

