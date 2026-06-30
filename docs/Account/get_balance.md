# Account.get_balance()

Получает баланс аккаунта во всех валютах.

## Сигнатура

```python
Account.get_balance(lot_id: int = 18853876) -> Balance
```

## Параметры

| Параметр | Тип | По умолч. | Описание |
|----------|-----|-----------|----------|
| `lot_id` | `int` | `18853876` | ID лота, на странице которого проверяется баланс |

## Возвращает

`Balance` — объект с балансом. Подробнее: [Types/Balance.md](../Types/Balance.md)

## Пример

```python
balance = acc.get_balance()
print(f"Доступно: {balance.available_rub} RUB")
print(f"Доступно: {balance.available_usd} USD")
```

← [Назад к Account](README.md)
