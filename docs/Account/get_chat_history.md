# Account.get_chat_history()

Получает историю сообщений одного чата (до 100 последних).

## Сигнатура

```python
Account.get_chat_history(
    chat_id: int | str,
    last_message_id: int = 99999999999999999999999,
    interlocutor_username: str | None = None,
    from_id: int = 0
) -> list[Message]
```

## Параметры

| Параметр | Тип | По умолч. | Описание |
|----------|-----|-----------|----------|
| `chat_id` | `int \| str` | — | ID чата или текстовое обозначение |
| `last_message_id` | `int` | максимум | Начать с этого ID (фильтр FunPay) |
| `interlocutor_username` | `str \| None` | `None` | Никнейм собеседника (желательно для личных чатов) |
| `from_id` | `int` | `0` | Исключить сообщения с ID ниже этого |

## Возвращает

`list[Message]` — список сообщений. Подробнее: [Types/Message.md](../Types/Message.md)

← [Назад к Account](README.md)
