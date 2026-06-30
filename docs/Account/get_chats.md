# Account.get_chats()

Получает список чатов аккаунта (до 50 чатов).

## Сигнатура

```python
Account.get_chats(include_saved_by_bot: bool = False) -> list[ChatShortcut]
```

## Параметры

| Параметр | Тип | По умолч. | Описание |
|----------|-----|-----------|----------|
| `include_saved_by_bot` | `bool` | `False` | Включать чаты, сохранённые Runner'ом |

## Возвращает

`list[ChatShortcut]` — список чатов. Подробнее: [Types/ChatShortcut.md](../Types/ChatShortcut.md)

← [Назад к Account](README.md)
