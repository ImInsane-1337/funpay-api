# Runner.parse_updates()

Парсит ответ `get_updates()` и создаёт объекты событий всех типов.

## Сигнатура

```python
Runner.parse_updates(updates: dict) -> list[BaseEvent]
```

## Параметры

| Параметр | Тип | Описание |
|----------|-----|----------|
| `updates` | `dict` | Результат `Runner.get_updates()` |

## Возвращает

Список событий всех типов.

← [Назад к Runner](README.md)
