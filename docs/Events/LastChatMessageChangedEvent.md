# LastChatMessageChangedEvent

Событие: последнее сообщение в чате изменилось.

## Сигнатура

```python
LastChatMessageChangedEvent(runner_tag: str, chat_obj: ChatShortcut)
```

## Атрибуты

| Атрибут | Тип | Описание |
|---------|-----|----------|
| `type` | `EventTypes.LAST_CHAT_MESSAGE_CHANGED` | Тип события |
| `chat` | `ChatShortcut` | Объект чата с изменённым последним сообщением |

## Пример

```python
for event in runner.listen():
    if event.type is enums.EventTypes.LAST_CHAT_MESSAGE_CHANGED:
        print(f"Последнее сообщение в чате с {event.chat.name} теперь: {event.chat.last_message_text}")
```

← [Назад к Events](README.md)
