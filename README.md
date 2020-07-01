# Набор правил для PHP_CodeSniffer

## Установка и подключение

Подключите пакет с помощью Composer:

```json
{
  "require": {
    "krenar-rm/phpcs": "~3.5.0"
  },
  "repositories": [
        {
            "type": "git",
            "url": "https://github.com/krenar-rm/phpcs.git"
        }
  ]
}
```
    
Также надо добавить в корень проекта файл `phpcs.xml` следующего вида:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<ruleset name="Dev-Standard">
    <rule ref="vendor/krenar-rm/phpcs/src/DevStandard"/>
    <file>src</file>
    <file>tests</file>
</ruleset>
```