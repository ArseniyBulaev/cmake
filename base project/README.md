# Исполняемые файлы
`add_executable(targetName [WIN32] [MAOSX_BUNDLE] [EXCLUDE_FROM_ALL] sorce1 [sorce2 ...])`
* EXCLUDE_FROM_ALL - файл не будет включён в цель по умолчанию all
# Связывание целей
* PRIVATE - библиотека A использует B только во внутренней реализации
* PUBLIC - библиотека A использует B нетолько во внутренней реализации, но и в своём интерфейсе (тип из B передаётся методу из A)
* INTERFACE - библиотека A использует B только в интерфейсе

```
target_link_libraries(targetName
<PUBLIC|PRIVATE|INTERFACE> item1 [item2 ...]
<PUBLIC|PRIVATE|INTERFACE> item3 [item4 ...]
...
)

```