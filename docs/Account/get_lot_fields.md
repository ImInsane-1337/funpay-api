# Account.get_lot_fields()

Получает поля лота для дальнейшего редактирования и сохранения.

## Сигнатура

```python
Account.get_lot_fields(lot_id: int) -> LotFields
```

## Параметры

| Параметр | Тип | Описание |
|----------|-----|----------|
| `lot_id` | `int` | ID лота |

## Возвращает

`LotFields` — поля лота. Подробнее: [Types/LotFields.md](../Types/LotFields.md)

## Пример

```python
fields = acc.get_lot_fields(12345)
fields.set("price", 150)
acc.save_lot(fields)
```

← [Назад к Account](README.md)
