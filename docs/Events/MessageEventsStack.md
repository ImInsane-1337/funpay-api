# MessageEventsStack

Класс представляет стек (пакет) событий новых сообщений, полученных в ходе одного запроса к серверам FunPay.  
Позволяет обрабатывать цепочки сообщений от одного пользователя разом, избегая дублирования ответов.

## Методы и свойства

| Метод | Тип возвращаемого значения | Описание |
|-------|----------------------------|----------|
| `get_stack()` | `list[NewMessageEvent]` | Возвращает весь список событий новых сообщений в стеке |
| `add_events(messages: list[NewMessageEvent])` | `None` | Добавляет события в стек |
| `id()` | `str` | Возвращает уникальный случайный ID стека (строка) |

## Пример использования

```python
for event in runner.listen():
    if event.type is enums.EventTypes.NEW_MESSAGE:
        # Получаем все новые сообщения из текущего пакета
        all_new_events = event.stack.get_stack()
        texts = [e.message.text for e in all_new_events if e.message.author_id != acc.id]
        if texts:
            print(f"Пользователь прислал серию сообщений: {texts}")
```

← [Назад к Events](README.md)
