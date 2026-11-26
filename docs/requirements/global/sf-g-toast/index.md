---
priority: "must"
status: "анализ"
icon: lucide/file-pen-line
order: 140
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

## SF-G-TOAST. Всплывающие уведомления {#sf-g-toast .collapsed}

- **Статус**: анализ
- **Приоритет**: must
- **Стабильность**: средняя — не подтверждены время показа успеха, вид предупреждения и порядок нескольких
  уведомлений (`UI-G-TOAST-001.H01`…`H03`)
- **Права доступа**: не ограничены: уведомление видит пользователь, выполнивший операцию
- **Использует**: [NFR-002][], [NFR-005][], [дизайн-система][design-system] (Toast)
- **Используется в**: [FR-PT-LIST-005][], [UI-PT-001][], [FR-PT-CREATE-003][], [FR-PT-UPDATE-003][],
[FR-PT-ACTIVATION-002][], [FR-PT-DELETE-003][]
- **Описание**: Единые правила всплывающих уведомлений о результате операции: виды, вид и положение на экране, время
показа, закрытие, доступность и атрибуты для автотестов. Тексты уведомлений задают FR функциональностей.
- **Границы**:
    - **Входит**: Уведомления «Готово» и «Ошибка», вид карточки, положение, время показа, закрытие, несколько
      уведомлений подряд, роли и атрибуты доступности.
    - **Не входит**: Тексты уведомлений (задают FR функциональностей); ошибки полей формы (показываются под полями);
      уведомления в колокольчике шапки.

### Состав требований {#sf-g-toast-content .collapsed}

| Требование | Что описывает |
| :--- | :--- |
| [UI-G-TOAST-001][] | Всплывающее уведомление |

### Как подключить {#sf-g-toast-usage .collapsed}

Функциональность указывает в своих FR, после какого события показывается уведомление, его вид и текст. Текст успеха
называет результат и, если записей несколько, их количество («Удалено изделий: 2.»); текст ошибки — причину без
технических подробностей.


[NFR-002]: <../nfr.md#nfr-002>
[NFR-005]: <../nfr.md#nfr-005>
[design-system]: <../design-system/index.md>
[UI-G-TOAST-001]: <ui.md#ui-g-toast-001>
[FR-PT-LIST-005]: <../../features/dict-product-type/sf-list/fr.md#fr-pt-list-005>
[UI-PT-001]: <../../features/dict-product-type/ui.md#ui-pt-001>
[FR-PT-CREATE-003]: <../../features/dict-product-type/sf-create/fr.md#fr-pt-create-003>
[FR-PT-UPDATE-003]: <../../features/dict-product-type/sf-update/fr.md#fr-pt-update-003>
[FR-PT-ACTIVATION-002]: <../../features/dict-product-type/sf-activation/fr.md#fr-pt-activation-002>
[FR-PT-DELETE-003]: <../../features/dict-product-type/sf-delete/fr.md#fr-pt-delete-003>
