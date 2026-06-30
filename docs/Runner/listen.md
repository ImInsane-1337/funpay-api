# Runner.listen()

⭐ **Основной метод.** Бесконечный генератор событий FunPay.

## Сигнатура

```python
Runner.listen(
    requests_delay: int | float = 6,
    orders_delay: int | float = 0,
    ignore_errors: bool = False
) -> Generator[BaseEvent, None, None]
```

## Параметры

| Параметр | Тип | По умолч. | Описание |
|----------|-----|-----------|----------|
| `requests_delay` | `int \| float` | `6` | Задержка между запросами к FunPay (сек.) |
| `orders_delay` | `int \| float` | `0` | Доп. задержка между запросами заказов |
| `ignore_errors` | `bool` | `False` | Игнорировать сетевые ошибки и продолжать |

## Возвращает

Генератор событий `BaseEvent` и его наследников.

## Генерируемые события

| Событие | Когда |
|---------|-------|
| `InitialChatEvent` | Первый запуск — найден чат |
| `ChatsListChangedEvent` | Список чатов изменился |
| `LastChatMessageChangedEvent` | Последнее сообщение в чате изменилось |
| `NewMessageEvent` | Новое сообщение в истории |
| `InitialOrderEvent` | Первый запуск — найден заказ |
| `OrdersListChangedEvent` | Список заказов изменился |
| `NewOrderEvent` | Новый заказ |
| `OrderStatusChangedEvent` | Статус заказа изменился |

## Пример

```python
from FunPayAPI import Account, Runner, enums

acc = Account("<golden_key>").get()
runner = Runner(acc)

for event in runner.listen(requests_delay=4):
    if event.type is enums.EventTypes.NEW_MESSAGE:
        print(f"{event.message.author}: {event.message.text}")
    elif event.type is enums.EventTypes.NEW_ORDER:
        print(f"Новый заказ #{event.order.id} от {event.order.buyer_username}")
    elif event.type is enums.EventTypes.ORDER_STATUS_CHANGED:
        print(f"Статус заказа #{event.order.id} изменился")
```

← [Назад к Runner](README.md)
