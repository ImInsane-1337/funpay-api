# BaseEvent

Базовый класс всех событий в FunPayAPI.

## Сигнатура

```python
BaseEvent(
    runner_tag: str,
    event_type: EventTypes,
    event_time: int | float | None = None
)
```

## Атрибуты

| Атрибут | Тип | Описание |
|---------|-----|----------|
| `type` | `EventTypes` | Тип события |
| `runner_tag` | `str` | Тег Runner'а, сгенерировавшего событие |
| `event_time` | `float` | Время генерации события (unix timestamp) |

← [Назад к Events](README.md)
