# Интеграционные тесты

## Запуск сервера
```
npm run start
```

## Запуск selenium 
```
selenium-standalone start
```

Тесты лежат по пути ```hermione/actions.hermione.js```
В файле ```hermione/helpers.js``` - вынесен вспомогательный объект с селекторами для удобного управления элементами.

Была идея поставить ```wdio-sync``` для теста мульти селекторов сразу, но почему-то не смог завести, если успею - исправлю.

## Проведены тесты:
1. Внешнее отображение эл-ов на страницах "История коммитов", "Файловая система", "Файл"
2. Переходы между страницами, а также по хлебным крошкам

# Модульные тесты


1. Хелпер Git
    - Получение объектов с коммитами на странице "История коммитов"
    - Разбитие строки коммита на объект
    - Получение из строки объекта в tree object

2. Навигация
    - Построение хлебных крошек на странице История коммитов
    - Построение хлебных крошек на странице с файлами
    - Построение хлебных крошек на странице файла
    
3. Контроллер для обработки конкретного коммита
    - Получение контента конкретного файла
