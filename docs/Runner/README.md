# Runner

**Модуль:** `FunPayAPI.updater.runner`

Класс для получения новых событий FunPay в бесконечном цикле.

```python
Runner(account: Account, disable_message_requests: bool = False, disabled_order_requests: bool = False)
```

## Параметры конструктора

| Параметр | Тип | По умолч. | Описание |
|----------|-----|-----------|----------|
| `account` | `Account` | — | Инициализированный аккаунт (`Account.get()`) |
| `disable_message_requests` | `bool` | `False` | Отключить запросы истории чатов (нет `NewMessageEvent`) |
| `disabled_order_requests` | `bool` | `False` | Отключить запросы заказов (нет `NewOrderEvent`) |

## Атрибуты

| Атрибут | Тип | Описание |
|---------|-----|----------|
| `account` | `Account` | Привязанный аккаунт |
| `make_msg_requests` | `bool` | Делать запросы истории чатов? |
| `make_order_requests` | `bool` | Делать запросы заказов? |
| `saved_orders` | `dict[str, OrderShortcut]` | Кэш состояний заказов |
| `last_messages` | `dict[int, list]` | Последние сообщения `{chat_id: [текст, время]}` |
| `init_messages` | `dict[int, str]` | Начальные тексты для генерации событий |
| `by_bot_ids` | `dict[int, list[int]]` | Сообщения, отправленные ботом |
| `last_messages_ids` | `dict[int, int]` | Последние ID сообщений в чатах |

## Методы

| Метод | Описание |
|-------|----------|
| [listen()](listen.md) | ⭐ Основной генератор событий |
| [get_updates()](get_updates.md) | Запросить обновления у FunPay |
| [parse_updates()](parse_updates.md) | Распарсить ответ в события |
| [parse_chat_updates()](parse_chat_updates.md) | Парсинг событий чатов |
| [parse_order_updates()](parse_order_updates.md) | Парсинг событий заказов |
| [generate_new_message_events()](generate_new_message_events.md) | Генерация NewMessageEvent |
| [update_last_message()](update_last_message.md) | Обновить кэш последнего сообщения |
| [update_order()](update_order.md) | Обновить кэш заказа |
| [mark_as_by_bot()](mark_as_by_bot.md) | Пометить сообщение как от бота |

← [Назад к README](../../README.md)
