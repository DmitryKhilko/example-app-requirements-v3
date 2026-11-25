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

## SF-G-FORM. Модальная форма записи {#sf-g-form .collapsed}

- **Статус**: анализ
- **Приоритет**: must
- **Стабильность**: средняя — открыт вопрос о подтверждении закрытия формы с изменёнными данными
  (`UI-G-FORM-001.Q01`)
- **Права доступа**: определяют операции создания и изменения, которые подключают форму
- **Использует**: [AR-001][], [SF-G-TOAST][], [SF-G-SESSION][], [SF-G-LOCK][], [NFR-002][], [NFR-005][],
[дизайн-система][design-system] (Modal, TextInput, Select, NumberInput, Switch, Button)
- **Используется в**: [F-PT][] ([UI-PT-001][]), [SF-PT-CREATE][], [SF-PT-UPDATE][]
- **Описание**: Единое модальное окно для создания и изменения записи: вид окна, поля, проверка на клиенте, ошибки,
кнопки, отправка, закрытие и общие ответы API.
- **Границы**:
    - **Входит**: Окно и режимы, раскладка и виды полей, обязательность, ошибки полей, «Отмена» и «Сохранить»,
      состояние отправки, фокус и закрытие, общие ответы (`400`, `403`, `401`, `500`), успех.
    - **Не входит**: Состав полей, проверки и их тексты, особые отказы (`409` уникальности) и тексты уведомлений —
      задаёт функциональность; одновременное изменение — [SF-G-LOCK][].

### Состав требований {#sf-g-form-content .collapsed}

| Требование | Что описывает |
| :--- | :--- |
| [UI-G-FORM-001][] | Модальная форма записи |

### Как подключить {#sf-g-form-usage .collapsed}

Функциональность описывает форму требованием UI уровня основной функциональности: приставка `data-testid`,
таблица режимов (заголовок, как открывается, значения при открытии, запрос, уведомление об успехе), поля
(подпись, `data-testid`, `data-field`, компонент, плейсхолдер, шаг стрелок), проверки с текстами под полями и особые
отказы.


[AR-001]: <../ar.md#ar-001>
[NFR-002]: <../nfr.md#nfr-002>
[NFR-005]: <../nfr.md#nfr-005>
[design-system]: <../design-system/index.md>
[SF-G-TOAST]: <../sf-g-toast/index.md#sf-g-toast>
[SF-G-SESSION]: <../sf-g-session/index.md#sf-g-session>
[SF-G-LOCK]: <../sf-g-lock/index.md#sf-g-lock>
[F-PT]: <../../features/dict-product-type/index.md#f-pt>
[UI-PT-001]: <../../features/dict-product-type/ui.md#ui-pt-001>
[SF-PT-CREATE]: <../../features/dict-product-type/sf-create/index.md#sf-pt-create>
[SF-PT-UPDATE]: <../../features/dict-product-type/sf-update/index.md#sf-pt-update>
[UI-G-FORM-001]: <ui.md#ui-g-form-001>
