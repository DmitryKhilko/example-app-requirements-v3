---
priority: "must"
status: "анализ"
icon: lucide/file-pen-line
order: 10
version: "0.00.02"
version_datetime: "24.11.2026 21:37:58"
editor: "Dmitry Khilko"
task_id:
release_id: 
release_date: 
---

# ДЕТАЛЬНАЯ ФУНКЦИОНАЛЬНОСТЬ {#sf}

## Журнал изменений {#change-history .collapsed}

- [Версия 0.00.02 (24.11.2026 21:37:58; api/AR-PT-LIST-001.fixture.json, api/AR-PT-LIST-001.request.invalid.json, api/AR-PT-LIST-001.request.json, api/AR-PT-LIST-001.request.not-found.json, api/AR-PT-LIST-001.request.schema.json, api/AR-PT-LIST-001.response.200.empty.json, api/AR-PT-LIST-001.response.200.json, api/AR-PT-LIST-001.response.200.schema.json, api/AR-PT-LIST-001.response.400.json, api/AR-PT-LIST-001.response.401.json, api/AR-PT-LIST-001.response.403.json, api/AR-PT-LIST-001.response.500.json, dr.md, fr.md, index.md)](https://github.com/DmitryKhilko/example-app-requirements-v2/commit/8ee0213ea8c2b02b0ec3e55b1b022cf4773562d3){target="_blank" rel="noopener"}. Редактор: Dmitry Khilko
- [Версия 0.00.01 (21.11.2026 20:29:40; index.md)](https://github.com/DmitryKhilko/example-app-requirements-v2/commit/b9d11e1ba751a4f7d5596281dab33423f7c4627a){target="_blank" rel="noopener"}. Редактор: Dmitry Khilko

## SF-PT-LIST. Список видов изделий {#sf-pt-list .collapsed}

- **Статус**: анализ
- **Приоритет**: must
- **Стабильность**: высокая — 2 допущения списка ждут подтверждения (аудит чтения, подпись фильтра); поведение экрана
  — в глобальных функциональностях
- **Права доступа**:
    - **Разрешено**: ais, pgipn, sgipn, igipn, pko, psh — просмотр списка (справочник используется в документах всех
      подсистем)
    - **Запрещено**: пользователи без аутентификации
    - **Действия над записями**: кнопки создания, изменения и удаления видит только роль `ais` (права заданы в
      [SF-PT-CREATE][], [SF-PT-UPDATE][], [SF-PT-DELETE][])
- **Использует**: [F-PT][], [SF-G-DICT][], [SF-G-CATALOG][], [SF-G-TABLE][], [SF-G-PAG][], [SF-G-SORT][],
[SF-G-SEARCH][], [SF-G-FILTER][], [SF-G-COLUMNS][], [SF-G-SELECT][], [SF-G-TOAST][], [SF-G-SESSION][],
[Дизайн-система][design-system]
- **Используется в**: [UC-PT-001][], [UC-PT-002][], [UC-PT-003][], [UC-PT-004][], [UC-PT-005][], [UC-PT-009][],
[DR-PT-LIST-001][], [FR-PT-LIST-001][], [FR-PT-LIST-002][], [FR-PT-LIST-003][], [FR-PT-LIST-004][],
[FR-PT-LIST-005][], [FR-PT-LIST-006][], [FR-PT-LIST-007][], [FR-PT-LIST-008][], [FR-PT-LIST-009][],
[AR-PT-LIST-001][]
- **Описание**: Пользователь просматривает справочник видов изделий постранично, ищет записи по наименованию,
фильтрует, сортирует и настраивает состав столбцов, чтобы оценить актуальность справочника и выбрать запись для
изменения или удаления.
- **Границы**:
    - **Входит**: Получение страницы записей и общего количества, поиск, фильтрация, сортировка, экран списка,
      настройка видимости столбцов, выделение записей.
    - **Не входит**: Создание ([SF-PT-CREATE][]), изменение ([SF-PT-UPDATE][]), смена статуса
      ([SF-PT-ACTIVATION][]) и удаление ([SF-PT-DELETE][]) записей: список только открывает эти операции.

### Состав требований {#sf-pt-list-content .collapsed}

| Требование | Что описывает |
| :--- | :--- |
| [DR-PT-LIST-001][] | Поля списка, поиск, сортировка и фильтры по полям, порядок по умолчанию, индексы |
| [FR-PT-LIST-001][] | Получение страницы списка и общего количества записей (API) |
| [FR-PT-LIST-002][] | Поиск по наименованию (API) |
| [FR-PT-LIST-009][] | Фильтрация (API) |
| [FR-PT-LIST-003][] | Сортировка (API) |
| [FR-PT-LIST-004][] | Отказ в получении списка (API) |
| [FR-PT-LIST-005][] | Экран списка: переход, заголовок, таблица, состояния (UI) |
| [FR-PT-LIST-006][] | Поле поиска и поля фильтра справочника (UI) |
| [FR-PT-LIST-007][] | Сортировка и настройка столбцов на экране (UI) |
| [FR-PT-LIST-008][] | Выделение записей на экране (UI) |
| [AR-PT-LIST-001][] | Операция `GET /api/v1/product-types` |


[F-PT]: <../index.md#f-pt>
[SF-G-TOAST]: <../../../global/sf-g-toast/index.md#sf-g-toast>
[design-system]: <../../../global/design-system/index.md>
[UC-PT-001]: <../uc.md#uc-pt-001>
[UC-PT-002]: <../uc.md#uc-pt-002>
[UC-PT-003]: <../uc.md#uc-pt-003>
[UC-PT-004]: <../uc.md#uc-pt-004>
[UC-PT-005]: <../uc.md#uc-pt-005>
[UC-PT-009]: <../uc.md#uc-pt-009>
[SF-PT-CREATE]: <../sf-create/index.md#sf-pt-create>
[SF-PT-UPDATE]: <../sf-update/index.md#sf-pt-update>
[SF-PT-ACTIVATION]: <../sf-activation/index.md#sf-pt-activation>
[SF-PT-DELETE]: <../sf-delete/index.md#sf-pt-delete>
[DR-PT-LIST-001]: <dr.md#dr-pt-list-001>
[FR-PT-LIST-001]: <fr.md#fr-pt-list-001>
[FR-PT-LIST-002]: <fr.md#fr-pt-list-002>
[FR-PT-LIST-003]: <fr.md#fr-pt-list-003>
[FR-PT-LIST-004]: <fr.md#fr-pt-list-004>
[FR-PT-LIST-005]: <fr.md#fr-pt-list-005>
[FR-PT-LIST-006]: <fr.md#fr-pt-list-006>
[FR-PT-LIST-007]: <fr.md#fr-pt-list-007>
[FR-PT-LIST-008]: <fr.md#fr-pt-list-008>
[FR-PT-LIST-009]: <fr.md#fr-pt-list-009>
[AR-PT-LIST-001]: <fr.md#ar-pt-list-001>
[SF-G-PAG]: <../../../global/sf-g-pag/index.md#sf-g-pag>
[SF-G-SORT]: <../../../global/sf-g-sort/index.md#sf-g-sort>
[SF-G-SEARCH]: <../../../global/sf-g-search/index.md#sf-g-search>
[SF-G-FILTER]: <../../../global/sf-g-filter/index.md#sf-g-filter>
[SF-G-DICT]: <../../../global/sf-g-dict/index.md#sf-g-dict>
[SF-G-CATALOG]: <../../../global/sf-g-catalog/index.md#sf-g-catalog>
[SF-G-TABLE]: <../../../global/sf-g-table/index.md#sf-g-table>
[SF-G-COLUMNS]: <../../../global/sf-g-columns/index.md#sf-g-columns>
[SF-G-SELECT]: <../../../global/sf-g-select/index.md#sf-g-select>
[SF-G-SESSION]: <../../../global/sf-g-session/index.md#sf-g-session>
