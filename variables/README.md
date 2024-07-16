# Переменные кэша
Такие переменные хранятся в файле CMakeCache.txt
## Синтаксис
``` set(varName value... CACHE type "docstring" [FORCE])  ```
## Типы переменных кэша
* BOOL 
* FILEPATH
* PATH (путь к каталогу, а не файлу)
* STRING
* INTERNAL (переменная не предназначена для того, чтобы её изменял пользователь)
## Синтаксический сахар для задания переменной кэша
```
 option(optVar helpString [initialValue]) 
 ~
 set(optVar initialValue CACHE BOOL helpString)

```
По умолчанию initialValue=OFF
