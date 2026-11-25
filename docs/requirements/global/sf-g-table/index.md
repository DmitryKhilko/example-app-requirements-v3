---
priority: "must"
status: "анализ"
icon: lucide/file-pen-line
order: 30
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

## SF-G-TABLE. Таблица списка и её состояния {#sf-g-table .collapsed}

- **Статус**: анализ
- **Приоритет**: must
- **Стабильность**: средняя — тексты ошибки загрузки и отсутствия прав достроены по дизайн-системе
  (`UI-G-TABLE-002.H01`)
- **Права доступа**: определяет операция списка, которая подключает функциональность
- **Использует**: [NFR-002][], [NFR-004][], [NFR-005][], [SF-G-TOAST][], [SF-G-SESSION][],
[дизайн-система][design-system] (DataTable, Badge, EmptyState, Skeleton)
- **Используется в**: [SF-PT-LIST][]
- **Описание**: Единые правила таблицы записей на экране списка: шапка, строки, форматы значений, открытие записи и
состояния таблицы (загрузка, пусто, ошибка, нет доступа).
- **Границы**:
    - **Входит**: Вид таблицы, форматы чисел, дат и статуса, открытие записи кликом по строке, состояния таблицы и
      повтор загрузки.
    - **Не входит**: Состав и заголовки столбцов (задаёт функциональность), сортировка ([SF-G-SORT][]), выделение
      ([SF-G-SELECT][]), настройка столбцов ([SF-G-COLUMNS][]), пагинация ([SF-G-PAG][]), «Ничего не найдено»
      ([SF-G-SEARCH][]).

### Состав требований {#sf-g-table-content .collapsed}

| Требование | Что описывает |
| :--- | :--- |
| [UI-G-TABLE-001][] | Таблица записей |
| [UI-G-TABLE-002][] | Состояния таблицы |

### Как подключить {#sf-g-table-usage .collapsed}

Функциональность указывает приставку `data-testid`, столбцы (заголовок, `data-field`, формат по таблице форматов
[UI-G-TABLE-001][]), что открывает клик по строке и каким ролям, а также объект в тексте «Нет доступа»
(«справочника», «реестра»).


[NFR-002]: <../nfr.md#nfr-002>
[NFR-004]: <../nfr.md#nfr-004>
[NFR-005]: <../nfr.md#nfr-005>
[design-system]: <../design-system/index.md>
[SF-G-TOAST]: <../sf-g-toast/index.md#sf-g-toast>
[SF-G-SESSION]: <../sf-g-session/index.md#sf-g-session>
[SF-G-SORT]: <../sf-g-sort/index.md#sf-g-sort>
[SF-G-SELECT]: <../sf-g-select/index.md#sf-g-select>
[SF-G-COLUMNS]: <../sf-g-columns/index.md#sf-g-columns>
[SF-G-PAG]: <../sf-g-pag/index.md#sf-g-pag>
[SF-G-SEARCH]: <../sf-g-search/index.md#sf-g-search>
[SF-PT-LIST]: <../../features/dict-product-type/sf-list/index.md#sf-pt-list>
[UI-G-TABLE-001]: <ui.md#ui-g-table-001>
[UI-G-TABLE-002]: <ui.md#ui-g-table-002>
