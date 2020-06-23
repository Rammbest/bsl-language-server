# Глобальный модуль с постфиксом "Клиент" (CommonModuleNameGlobalClient)

| Тип | Поддерживаются<br/>языки | Важность | Включена<br/>по умолчанию | Время на<br/>исправление (мин) | Тэги |
| :-: | :-: | :-: | :-: | :-: | :-: |
| `Дефект кода` | `BSL` | `Важный` | `Да` | `5` | `standard` |

<!-- Блоки выше заполняются автоматически, не трогать -->
## Описание диагностики
<!-- Описание диагностики заполняется вручную. Необходимо понятным языком описать смысл и схему работу -->

Для глобальных модулей добавляется постфикс "Глобальный" (англ. "Global"), 
в этом случае постфикс "Клиент" добавлять не следует.

## Примеры
<!-- В данном разделе приводятся примеры, на которые диагностика срабатывает, а также можно привести пример, как можно исправить ситуацию -->

НеПравильно: 
РаботаСФайламиГлобальныйКлиент, InfobaseUpdateGlobalClient

Правильно: 
РаботаСФайламиГлобальный, InfobaseUpdateGlobal

## Источники
<!-- Необходимо указывать ссылки на все источники, из которых почерпнута информация для создания диагностики -->



[Стандарт: Тексты модулей](https://its.1c.ru/db/v8std#content:469:hdoc:3.2.1)

## Сниппеты

<!-- Блоки ниже заполняются автоматически, не трогать -->
### Экранирование кода

```bsl
// BSLLS:CommonModuleNameGlobalClient-off
// BSLLS:CommonModuleNameGlobalClient-on
```

### Параметр конфигурационного файла

```json
"CommonModuleNameGlobalClient": false
```