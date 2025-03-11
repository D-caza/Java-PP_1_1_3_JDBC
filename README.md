# Java-PP_1_1_3_JDBC
Working with a database using JDBC.
Описание задачи:
Необходимо ознакомиться с заготовкой и доработать приложение, которое взаимодействует с базой оперируя пользователем (класс User) и проверить свои методы заранее написанными JUnit тестами. По итогу все тесты должны быть пройдены.

Класс UserHibernateDaoImpl в рамках этой задачи не затрагивается (остаётся пустой)

User представляет из себя сущность с полями:

Long id
String name
String lastName
Byte age

Архитектура приложения создана с опорой на паттерн проектирования MVC (частично, у нас не WEB приложение)

Требования к классам приложения:
1) Классы dao/service должны реализовывать соответствующие интерфейсы
2) Класс dao должен иметь конструктор пустой/по умолчанию
3) Все поля должны быть private
4) service переиспользует методы dao
5) Обработка всех исключений, связанных с работой с базой данных должна находиться в dao
6) Класс Util должен содержать логику настройки соединения с базой данных
 
Необходимые операции:
1) Создание таблицы для User(ов) — не должно приводить к исключению, если такая таблица уже существует
2) Удаление таблицы User(ов) — не должно приводить к исключению, если таблицы не существует
3) Очистка содержания таблицы
4) Добавление User в таблицу
5) Удаление User из таблицы (по id)
6) Получение всех User(ов) из таблицы
