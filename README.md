# Spring Boot приложение "Библиотека"

## Описание

Это Spring MVC приложение под названием "Библиотека", предназначенное для управления библиотекой книг и взаимодействия с читателями. Приложение сконфигурировано с использованием Spring Boot.

### Используемые технологии

*   **Spring Boot** 
*   **Spring MVC**  
*   **Шаблонизатор Thymeleaf**  
*   **Hibernate** 
*   **Hibernate Validator** 
*   **Spring Data JPA** 
*   **PostgreSQL** 

## Функциональность

Приложение реализует следующий функционал:

*   **Управление сущностями "Человек" и "Книга":**
    *   Добавление новых записей.
    *   Редактирование существующих записей.
    *   Удаление записей.

*   **Выдача и возврат книг:**
    *   На странице книги:
        *   **Если книга свободна:**  Предоставляется выпадающий список всех зарегистрированных пользователей для привязки книги к конкретному человеку.
        *   **Если книга занята:**  Отображается информация о текущем владельце книги и возможность "отвязать" книгу (вернуть ее в библиотечный фонд).

*   **Просмотр информации о пользователе и взятых книгах:**
    *   На странице пользователя отображается список взятых им книг.
    *   Если у пользователя нет взятых книг, отображается соответствующее сообщение.
    *   **Просроченные книги:** Книги, взятые более 10 дней назад и не возвращенные, подсвечиваются красным цветом.

*   **Поиск книг по названию:**
    *   Поиск возвращает список книг, название которых начинается с введенной пользователем строки.

*   **Пагинация и сортировка:**
    *   На странице списка книг реализована пагинация для удобного просмотра большого количества записей.
    *   Книги можно сортировать по году издания.
