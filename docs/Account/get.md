# Account.get()

Получает и обновляет данные аккаунта. Вызывать каждые **40–60 минут** для обновления `phpsessid`.

## Сигнатура

```python
Account.get(update_phpsessid: bool = False) -> Account
```

## Параметры

| Параметр | Тип | По умолч. | Описание |
|----------|-----|-----------|----------|
| `update_phpsessid` | `bool` | `False` | Обновить `phpsessid` или использовать старый |

## Возвращает

`Account` — объект аккаунта с обновлёнными данными.

## Пример

```python
acc = Account("<golden_key>").get()
print(acc.username)  # Никнейм
print(acc.id)        # ID аккаунта
```

← [Назад к Account](README.md)
