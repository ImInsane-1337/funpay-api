# Runner.update_last_message()

Обновляет сохранённый текст последнего сообщения чата в кэше Runner'а.

## Сигнатура

```python
Runner.update_last_message(
    chat_id: int,
    message_text: str | None,
    message_time: str | None = None
) -> None
```

## Параметры

| Параметр | Тип | Описание |
|----------|-----|----------|
| `chat_id` | `int` | ID чата |
| `message_text` | `str \| None` | Текст (если `None` → сохраняется «Изображение») |
| `message_time` | `str \| None` | Время в формате `ЧЧ:ММ` |

← [Назад к Runner](README.md)
