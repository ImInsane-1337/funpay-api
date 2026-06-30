# InitialChatEvent

Событие: чат обнаружен при **первом запросе** Runner'а (при инициализации).

## Сигнатура

```python
InitialChatEvent(runner_tag: str, chat_obj: ChatShortcut)
```

## Атрибуты

| Атрибут | Тип | Описание |
|---------|-----|----------|
| `type` | `EventTypes.INITIAL_CHAT` | Тип события |
| `chat` | `ChatShortcut` | Объект обнаруженного чата |

## Пример

```python
for event in runner.listen():
    if event.type is enums.EventTypes.INITIAL_CHAT:
        print(f"Инициализирован чат с пользователем: {event.chat.name} (ID: {event.chat.id})")
```

← [Назад к Events](README.md)
