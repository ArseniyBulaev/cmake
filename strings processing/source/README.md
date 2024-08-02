# Обработка сторок. стр 37
## Поиск
```string(FIND inputString subString outVar [REVERSE])```
## Замена
```string(REPLACE matchString replaceWith outVar input [input...])```
## Регулярные выражения
* ```string(REGEX MATCH regex outVar input [input ...])```
* ```string(REGEX MATCHALL regex outVar input [input ...])```
* ```string(REGEX REPLACE regex replaceWith outVar input [input ...])```
Ссылаться на совпадения в replaceWith, используя \1, \2 ... (В команде слеши должны быть экранированы: \1 -> \\1)
## Подстрока
* ```string(SUBSTRING input index length outVar)```
 index - начало подстрокаи. length - длина извлекаемой подстроки. Если length = -1 возвращаются символы до конца строки
## Длина, Нижний регистр, Верхний регистр, удаление пробелов
* ```string(LENGTH input outVar)```
* ```string(TOLOWER input outVar)```
* ```string(TOUPPER input outVar)```
* ```string(STRIP input outVar)```