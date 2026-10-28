# Country Parser Toolkit

[![CI](https://github.com/Raphailinc/Country-Parser-Toolkit/actions/workflows/ci.yml/badge.svg)](https://github.com/Raphailinc/Country-Parser-Toolkit/actions/workflows/ci.yml)

[English](README.md) · [Русский](README.ru.md)

A small data-processing project that collects country names, parses country infoboxes and produces structured records and summary statistics.

## What it does

- Fetch a country list and build Wikipedia URLs.
- Parse infobox HTML into country records.
- Deduplicate records and compute population, area and currency summaries.
- Test parsing with offline HTML fixtures.

## Run locally

```bash
python -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
python -m parse_algorithm --limit 10 -o output.json
```

## Checks

```bash
python -m pytest
```

## Scope and implementation notes

Live collection requires network access and depends on upstream API/HTML structures. Offline parser tests do not guarantee current availability of those external services.
