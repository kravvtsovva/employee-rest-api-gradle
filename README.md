# Employee REST API (TRPP Practical Work 2, Variant 1)

Этот проект — учебное задание на основе репозитория [rtu-mirea/trpp-second-1](https://github.com/rtu-mirea/trpp-second-1).

Цель: исправить ошибки сборки и настройки Gradle, собрать UberJar, протестировать REST API и устранить нарушения кодстайла.

## Что было сделано

- Найдена и добавлена отсутствующая зависимость в `build.gradle`
- Исправлены ошибки в структуре пакетов Java
- Сгенерирована документация (Javadoc)
- Собран UberJar с помощью `shadowJar`, файл включает фамилию
- Протестирован запуск на `localhost:8080`
- Протестированы запросы:
  - `GET /` — статус сервера
  - `GET /employee/{id}` — получение сотрудника по ID
- Выполнена проверка `checkstyleMain`, исправлены ошибки

## Сборка и запуск

```bash
./gradlew shadowJar
java -jar build/libs/trpp-second-1-YourSurname-all.jar
