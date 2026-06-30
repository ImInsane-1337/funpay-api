# Account.get_order()

Получает полную информацию о конкретном заказе.

## Сигнатура

```python
Account.get_order(order_id: str) -> Order
```

## Параметры

| Параметр | Тип | Описание |
|----------|-----|----------|
| `order_id` | `str` | ID заказа (напр. `"ABCD1234"`) |

## Возвращает

`Order` — полный объект заказа. Подробнее: [Types/Order.md](../Types/Order.md)

## Пример

```python
order = acc.get_order("ABCD1234")
print(order.title, order.price, order.status)
```

← [Назад к Account](README.md)
