# Method definitions must be placed before the module body operators (CodeBlockBeforeSub)

| Type | Scope | Severity | Activated<br/>by default | Minutes<br/>to fix | Tags |
| :-: | :-: | :-: | :-: | :-: | :-: |
| `Error` | `BSL`<br/>`OS` | `Blocker` | `Yes` | `5` | `error` |

<!-- Блоки выше заполняются автоматически, не трогать -->
## Description

<!-- Описание диагностики заполняется вручную. Необходимо понятным языком описать смысл и схему работу -->

The structure of the software module *(in general form)* is clearly defined:

- first comes the variable definition block
- then definitions of procedures and functions
- then the module code block.

Based on the structure described above, the location of the program code before the definition of methods is unacceptable.

## Examples

<!-- В данном разделе приводятся примеры, на которые диагностика срабатывает, а также можно привести пример, как можно исправить ситуацию -->

Wrong

```bsl
Method();
Message("Before methods");

Procedure Method()
// Method body
EndProcedure
```

## Sources

<!-- Необходимо указывать ссылки на все источники, из которых почерпнута информация для создания диагностики -->

<!-- Примеры источников

* Источник: [Стандарт: Тексты модулей](https://its.1c.ru/db/v8std#content:456:hdoc)
* Полезная информаця: [Отказ от использования модальных окон](https://its.1c.ru/db/metod8dev#content:5272:hdoc)
* Источник: [Cognitive complexity, ver. 1.4](https://www.sonarsource.com/docs/CognitiveComplexity.pdf) -->

- [Module structure](https://its.1c.ru/db/v8std/content/455/hdoc)

## Snippets

<!-- Блоки ниже заполняются автоматически, не трогать -->
### Diagnostic ignorance in code

```bsl
// BSLLS:CodeBlockBeforeSub-off
// BSLLS:CodeBlockBeforeSub-on
```

### Parameter for config

```json
"CodeBlockBeforeSub": false
```