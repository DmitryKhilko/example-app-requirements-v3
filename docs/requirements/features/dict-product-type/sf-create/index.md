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

## SF-PT-CREATE. Создание вида изделий {#sf-pt-create .collapsed}

- **Статус**: анализ
- **Приоритет**: must
- **Стабильность**: высокая — данные и форма согласованы; открыт общий для форм вопрос `UI-G-FORM-001.Q01`
- **Права доступа**:
    - **Разрешено**: ais
    - **Запрещено**: pgipn, sgipn, igipn, pko, psh
- **Использует**: [F-PT][], [SF-G-FORM][], [SF-G-TOAST][], [SF-G-SESSION][], [Дизайн-система][design-system]
- **Используется в**: [UC-PT-006][], [DR-PT-CREATE-001][], [FR-PT-CREATE-001][], [FR-PT-CREATE-002][],
[FR-PT-CREATE-003][], [AR-PT-CREATE-001][]
- **Описание**: Пользователь добавляет в справочник новый вид изделий из драгоценных металлов, чтобы он стал доступен
для выбора в заявлениях на проведение пробирных работ и отображения в иных документах.
- **Границы**:
    - **Входит**: Создание записи через API, форма создания (режим формы [UI-PT-001][]), выбор статуса при создании.
    - **Не входит**: Изменение и удаление записей ([SF-PT-UPDATE][], [SF-PT-DELETE][]); загрузка записей из файла и
      внешних классификаторов ([F-PT][]).

### Состав требований {#sf-pt-create-content .collapsed}

| Требование | Что описывает |
| :--- | :--- |
| [DR-PT-CREATE-001][] | Поля, которые передаёт пользователь и заполняет система |
| [FR-PT-CREATE-001][] | Создание записи (API) |
| [FR-PT-CREATE-002][] | Отказ в создании записи (API) |
| [FR-PT-CREATE-003][] | Форма создания: особенности режима формы [UI-PT-001][] |
| [AR-PT-CREATE-001][] | Операция `POST /api/v1/product-types` |


[F-PT]: <../index.md#f-pt>
[DR-PT-CREATE-001]: <dr.md#dr-pt-create-001>
[FR-PT-CREATE-001]: <fr.md#fr-pt-create-001>
[FR-PT-CREATE-002]: <fr.md#fr-pt-create-002>
[FR-PT-CREATE-003]: <fr.md#fr-pt-create-003>
[AR-PT-CREATE-001]: <fr.md#ar-pt-create-001>
[SF-G-TOAST]: <../../../global/sf-g-toast/index.md#sf-g-toast>
[design-system]: <../../../global/design-system/index.md>
[UC-PT-006]: <../uc.md#uc-pt-006>
[UI-PT-001]: <../ui.md#ui-pt-001>
[SF-PT-UPDATE]: <../sf-update/index.md#sf-pt-update>
[SF-PT-DELETE]: <../sf-delete/index.md#sf-pt-delete>
[SF-G-FORM]: <../../../global/sf-g-form/index.md#sf-g-form>
[SF-G-SESSION]: <../../../global/sf-g-session/index.md#sf-g-session>
