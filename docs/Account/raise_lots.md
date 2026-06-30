# Account.raise_lots()

Поднимает лоты в указанной подкатегории (кнопка «Поднять» на FunPay).

## Сигнатура

```python
Account.raise_lots(subcategory_id: int, subcategory_type: SubCategoryTypes) -> None
```

## Параметры

| Параметр | Тип | Описание |
|----------|-----|----------|
| `subcategory_id` | `int` | ID подкатегории |
| `subcategory_type` | `SubCategoryTypes` | Тип подкатегории |

> ⚠️ Нельзя поднимать лоты типа `SubCategoryTypes.CURRENCY`.

← [Назад к Account](README.md)
