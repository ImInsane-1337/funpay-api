# Runner.mark_as_by_bot()

Помечает сообщение как отправленное ботом через `send_message()`. Предотвращает его обработку как входящего.

## Сигнатура

```python
Runner.mark_as_by_bot(chat_id: int, message_id: int) -> None
```

## Параметры

| Параметр | Тип | Описание |
|----------|-----|----------|
| `chat_id` | `int` | ID чата |
| `message_id` | `int` | ID сообщения |

← [Назад к Runner](README.md)
