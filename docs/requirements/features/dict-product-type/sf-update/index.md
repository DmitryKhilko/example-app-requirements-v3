---
priority: "must"
status: "анализ"
icon: lucide/file-pen-line
order: 10
version: "0.00.00"
version_datetime: ""
editor: "Dmitry Khilko"
task_id:
release_id: 
release_date:
---

# ДЕТАЛЬНАЯ ФУНКЦИОНАЛЬНОСТЬ {#sf}

## Журнал изменений {#change-history .collapsed}

- Записей пока нет.

## SF-PT-UPDATE. Изменение вида изделий {#sf-pt-update .collapsed}

- **Статус**: анализ
- **Приоритет**: must
- **Стабильность**: средняя — проверка одновременного изменения (`DR-PT-001.H01`, [SF-G-LOCK][]) ждёт подтверждения
- **Права доступа**:
    - **Разрешено**: ais
    - **Запрещено**: pgipn, sgipn, igipn, pko, psh
- **Использует**: [F-PT][], [UI-PT-001][], [SF-PT-READ][], [SF-G-FORM][], [SF-G-LOCK][], [SF-G-TOAST][],
[SF-G-SESSION][]
- **Используется в**: [UC-PT-007][], [UC-PT-008][], [DR-PT-UPDATE-001][], [FR-PT-UPDATE-001][], [FR-PT-UPDATE-002][],
[FR-PT-UPDATE-003][], [AR-PT-UPDATE-001][]
- **Описание**: Пользователь исправляет данные существующего вида изделий, чтобы справочник оставался достоверным
для документов всех подсистем.
- **Границы**:
    - **Входит**: Изменение наименования, типа, количества натиров и оттисков и статуса записи одним запросом; форма
      изменения; проверка, что запись не изменили другие пользователи.
    - **Не входит**: Правила смены статуса ([SF-PT-ACTIVATION][]): статус передаётся тем же запросом, но его
      последствия описаны там.

### Состав требований {#sf-pt-update-content .collapsed}

| Требование | Что описывает |
| :--- | :--- |
| [DR-PT-UPDATE-001][] | Данные запроса изменения, проверка версии записи |
| [FR-PT-UPDATE-001][] | Изменение записи (API) |
| [FR-PT-UPDATE-002][] | Отказ в изменении записи (API) |
| [FR-PT-UPDATE-003][] | Форма изменения: особенности режима формы [UI-PT-001][] |
| [AR-PT-UPDATE-001][] | Операция `PUT /api/v1/product-types/{pk}` |


[F-PT]: <../index.md#f-pt>
[UI-PT-001]: <../ui.md#ui-pt-001>
[SF-PT-READ]: <../sf-read/index.md#sf-pt-read>
[SF-PT-ACTIVATION]: <../sf-activation/index.md#sf-pt-activation>
[SF-G-TOAST]: <../../global/sf-g-toast/index.md#sf-g-toast>
[UC-PT-007]: <../uc.md#uc-pt-007>
[UC-PT-008]: <../uc.md#uc-pt-008>
[DR-PT-UPDATE-001]: <dr.md#dr-pt-update-001>
[FR-PT-UPDATE-001]: <fr.md#fr-pt-update-001>
[FR-PT-UPDATE-002]: <fr.md#fr-pt-update-002>
[FR-PT-UPDATE-003]: <fr.md#fr-pt-update-003>
[AR-PT-UPDATE-001]: <fr.md#ar-pt-update-001>
[SF-G-FORM]: <../../global/sf-g-form/index.md#sf-g-form>
[SF-G-LOCK]: <../../global/sf-g-lock/index.md#sf-g-lock>
[SF-G-SESSION]: <../../global/sf-g-session/index.md#sf-g-session>
