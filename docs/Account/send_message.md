# Account.send_message()

Отправляет текстовое сообщение в чат.

## Сигнатура

```python
Account.send_message(
    chat_id: int,
    text: str | None,
    chat_name: str | None = None,
    image_id: int | None = None
) -> Message
```

## Параметры

| Параметр | Тип | Описание |
|----------|-----|----------|
| `chat_id` | `int` | ID чата |
| `text` | `str \| None` | Текст сообщения |
| `chat_name` | `str \| None` | Никнейм собеседника (для приватного чата) |
| `image_id` | `int \| None` | ID ранее загруженного изображения |

## Возвращает

`Message` — объект отправленного сообщения.

## Пример

```python
acc.send_message(chat_id=123456, text="Привет!")

# С изображением
img_id = acc.upload_image("photo.png")
acc.send_message(chat_id=123456, text="Смотри:", image_id=img_id)
```

← [Назад к Account](README.md)
