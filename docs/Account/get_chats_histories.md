# Account.get_chats_histories()

Получает историю нескольких чатов одним запросом.
- Личный чат: до **50** сообщений
- Публичный чат: до **25** сообщений

## Сигнатура

```python
Account.get_chats_histories(
    chats_data: dict[int | str, str | None]
) -> dict[int, list[Message]]
```

## Параметры

| Параметр | Тип | Описание |
|----------|-----|----------|
| `chats_data` | `dict` | `{ID чата: никнейм или None}` |

## Возвращает

`dict[int, list[Message]]` — `{ID чата: [сообщения]}`.

## Пример

```python
histories = acc.get_chats_histories({
    48392847: "PlayerOne",
    58392098: "PlayerTwo",
    38948728: None  # никнейм неизвестен
})
for chat_id, messages in histories.items():
    print(f"Чат {chat_id}: {len(messages)} сообщений")
```

← [Назад к Account](README.md)
