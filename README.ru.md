# Country Parser Toolkit

[![CI](https://github.com/Raphailinc/Country-Parser-Toolkit/actions/workflows/ci.yml/badge.svg)](https://github.com/Raphailinc/Country-Parser-Toolkit/actions/workflows/ci.yml)

[English](README.md) · [Русский](README.ru.md)

Небольшой проект сбора и обработки сведений о странах: HTML-парсинг, нормализация записей и сводная статистика.

## Возможности

- Получение списка стран и формирование адресов Wikipedia.
- Извлечение полей из HTML-инфоблоков.
- Удаление дублей и сводки по населению, площади и валютам.
- Проверка парсинга на локальных HTML-образцах.

## Локальный запуск

```bash
python -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
python -m parse_algorithm --limit 10 -o output.json
```

## Проверки

```bash
python -m pytest
```

## Условия запуска и границы проекта

Живой сбор требует интернета и зависит от структуры внешних API и HTML. Локальные тесты парсера не подтверждают текущую доступность этих сервисов.
