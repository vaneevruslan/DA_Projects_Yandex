# [Проверка гипотез по увеличению выручки в интернет-магазине](https://github.com/vaneevruslan/DA_Projects_Yandex/blob/main/07.%20Проверка%20гипотез%20по%20увеличению%20выручки%20в%20интернет-магазине/AB_tests_internet_shop.ipynb)

## Инструменты и навыки

`Python`, `pandas`, `matplotlib`, `scipy`, `numpy`, `datetime`, `A/B-тестирование`, `проверка статистических гипотез`

## Задачи проекта

Мы выступаем в роли аналитика крупного интернет-магазина. Вместе с отделом маркетинга мы подготовили список гипотез для увеличения выручки.

Нам необходимо:

- Приоритизировать гипотезы;
- Запустить A/B-тест и проанализировать результаты

## Выводы

В ходе исследоваания данных по увеличению выручки в интернет-магазине мы:

1. Провели обзор и предобработку входных данных;
2. Приоритизировали гипотезы, использовав фреймворки `ICE` и `RICE`:
- После применения фреймворка `ICE` наиболее приоритетными гипотезами являются:


    - Запустить акцию, дающую скидку на товар в день рождения (Гипотеза № 8)
    - Добавить два новых канала привлечения трафика, что позволит привлекать на 30% больше пользователей (Гипотеза № 0)
    - Добавить форму подписки на все основные страницы, чтобы собрать базу клиентов для email-рассылок (Гипотеза № 7)
    - Показать на главной странице баннеры с актуальными акциями и распродажами, чтобы увеличить конверсию (Гипотеза № 6)
    - Добавить блоки рекомендаций товаров на сайт интернет магазина, чтобы повысить конверсию и средний чек заказа (Гипотеза №2)
    
    
- После применения фреймворка `RICE` наиболее приоритетными гипотезами являются:


    - Добавить форму подписки на все основные страницы, чтобы собрать базу клиентов для email-рассылок (Гипотеза № 7)
    - Добавить блоки рекомендаций товаров на сайт интернет магазина, чтобы повысить конверсию и средний чек заказа (Гипотеза № 2)
    - Добавить два новых канала привлечения трафика, что позволит привлекать на 30% больше пользователей (Гипотеза № 0)
    - Показать на главной странице баннеры с актуальными акциями и распродажами, чтобы увеличить конверсию (Гипотеза № 6)
    - Запустить акцию, дающую скидку на товар в день рождения (Гипотеза № 8)

3. Провели A/B тест:

- была посчитана статистическая значимость различий между группами по «сырым» и «очищенным» данным;
- посчитана 95 и 99 перцентили для количества заказов и среднего чека (аномалией считалось более `2-х заказов` и стоимость более `28000 у.е`)
- по результату A/B теста мы приняли решение его остановить и признать успешным, даже несмотря на то, что по среднему чеку статистической значимости не обнаружено, так как мы выявили статистически значимое различие по конверсии между группами как в "сырых" так и "очищенных" от аномалий данных, что напрямую влияет на выручку.
