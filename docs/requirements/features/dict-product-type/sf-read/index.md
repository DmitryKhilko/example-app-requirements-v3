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

## SF-PT-READ. Получение вида изделий {#sf-pt-read .collapsed}

- **Статус**: анализ
- **Приоритет**: must
- **Стабильность**: высокая — простая операция чтения; открыт только вопрос об отдельном экране просмотра
  (`SF-PT-READ.H01`)
- **Права доступа**:
    - **Разрешено**: ais, pgipn, sgipn, igipn, pko, psh
    - **Запрещено**: пользователи без аутентификации
- **Использует**: [F-PT][], [SF-G-SESSION][]
- **Используется в**: [UC-PT-007][], [UC-PT-008][], [FR-PT-READ-001][], [FR-PT-READ-002][], [AR-PT-READ-001][],
[FR-PT-UPDATE-003][]
- **Описание**: Пользователь открывает запись справочника видов изделий, чтобы увидеть её актуальные данные перед
изменением; другие подсистемы получают запись по идентификатору для показа в документах.
- **Границы**:
    - **Входит**: Получение всех полей записи по идентификатору через API; загрузка данных записи в форму изменения.
    - **Не входит**: Отдельный экран просмотра записи (см. `H01`); изменение записи ([SF-PT-UPDATE][]).

### Состав требований {#sf-pt-read-content .collapsed}

| Требование | Что описывает |
| :--- | :--- |
| [FR-PT-READ-001][] | Получение записи по идентификатору (API) |
| [FR-PT-READ-002][] | Отказ в получении записи (API) |
| [AR-PT-READ-001][] | Операция `GET /api/v1/product-types/{pk}` |

Состав полей записи — как у записи списка в [DR-PT-LIST-001][].

### Допущения {#sf-pt-read-assumptions .collapsed}

- **SF-PT-READ.H01**
    - **Статус**: требует подтверждения
    - **Подтверждает**: владелец справочника
    - **Допущение**: Отдельного экрана просмотра записи нет: все поля видны в таблице списка, а роль `ais` открывает
      запись в форме изменения ([FR-PT-UPDATE-003][]), которая получает данные операцией [AR-PT-READ-001][].


[F-PT]: <../index.md#f-pt>
[UC-PT-007]: <../uc.md#uc-pt-007>
[UC-PT-008]: <../uc.md#uc-pt-008>
[SF-PT-UPDATE]: <../sf-update/index.md#sf-pt-update>
[DR-PT-LIST-001]: <../sf-list/dr.md#dr-pt-list-001>
[FR-PT-READ-001]: <fr.md#fr-pt-read-001>
[FR-PT-READ-002]: <fr.md#fr-pt-read-002>
[AR-PT-READ-001]: <fr.md#ar-pt-read-001>
[FR-PT-UPDATE-003]: <../sf-update/fr.md#fr-pt-update-003>
[SF-G-SESSION]: <../../../global/sf-g-session/index.md#sf-g-session>
