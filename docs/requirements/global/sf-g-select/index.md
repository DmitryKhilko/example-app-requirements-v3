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

## SF-G-SELECT. Выделение строк и массовые действия {#sf-g-select .collapsed}

- **Статус**: анализ
- **Приоритет**: must
- **Стабильность**: средняя — не подтверждено, что выделение действует только на текущей странице
  (`UI-G-SELECT-001.H01`)
- **Права доступа**: флажки и панель видят только роли, которым разрешено хотя бы одно массовое действие
- **Использует**: [SF-G-TABLE][], [SF-G-PAG][], [NFR-005][], [дизайн-система][design-system] (Checkbox,
SelectionBar, Button)
- **Используется в**: [SF-PT-LIST][], [SF-PT-DELETE][]
- **Описание**: Пользователь отмечает строки таблицы и выполняет над ними действие из панели выделения.
- **Границы**:
    - **Входит**: Флажки строк и шапки, выделение строки, панель «Выбрано: N из M», снятие выделения, условия, при
      которых выделение снимается.
    - **Не входит**: Сами массовые действия (их задают функциональности, например удаление); выделение записей на
      нескольких страницах.

### Состав требований {#sf-g-select-content .collapsed}

| Требование | Что описывает |
| :--- | :--- |
| [UI-G-SELECT-001][] | Выделение строк и панель выделения |

### Как подключить {#sf-g-select-usage .collapsed}

Функциональность указывает приставку `data-testid`, роли, которым доступно выделение, и кнопки действий панели:
подпись, вариант кнопки, `data-testid` вида `<p>-selection-<действие>` и что открывает нажатие.


[NFR-005]: <../nfr.md#nfr-005>
[design-system]: <../design-system/index.md>
[SF-G-TABLE]: <../sf-g-table/index.md#sf-g-table>
[SF-G-PAG]: <../sf-g-pag/index.md#sf-g-pag>
[SF-PT-LIST]: <../../features/dict-product-type/sf-list/index.md#sf-pt-list>
[SF-PT-DELETE]: <../../features/dict-product-type/sf-delete/index.md#sf-pt-delete>
[UI-G-SELECT-001]: <ui.md#ui-g-select-001>
