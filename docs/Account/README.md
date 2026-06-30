# Account

**Модуль:** `FunPayAPI.account`

Класс для управления аккаунтом FunPay.

```python
Account(golden_key: str, user_agent: str | None = None, requests_timeout: int | float = 10, proxy: dict | None = None)
```

## Атрибуты

| Атрибут | Тип | Описание |
|---------|-----|----------|
| `golden_key` | `str` | Токен аккаунта |
| `user_agent` | `str \| None` | User-agent браузера |
| `requests_timeout` | `int \| float` | Тайм-аут запросов |
| `html` | `str \| None` | HTML главной страницы |
| `app_data` | `dict \| None` | Appdata |
| `id` | `int \| None` | ID аккаунта |
| `username` | `str \| None` | Никнейм |
| `active_sales` | `int \| None` | Активные продажи |
| `active_purchases` | `int \| None` | Активные покупки |
| `csrf_token` | `str \| None` | CSRF токен |
| `phpsessid` | `str \| None` | PHPSESSID сессии |
| `last_update` | `int \| None` | Время последнего обновления |
| `runner` | `Runner \| None` | Привязанный Runner |

## Методы

| Метод | Описание |
|-------|----------|
| [get()](get.md) | Получить/обновить данные аккаунта |
| [send_message()](send_message.md) | Отправить сообщение в чат |
| [send_image()](send_image.md) | Отправить изображение в чат |
| [upload_image()](upload_image.md) | Загрузить изображение на сервер |
| [get_chat()](get_chat.md) | Получить чат по ID |
| [get_chats()](get_chats.md) | Получить список чатов |
| [get_chat_by_name()](get_chat_by_name.md) | Найти чат по никнейму |
| [get_chat_history()](get_chat_history.md) | История одного чата |
| [get_chats_histories()](get_chats_histories.md) | История нескольких чатов |
| [get_order()](get_order.md) | Получить заказ по ID |
| [get_orders()](get_orders.md) | Получить список заказов |
| [get_balance()](get_balance.md) | Получить баланс |
| [get_user_profile()](get_user_profile.md) | Профиль пользователя |
| [get_categories()](get_categories.md) | Список категорий |
| [get_subcategory_public_lots()](get_subcategory_public_lots.md) | Лоты подкатегории |
| [get_lot_fields()](get_lot_fields.md) | Поля лота |
| [save_lot()](save_lot.md) | Сохранить лот |
| [raise_lots()](raise_lots.md) | Поднять лоты |
| [refund()](refund.md) | Вернуть деньги |

← [Назад к README](../../README.md)
