# Логирование

1. Лучше всего выносить логирование в отдельный модуль (или хотя бы пакет)
2. Модуль должен определять (и реализовывать) интерфейс. Структура, реализующая интерфейс приватна для пакета модуля

## Zap или zerolog. 

По умолчанию лучше выбирать zerolog. В дальнейшем, если надо, то интерфейс позволяет использовать другую его реализацию.

Ответ от GPT:
| **Критерий**                          | **zerolog**                         | **zap**                             |
|---------------------------------------|-------------------------------------|-------------------------------------|
| **Высокая производительность**        | ✅                                   | ✅                                   |
| **JSON как основной формат логов**    | ✅                                   | ✅                                   |
| **Простота интеграции**               | ✅                                   | ❌ (требует больше конфигураций)    |
| **Нужен текстовый вывод**             | ❌                                   | ✅                                   |
| **Малый размер бинарного файла**      | ✅                                   | ❌                                   |
| **Сложные требования к логам**        | ❌                                   | ✅                                   |
| **Логирование в production-режиме**   | ✅                                   | ✅                                   |
| **Упрощенные требования в микросервисах** | ✅                                | ❌                                   |
