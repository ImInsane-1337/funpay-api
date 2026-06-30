# Account.upload_image()

Загружает изображение на сервер FunPay. Для отправки используйте полученный ID в `send_message(image_id=...)`.

## Сигнатура

```python
Account.upload_image(image: str | IO[bytes]) -> int
```

## Параметры

| Параметр | Тип | Описание |
|----------|-----|----------|
| `image` | `str \| IO[bytes]` | Путь до файла или байты изображения |

## Возвращает

`int` — ID изображения на серверах FunPay.

## Пример

```python
image_id = acc.upload_image("photo.png")
acc.send_message(chat_id=123456, text=None, image_id=image_id)
```

← [Назад к Account](README.md)
