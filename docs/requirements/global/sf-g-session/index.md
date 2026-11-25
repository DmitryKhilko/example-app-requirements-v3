---
priority: "must"
status: "анализ"
icon: lucide/file-pen-line
version: "0.00.00"
version_datetime: ""
editor: 
task_id:
release_id: 
release_date: 
---

# ГЛОБАЛЬНАЯ ДЕТАЛЬНАЯ ФУНКЦИОНАЛЬНОСТЬ {#sf}

## Журнал изменений {#change-history .collapsed}

- Записей пока нет.

## SF-G-SESSION. Истёкшая сессия {#sf-g-session .collapsed}

- **Статус**: анализ
- **Приоритет**: must
- **Стабильность**: низкая — экран входа и способ аутентификации не описаны, сообщение и судьба несохранённых
  данных не подтверждены (`UI-G-SESSION-001.H01`…`H03`)
- **Права доступа**: не ограничены: касается любого аутентифицированного пользователя
- **Использует**: [AR-001][]
- **Используется в**: [SF-PT-LIST][], [SF-PT-READ][], [SF-PT-CREATE][], [SF-PT-UPDATE][], [SF-PT-DELETE][]
- **Описание**: Если сессия пользователя истекла и API отвечает `401`, интерфейс переводит пользователя на вход и
после входа возвращает на тот же экран с теми же условиями.
- **Границы**:
    - **Входит**: Реакция любого экрана на ответ `401`, адрес возврата, сообщение об истёкшей сессии.
    - **Не входит**: Экран входа, способ аутентификации, срок жизни и продление сессии — их определяет технический
      стандарт.

### Состав требований {#sf-g-session-content .collapsed}

| Требование | Что описывает |
| :--- | :--- |
| [UI-G-SESSION-001][] | Переход на вход и возврат на экран |

### Как подключить {#sf-g-session-usage .collapsed}

Подключать не нужно: правило действует на всех экранах продукта. FR функциональностей не описывают ответ `401`, а
ссылаются на [UI-G-SESSION-001][]. Условия экрана, которые должны восстановиться, хранятся в адресе экрана.


[AR-001]: <../ar.md#ar-001>
[SF-PT-LIST]: <../../features/dict-product-type/sf-list/index.md#sf-pt-list>
[SF-PT-READ]: <../../features/dict-product-type/sf-read/index.md#sf-pt-read>
[SF-PT-CREATE]: <../../features/dict-product-type/sf-create/index.md#sf-pt-create>
[SF-PT-UPDATE]: <../../features/dict-product-type/sf-update/index.md#sf-pt-update>
[SF-PT-DELETE]: <../../features/dict-product-type/sf-delete/index.md#sf-pt-delete>
[UI-G-SESSION-001]: <ui.md#ui-g-session-001>
