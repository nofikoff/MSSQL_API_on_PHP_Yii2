
# Создание API интерфейса CRUD для существующие БД Microsoft SQL 
Выбран PHP феймворк Yii2

Исходные данные
- Логин пароль индивидуальный к БД и передается снаружи клиентом при каждом запросе (специфика проекта)
- Фреймворк используя переданные логин пароль подключается к БД и от имени пользователя формирует нужне SQL запросы 
- Результат возвращается в JSON

# Решение
- API структура разбита на модули v1 v2 что позволит в будущем параллельно запустить новую версию API без поломки старой v1 версии
на новом http адресе
- смотри точку входа api/index.php
- в конфиге URL менеджер и подключение модулей 
