# Runner.parse_order_updates()

Парсит события заказов из объекта с `"type" == "orders_counters"`.

## Сигнатура

```python
Runner.parse_order_updates(obj: dict) -> list
```

## Возвращает

`list` событий: `InitialOrderEvent | OrdersListChangedEvent | NewOrderEvent | OrderStatusChangedEvent`

← [Назад к Runner](README.md)
