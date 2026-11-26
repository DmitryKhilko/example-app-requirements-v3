---
icon: lucide/file-pen-line
---

# ТРЕБОВАНИЯ К API {#ar}

## AR-PT-001. API справочника видов изделий {#ar-pt-001 .collapsed}

- **Использует**: [AR-001][], [DR-PT-001][]
- **Используется в**: [AR-PT-LIST-001][], [AR-PT-READ-001][], [AR-PT-CREATE-001][], [AR-PT-UPDATE-001][],
[AR-PT-DELETE-001][]
- **Описание**: Общие правила операций справочника видов изделий: ресурс, перечень операций, права и единое
представление записи в ответах. Общие для продукта правила (форматы, порядок проверок, коды ошибок, эталоны `401`,
`403`, `500`) заданы в [AR-001][]; операции описывают только своё.

### Операции {#ar-pt-001-operations .collapsed}

Ресурс — `/api/v1/product-types`.

| Операция | Метод и путь | Роли | Требование |
| :--- | :--- | :--- | :--- |
| Список | `GET /api/v1/product-types` | Все роли | [AR-PT-LIST-001][] |
| Запись | `GET /api/v1/product-types/{pk}` | Все роли | [AR-PT-READ-001][] |
| Создание | `POST /api/v1/product-types` | `ais` | [AR-PT-CREATE-001][] |
| Изменение и смена статуса | `PUT /api/v1/product-types/{pk}` | `ais` | [AR-PT-UPDATE-001][] |
| Удаление | `POST /api/v1/product-types/batch-delete` | `ais` | [AR-PT-DELETE-001][] |

Права подробно — в [матрице прав][access] справочника.

### Представление записи {#ar-pt-001-record .collapsed}

Все операции, которые возвращают запись справочника (запись, создание, изменение, элементы страницы списка),
возвращают её в одном виде: все поля [DR-PT-001][] — `pk`, `name_nominative`, `product_group`,
`default_streak_count`, `wholesale_gold_streak_count`, `stamp_impressions_count`, `is_active`, `created_at`,
`updated_at`. Схема записи — файл `api/AR-PT-001.product-type.schema.json`; схемы ответов операций ссылаются на неё
и не повторяют её поля.

В разделе `$defs` этой схемы каждое поле записи определено один раз: тип, допустимые значения и границы. Схемы
запросов создания, изменения и фильтров списка ссылаются на эти определения (`$ref`), поэтому перечень типов изделий
и границы чисел меняются в одном месте.

```json
--8<-- "requirements/features/dict-product-type/api/AR-PT-001.product-type.schema.json"
```

### Критерии приёмки (AC) {#ar-pt-001-ac .collapsed}

```gherkin
# language: ru
@AR-PT-001
Функционал: Единое представление записи

  Предыстория:
    Дано в справочнике записи из файла "PT.fixture.json"
    И аутентифицированный пользователь с ролью "ais"

  Структура сценария: Запись в ответе соответствует общей схеме
    Когда он выполняет операцию "<операция>" с корректными данными
    Тогда каждая запись справочника в ответе соответствует схеме "AR-PT-001.product-type.schema.json"

    Примеры:
      | операция                       |
      | GET /api/v1/product-types      |
      | GET /api/v1/product-types/{pk} |
      | POST /api/v1/product-types     |
      | PUT /api/v1/product-types/{pk} |
```


[AR-001]: <../global/ar.md#ar-001>
[DR-PT-001]: <dr.md#dr-pt-001>
[access]: <index.md#f-pt-access>
[AR-PT-LIST-001]: <sf-list/fr.md#ar-pt-list-001>
[AR-PT-READ-001]: <sf-read/fr.md#ar-pt-read-001>
[AR-PT-CREATE-001]: <sf-create/fr.md#ar-pt-create-001>
[AR-PT-UPDATE-001]: <sf-update/fr.md#ar-pt-update-001>
[AR-PT-DELETE-001]: <sf-delete/fr.md#ar-pt-delete-001>

