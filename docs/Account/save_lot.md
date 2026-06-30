# Account.save_lot()

Создаёт новый или обновляет существующий лот.

## Сигнатура

```python
Account.save_lot(lot_fields: LotFields) -> None
```

## Параметры

| Параметр | Тип | Описание |
|----------|-----|----------|
| `lot_fields` | `LotFields` | Заполненные поля лота |

## Пример

```python
fields = acc.get_lot_fields(12345)
fields.set("active", 1)
fields.set("price", 200)
acc.save_lot(fields)
```

← [Назад к Account](README.md)
