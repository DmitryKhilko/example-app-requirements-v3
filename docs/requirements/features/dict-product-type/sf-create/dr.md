# ТРЕБОВАНИЯ К ДАННЫМ {#dr}

## DR-PT-CREATE-001. Данные для создания вида изделий {#dr-pt-create-001 .collapsed}

- **Использует**: [F-PT][], [DR-PT-001][]
- **Используется в**: [SF-PT-CREATE][], [FR-PT-CREATE-001][], [FR-PT-CREATE-002][],
[FR-PT-CREATE-003][], [AR-PT-CREATE-001][]
- **Описание**: Какие поля записи справочника видов изделий передаёт пользователь при создании и какие заполняет
система. Типы, ограничения, допустимые значения и уникальность полей заданы в [DR-PT-001][].

### Данные, которые передаёт пользователь {#dr-pt-create-001-input .collapsed}

| Поле | Обязательно | Если не передано |
| :--- | :--- | :--- |
| `name_nominative` | Да | Отказ ([FR-PT-CREATE-002][]) |
| `product_group` | Да | Отказ |
| `default_streak_count` | Да | Отказ |
| `wholesale_gold_streak_count` | Да | Отказ |
| `stamp_impressions_count` | Да | Отказ |
| `is_active` | Нет | Запись создаётся действующей (`true`) |

Пробелы по краям `name_nominative` система обрезает до проверки ограничений.

### Данные, которые заполняет система {#dr-pt-create-001-system .collapsed}

| Поле | Значение при создании |
| :--- | :--- |
| `pk` | Новый уникальный идентификатор |
| `is_active` | Значение из запроса; если не передано — `true` |
| `created_at` | Дата и время создания (UTC, до секунды) |
| `updated_at` | Равно `created_at` (допущение `FR-PT-CREATE-001.H01`) |


[F-PT]: <../index.md#f-pt>
[DR-PT-001]: <../dr.md#dr-pt-001>
[SF-PT-CREATE]: <index.md#sf-pt-create>
[FR-PT-CREATE-001]: <fr.md#fr-pt-create-001>
[FR-PT-CREATE-002]: <fr.md#fr-pt-create-002>
[FR-PT-CREATE-003]: <fr.md#fr-pt-create-003>
[AR-PT-CREATE-001]: <fr.md#ar-pt-create-001>
