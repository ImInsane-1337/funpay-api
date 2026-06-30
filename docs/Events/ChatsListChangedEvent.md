# ChatsListChangedEvent

Событие: список чатов изменился (например, поднялся существующий чат или появился новый).

## Сигнатура

```python
ChatsListChangedEvent(runner_tag: str)
```

## Атрибуты

| Атрибут | Тип | Описание |
|---------|-----|----------|
| `type` | `EventTypes.CHATS_LIST_CHANGED` | Тип события |

> **Примечание:** Данное событие сигнализирует лишь о факте изменения списка. Для детальной информации о сообщениях используйте события `NewMessageEvent` или `LastChatMessageChangedEvent`.

← [Назад к Events](README.md)
