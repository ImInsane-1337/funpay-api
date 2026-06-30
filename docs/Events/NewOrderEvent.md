# NewOrderEvent

Событие: в списке заказов обнаружен новый заказ (оплата).

## Сигнатура

```python
NewOrderEvent(runner_tag: str, order_obj: OrderShortcut)
```

## Атрибуты

| Атрибут | Тип | Описание |
|---------|-----|----------|
| `type` | `EventTypes.NEW_ORDER` | Тип события |
| `order` | `OrderShortcut` | Объект нового заказа |

## Пример

```python
for event in runner.listen():
    if event.type is enums.EventTypes.NEW_ORDER:
        order = event.order
        print(f"Покупатель {order.buyer_username} оплатил заказ #{order.id} на сумму {order.price} руб.")
```

← [Назад к Events](README.md)
