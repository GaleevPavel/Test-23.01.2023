#  Итоговый проект по автоматизации тестирования:
## Объект тестирования:(https://b2c.passport.rt.ru)

# Для тестирования сайта были использованы:
- ручные и автоматизированные тесты
- разбиение на классы эквивалентности
- анализ граничных значений
- тестирование состояний и переходов

## тест-кейсы и баг-репорты здесь: https://docs.google.com/spreadsheets/d/16SpEWKnky903jaoomSKN7AmZjqWvcsua__6D8cudg7c/edit?usp=sharing
# Тесты настроены на запуск через Run! 

## Окружение: 
Google Chrome Version Версия 112.0.5615.121 (Официальная сборка), (64 бит)
Windows 10 

Использована комбинация:   
.send_keys(Keys.CONTROL, 'a')   
.send_keys(Keys.DELETE)   


## Папка tests: 
test_negative_auth_page - тестируем негативные сценарии страницы авторизации   
test_negative_reg_page - тестируем негативные сценарии страницы регистрации test_negative_new_pass_page - тестируем негативные сценарии страницы восстановления пароля   
test_positive_auth_page - тестируем позитивные сценарии страницы авторизации   
test_positive_reg_page - тестируем позитивные сценарии страницы регистрации   
test_positive_new_pass_page - тестируем позитивные сценарии страницы восстановления пароля

## Папка pages: 
Api_RegMail - GET-запросы к виртуальному почтовому ящику (1secmail.com) для получения валидного 
e-mail и кода для регистрации на сайте/восстановления пароля.   
locators - локаторы XPath и CSS на web-элементы сайта   
auth - функции-обёртки для локаторов, распределённые по классам в зависимости от тематики тестов   
base - функции для применения к локаторам явных ожиданий, получения главной страницы сайта и пути текущей страницы   
config - исходные статические данные   
settings - учетные данные, используемые в процессе теста



