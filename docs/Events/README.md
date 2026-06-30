# Events

**Модуль:** `FunPayAPI.updater.events`

Классы событий, генерируемых `Runner.listen()`.

## Иерархия

```
BaseEvent
├── Чаты
│   ├── InitialChatEvent           (INITIAL_CHAT)
│   ├── ChatsListChangedEvent      (CHATS_LIST_CHANGED)
│   ├── LastChatMessageChangedEvent(LAST_CHAT_MESSAGE_CHANGED)
│   └── NewMessageEvent            (NEW_MESSAGE) → MessageEventsStack
└── Заказы
    ├── InitialOrderEvent          (INITIAL_ORDER)
    ├── OrdersListChangedEvent     (ORDERS_LIST_CHANGED)
    ├── NewOrderEvent              (NEW_ORDER)
    └── OrderStatusChangedEvent    (ORDER_STATUS_CHANGED)
```

## Все классы

| Класс | Тип события | Файл |
|-------|------------|------|
| `BaseEvent` | — | [BaseEvent.md](BaseEvent.md) |
| `InitialChatEvent` | `INITIAL_CHAT` | [InitialChatEvent.md](InitialChatEvent.md) |
| `ChatsListChangedEvent` | `CHATS_LIST_CHANGED` | [ChatsListChangedEvent.md](ChatsListChangedEvent.md) |
| `LastChatMessageChangedEvent` | `LAST_CHAT_MESSAGE_CHANGED` | [LastChatMessageChangedEvent.md](LastChatMessageChangedEvent.md) |
| `NewMessageEvent` | `NEW_MESSAGE` | [NewMessageEvent.md](NewMessageEvent.md) |
| `MessageEventsStack` | — | [MessageEventsStack.md](MessageEventsStack.md) |
| `InitialOrderEvent` | `INITIAL_ORDER` | [InitialOrderEvent.md](InitialOrderEvent.md) |
| `OrdersListChangedEvent` | `ORDERS_LIST_CHANGED` | [OrdersListChangedEvent.md](OrdersListChangedEvent.md) |
| `NewOrderEvent` | `NEW_ORDER` | [NewOrderEvent.md](NewOrderEvent.md) |
| `OrderStatusChangedEvent` | `ORDER_STATUS_CHANGED` | [OrderStatusChangedEvent.md](OrderStatusChangedEvent.md) |

← [Назад к README](../../README.md)
