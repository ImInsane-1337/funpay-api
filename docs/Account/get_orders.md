# Account.get_orders()

Получает список заказов аккаунта с фильтрацией по статусу.

## Сигнатура

```python
Account.get_orders(
    include_paid: bool = True,
    include_closed: bool = True,
    include_refunded: bool = True,
    exclude: list[str] | None = None,
    start_from: str | None = None,
    pages: int = 1,
    delay: int | float = 1
) -> tuple[list[OrderShortcut], str | None]
```

## Параметры

| Параметр | Тип | По умолч. | Описание |
|----------|-----|-----------|----------|
| `include_paid` | `bool` | `True` | Включать оплаченные заказы |
| `include_closed` | `bool` | `True` | Включать закрытые заказы |
| `include_refunded` | `bool` | `True` | Включать возвращённые заказы |
| `exclude` | `list[str] \| None` | `None` | ID заказов для исключения |
| `start_from` | `str \| None` | `None` | ID заказа, с которого начать |
| `pages` | `int` | `1` | Кол-во страниц для загрузки |
| `delay` | `int \| float` | `1` | Задержка между страницами (сек.) |

## Возвращает

`tuple[list[OrderShortcut], str | None]` — список заказов и ID следующей страницы (или `None`).

## Пример

```python
orders, next_page = acc.get_orders(include_closed=False, pages=2)
for order in orders:
    print(f"#{order.id} — {order.title} ({order.status})")
```

← [Назад к Account](README.md)
