# OrderStatusChangedEvent

Событие: статус заказа изменился (например, заказ был подтверждён покупателем или возвращён).

## Сигнатура

```python
OrderStatusChangedEvent(runner_tag: str, order_obj: OrderShortcut)
```

## Атрибуты

| Атрибут | Тип | Описание |
|---------|-----|----------|
| `type` | `EventTypes.ORDER_STATUS_CHANGED` | Тип события |
| `order` | `OrderShortcut` | Объект заказа с обновлённым статусом |

## Пример

```python
for event in runner.listen():
    if event.type is enums.EventTypes.ORDER_STATUS_CHANGED:
        order = event.order
        print(f"Статус заказа #{order.id} изменился на: {order.status.name}")
```

← [Назад к Events](README.md)
