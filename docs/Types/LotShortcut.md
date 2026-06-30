# LotShortcut

Класс представляет краткую информацию о лоте продавца на FunPay.

## Атрибуты

| Атрибут | Тип | Описание |
|---------|-----|----------|
| `id` | `int` | ID лота |
| `server_id` | `int \| None` | ID игрового сервера (если применимо) |
| `description` | `str \| None` | Краткое описание лота |
| `price` | `float` | Цена лота |
| `currency` | `Currency` | Валюта лота (RUB, USD, EUR) |
| `subcategory` | `SubCategory` | Подкатегория, к которой относится лот |
| `html` | `str` | HTML-код элемента лота в таблице |

← [Назад к Types](README.md)
