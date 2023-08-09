# HW-28.1
ИТОГОВЫЙ ПРОЕКТ ПО АВТОМАТИЗАЦИИ ТЕСТИРОВАНИЯ (PJ-04)

В рамках выполнения итогового проекта требуется протестировать интерфейс авторизации в личном кабинете Ростелеком Информационные Технологии.

Объект тестирования: https://b2c.passport.rt.ru

Заказчик передал вам следующее задание:

Протестировать требования.
Разработать тест-кейсы (не менее 15). Необходимо применить несколько техник тест-дизайна.
Провести автоматизированное тестирование продукта (не менее 20 автотестов). Заказчик ожидает по одному автотесту на каждый написанный тест-кейс. Оформите свой набор автотестов в GitHub.
Оформить описание обнаруженных дефектов. Во время обучения вы работали с разными сервисами и шаблонами, используйте их для оформления тест-кейсов и обнаруженных дефектов. (если дефекты не будут обнаружены, то составить описание трех дефектов)

Результат работы:

Тестирование требований, Тест-кейсы и баг-отчеты представлены в гугл-таблице: [https://docs.google.com/spreadsheets/d/15_bRnwRjYazeY_O38of8pPxIuTWnatsR/edit?usp=sharing&ouid=108049235031232211561&rtpof=true&sd=true](https://docs.google.com/spreadsheets/d/1onHQ9sZBz9Jr5PfnRg8j_c2GCKmuLvD5/edit?usp=sharing&ouid=111839530828328238177&rtpof=true&sd=true)

Проведено ручное и автоматизированное тестирование с использованием PyTest и Selenium

Для составления и написания тест-кейсов применены техники тест-дизайна: классы эквивалентности, анализ граничных значений, предугадывание ошибок.

Комментарий по автотестам:

В файле base_data.py находятся базовые классы, процедуры, функции и локаторы для автотестов

В файле settings.py - регистрационные данные для позитивных тестов авторизации

В файле tests_SF_RT_passport.py - автотесты. Все тесты помечены номером, который совпадает с номером тест-кейса в файле: [https://docs.google.com/spreadsheets/d/15_bRnwRjYazeY_O38of8pPxIuTWnatsR/edit?usp=sharing&ouid=108049235031232211561&rtpof=true&sd=true](https://docs.google.com/spreadsheets/d/1onHQ9sZBz9Jr5PfnRg8j_c2GCKmuLvD5/edit?usp=sharing&ouid=111839530828328238177&rtpof=true&sd=true)

запуск автотестов (драйвер в одной папке с тест-скриптом)

python -m pytest -v --driver Chrome --driver-path chromedriver.exe test_SF_RT_passport.py

В корне проекта в файле requirements.txt описаны используемые библиотеки.
