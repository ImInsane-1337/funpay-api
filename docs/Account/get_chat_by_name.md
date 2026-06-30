# Account.get_chat_by_name()

Находит чат по никнейму пользователя.

## Сигнатура

```python
Account.get_chat_by_name(username: str, make_request: bool = False) -> ChatShortcut | None
```

## Параметры

| Параметр | Тип | По умолч. | Описание |
|----------|-----|-----------|----------|
| `username` | `str` | — | Никнейм пользователя |
| `make_request` | `bool` | `False` | Делать доп. запрос, если чат не найден локально |

## Возвращает

`ChatShortcut | None` — чат или `None` если не найден.

## Пример

```python
chat = acc.get_chat_by_name("PlayerOne", make_request=True)
if chat:
    acc.send_message(chat.id, "Привет!")
```

← [Назад к Account](README.md)
