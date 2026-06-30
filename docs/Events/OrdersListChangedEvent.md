# OrdersListChangedEvent

Событие: список заказов или статус одного/нескольких заказов изменился на аккаунте.

## Сигнатура

```python
OrdersListChangedEvent(runner_tag: str, purchases: int, sales: int)
```

## Атрибуты

| Атрибут | Тип | Описание |
|---------|-----|----------|
| `type` | `EventTypes.ORDERS_LIST_CHANGED` | Тип события |
| `purchases` | `int` | Текущее количество незавершённых покупок |
| `sales` | `int` | Текущее количество незавершённых продаж |

← [Назад к Events](README.md)
