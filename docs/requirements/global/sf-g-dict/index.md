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

Записей пока нет.

## SF-G-DICT. Типовой экран справочника {#sf-g-dict .collapsed}

- **Статус**: анализ
- **Приоритет**: must
- **Стабильность**: средняя — собирается из глобальных функциональностей; адрес экрана не подтверждён
  (`UI-G-DICT-001.H01`)
- **Права доступа**: задаёт справочник: роли просмотра, создания, изменения и удаления
- **Использует**: [SF-G-CATALOG][], [SF-G-TABLE][], [SF-G-PAG][], [SF-G-SORT][], [SF-G-SEARCH][], [SF-G-FILTER][],
[SF-G-COLUMNS][], [SF-G-SELECT][], [SF-G-CONFIRM][], [SF-G-FORM][], [SF-G-LOCK][], [SF-G-TOAST][],
[SF-G-SESSION][], [дизайн-система][design-system] (PageHeader, Toolbar)
- **Используется в**: [F-PT][]
- **Описание**: Шаблон экрана справочника: раскладка экрана, заголовок, панель инструментов и перечень того, что
справочник должен определить сам. Новый справочник описывает поля, права и тексты, а поведение экрана берёт из
шаблона.
- **Границы**:
    - **Входит**: Адрес и раскладка экрана, заголовок страницы, панель инструментов, кнопка создания, порядок
      блоков, чек-лист требований справочника.
    - **Не входит**: Поведение отдельных блоков — оно в подключаемых глобальных функциональностях; справочники
      с иерархией и вложенными записями.

### Состав требований {#sf-g-dict-content .collapsed}

| Требование | Что описывает |
| :--- | :--- |
| [UI-G-DICT-001][] | Экран справочника |

### Как подключить {#sf-g-dict-usage .collapsed}

Справочник заполняет чек-лист [UI-G-DICT-001][] (раздел «Что задаёт справочник») и описывает только отклонения от
шаблона. Эталон — справочник видов изделий ([F-PT][]).


[design-system]: <../design-system/index.md>
[SF-G-CATALOG]: <../sf-g-catalog/index.md#sf-g-catalog>
[SF-G-TABLE]: <../sf-g-table/index.md#sf-g-table>
[SF-G-PAG]: <../sf-g-pag/index.md#sf-g-pag>
[SF-G-SORT]: <../sf-g-sort/index.md#sf-g-sort>
[SF-G-SEARCH]: <../sf-g-search/index.md#sf-g-search>
[SF-G-FILTER]: <../sf-g-filter/index.md#sf-g-filter>
[SF-G-COLUMNS]: <../sf-g-columns/index.md#sf-g-columns>
[SF-G-SELECT]: <../sf-g-select/index.md#sf-g-select>
[SF-G-CONFIRM]: <../sf-g-confirm/index.md#sf-g-confirm>
[SF-G-FORM]: <../sf-g-form/index.md#sf-g-form>
[SF-G-LOCK]: <../sf-g-lock/index.md#sf-g-lock>
[SF-G-TOAST]: <../sf-g-toast/index.md#sf-g-toast>
[SF-G-SESSION]: <../sf-g-session/index.md#sf-g-session>
[F-PT]: <../../features/dict-product-type/index.md#f-pt>
[UI-G-DICT-001]: <ui.md#ui-g-dict-001>
