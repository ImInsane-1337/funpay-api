# NewMessageEvent

Событие: в истории чата обнаружено новое сообщение.

## Сигнатура

```python
NewMessageEvent(
    runner_tag: str,
    message_obj: Message,
    stack: MessageEventsStack | None = None
)
```

## Атрибуты

| Атрибут | Тип | Описание |
|---------|-----|----------|
| `type` | `EventTypes.NEW_MESSAGE` | Тип события |
| `message` | `Message` | Объект нового сообщения |
| `stack` | `MessageEventsStack` | Стек всех новых сообщений из этого же запроса (пакета) |

## Пример

```python
for event in runner.listen():
    if event.type is enums.EventTypes.NEW_MESSAGE:
        msg = event.message
        # Проверяем, что сообщение прислал покупатель/собеседник, а не наш бот
        if msg.author_id != acc.id:
            print(f"Новое сообщение от {msg.author}: {msg.text}")
```

← [Назад к Events](README.md)
