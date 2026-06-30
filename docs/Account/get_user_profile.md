# Account.get_user_profile()

Получает публичный профиль пользователя FunPay по его ID.

## Сигнатура

```python
Account.get_user_profile(user_id: int) -> UserProfile
```

## Параметры

| Параметр | Тип | Описание |
|----------|-----|----------|
| `user_id` | `int` | ID пользователя |

## Возвращает

`UserProfile` — профиль пользователя. Подробнее: [Types/UserProfile.md](../Types/UserProfile.md)

## Пример

```python
profile = acc.get_user_profile(12345)
print(profile.username, profile.active_lots)
```

← [Назад к Account](README.md)
