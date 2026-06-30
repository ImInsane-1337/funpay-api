# Runner.parse_chat_updates()

Парсит события чатов из объекта с `"type" == "chat_bookmarks"`.

## Сигнатура

```python
Runner.parse_chat_updates(obj: dict) -> list
```

## Возвращает

`list` событий: `InitialChatEvent | ChatsListChangedEvent | LastChatMessageChangedEvent | NewMessageEvent`

← [Назад к Runner](README.md)
