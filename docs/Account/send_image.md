# Account.send_image()

Загружает и отправляет изображение в чат одним вызовом.

## Сигнатура

```python
Account.send_image(
    chat_id: int,
    image: str | IO[bytes],
    chat_name: str | None = None
) -> Message
```

## Параметры

| Параметр | Тип | Описание |
|----------|-----|----------|
| `chat_id` | `int` | ID чата |
| `image` | `str \| IO[bytes]` | Путь до файла или байты изображения |
| `chat_name` | `str \| None` | Никнейм собеседника |

## Возвращает

`Message` — объект отправленного сообщения.

## Пример

```python
acc.send_image(chat_id=123456, image="screenshot.png")

# Или с байтами
with open("photo.jpg", "rb") as f:
    acc.send_image(chat_id=123456, image=f)
```

← [Назад к Account](README.md)
