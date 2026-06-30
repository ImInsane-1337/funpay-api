# Runner.generate_new_message_events()

Запрашивает историю переданных чатов и генерирует события новых сообщений.

## Сигнатура

```python
Runner.generate_new_message_events(
    chats_data: dict[int, str | None]
) -> dict[int, list[NewMessageEvent]]
```

## Параметры

| Параметр | Тип | Описание |
|----------|-----|----------|
| `chats_data` | `dict` | `{ID чата: никнейм или None}` |

## Возвращает

`dict[int, list[NewMessageEvent]]` — `{ID чата: [события]}`.

← [Назад к Runner](README.md)
