---
priority: "must"
status: "анализ"
icon: lucide/file-pen-line
order: 10
version: "0.00.01"
version_datetime: "21.11.2026 20:29:40"
editor: "Dmitry Khilko"
task_id:
release_id: 
release_date:
---

# ДЕТАЛЬНАЯ ФУНКЦИОНАЛЬНОСТЬ {#sf}

## Журнал изменений {#change-history .collapsed}

- [Версия 0.00.01 (21.11.2026 20:29:40; index.md)](https://github.com/DmitryKhilko/example-app-requirements-v2/commit/b9d11e1ba751a4f7d5596281dab33423f7c4627a){target="_blank" rel="noopener"}. Редактор: Dmitry Khilko

## SF-PT-DELETE. Удаление видов изделий {#sf-pt-delete .collapsed}

- **Статус**: анализ
- **Приоритет**: must
- **Стабильность**: низкая — не подтверждены неделимость удаления, определение использования записи и тексты ошибок
- **Права доступа**:
    - **Разрешено**: ais
    - **Запрещено**: pgipn, sgipn, igipn, pko, psh
- **Использует**: [F-PT][], [FR-PT-LIST-008][], [SF-G-SELECT][], [SF-G-CONFIRM][], [SF-G-TOAST][], [SF-G-SESSION][]
- **Используется в**: [UC-PT-009][], [FR-PT-DELETE-001][], [FR-PT-DELETE-002][], [FR-PT-DELETE-003][],
[AR-PT-DELETE-001][]
- **Описание**: Пользователь удаляет из справочника одну или несколько записей, внесённых ошибочно и нигде не
используемых, чтобы в справочнике не оставалось лишних видов изделий.
- **Границы**:
    - **Входит**: Физическое удаление записей, которые не используются в других сущностях; удаление нескольких
      записей одним запросом; подтверждение удаления в интерфейсе.
    - **Не входит**: Мягкое удаление и восстановление удалённых записей — их нет; выделение записей в списке
      ([FR-PT-LIST-008][]); скрытие используемой записи — это деактивация ([SF-PT-ACTIVATION][]).

### Состав требований {#sf-pt-delete-content .collapsed}

| Требование | Что описывает |
| :--- | :--- |
| [FR-PT-DELETE-001][] | Удаление записей (API) |
| [FR-PT-DELETE-002][] | Отказ в удалении записей (API) |
| [FR-PT-DELETE-003][] | Подтверждение удаления и результат на экране (UI) |
| [AR-PT-DELETE-001][] | Операция `POST /api/v1/product-types/batch-delete` |


[F-PT]: <../index.md#f-pt>
[SF-G-TOAST]: <../../../global/sf-g-toast/index.md#sf-g-toast>
[SF-PT-ACTIVATION]: <../sf-activation/index.md#sf-pt-activation>
[FR-PT-LIST-008]: <../sf-list/fr.md#fr-pt-list-008>
[UC-PT-009]: <../uc.md#uc-pt-009>
[FR-PT-DELETE-001]: <fr.md#fr-pt-delete-001>
[FR-PT-DELETE-002]: <fr.md#fr-pt-delete-002>
[FR-PT-DELETE-003]: <fr.md#fr-pt-delete-003>
[AR-PT-DELETE-001]: <fr.md#ar-pt-delete-001>
[SF-G-SELECT]: <../../../global/sf-g-select/index.md#sf-g-select>
[SF-G-CONFIRM]: <../../../global/sf-g-confirm/index.md#sf-g-confirm>
[SF-G-SESSION]: <../../../global/sf-g-session/index.md#sf-g-session>
