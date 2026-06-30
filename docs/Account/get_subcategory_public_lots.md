# Account.get_subcategory_public_lots()

Получает список всех опубликованных лотов в указанной подкатегории.

## Сигнатура

```python
Account.get_subcategory_public_lots(
    subcategory_type: SubCategoryTypes,
    subcategory_id: int
) -> list[LotShortcut]
```

## Параметры

| Параметр | Тип | Описание |
|----------|-----|----------|
| `subcategory_type` | `SubCategoryTypes` | Тип подкатегории |
| `subcategory_id` | `int` | ID подкатегории |

## Возвращает

`list[LotShortcut]` — список лотов. Подробнее: [Types/LotShortcut.md](../Types/LotShortcut.md)

← [Назад к Account](README.md)
