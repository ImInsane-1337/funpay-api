# InitialOrderEvent

Событие: заказ обнаружен при **первом запросе** Runner'а (при инициализации).

## Сигнатура

```python
InitialOrderEvent(runner_tag: str, order_obj: OrderShortcut)
```

## Атрибуты

| Атрибут | Тип | Описание |
|---------|-----|----------|
| `type` | `EventTypes.INITIAL_ORDER` | Тип события |
| `order` | `OrderShortcut` | Объект обнаруженного заказа |

← [Назад к Events](README.md)
