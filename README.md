Решение находится в виде DT файла для 1С https://disk.yandex.ru/d/5n08fjTVObrVFg
Видео с описанием решения https://disk.yandex.ru/i/_ArY5xPkdh5G_Q
Демо https://csmvstu.link.1c.ru/asml/ru/

Наша команда использовала для решения кейса «Построй свою универсальную систему» самый распространенный в РФ язык программирования учетно-ориентированных задач – 1С. В решении нами использованы такие библиотеки машинного обучения 1С как БиблиотекаСтандартныхПодсистем и библиотека интеллектуального анализа АнализДанных 

В ходе решения нами была создана клиент-серверный программный продукт, он размещен как веб-сервис по адресу в нашем тизере, пользователь – Администратор, пароля нет
В решении мы смоделировали реальные процессы формирования покупок товаров в ритейле. 
Основные автоматизированные бизнес процессы представлены на слайде.
 Основным учетным объектом выступил ЧекККМ. Он обезличен, после ввода формирует записи в БД СтатистическиеДанные
1 задача. Загрузка данных в БД. 
Загрузка данных не является сложной задачей. Методы все известны. Однако, мы не просто считываем данные, но и заполняем базы данных Номенклатура и ЧекиККМ, при этом Чеки ККМ фиксируют свои движения в специальном классе РегистрНакопления (у нас СтатистическиеДанные). Так рекомендовано делать при создании учетных торговых систем, этот класс некий аналог СУБД.
2 задача. Поиск и замена дублей товаров. 
Большой проблемой учета товаров в ритейле является проблема дублей наименований идентичных товаров. Поэтому нами был создан интеллектуальный модуль, позволяющий предопределить наличие таких дублей и, при необходимости, (это решает пользователь) заменить все дубли на единственное выбранное значение.
3 задача. Разработка рекомендательной системы. 
