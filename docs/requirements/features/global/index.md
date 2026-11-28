# Реестр глобальных требований {#registry-global}

Описание требований к глобальным функциональностям, которые используются в бизнес-функциональностях программного
продукта, и требований, которые относятся ко всему продукту.

| Раздел | Требования | Что описывает |
| :--- | :--- | :--- |
| [Требования к API](ar.md) | [AR-001](ar.md#ar-001) | Форматы, порядок проверок, коды ошибок, эталоны 401, 403, 500 |
| [Нефункциональные требования](nfr.md) | [NFR-001](nfr.md#nfr-001) | Условия проверки производительности |
| | [NFR-002](nfr.md#nfr-002) | Доступность интерфейса (WCAG 2.1 AA) |
| | [NFR-003](nfr.md#nfr-003) | Журнал аудита |
| | [NFR-004](nfr.md#nfr-004) | Дата, время и часовой пояс |
| | [NFR-005](nfr.md#nfr-005) | Атрибуты `data-testid` для автотестов |
| [Системные требования](sr.md) | [SR-001](sr.md#sr-001) | Браузеры и экран рабочего места |
| | [SR-002](sr.md#sr-002) | Технический стандарт: стек, слои, ошибки, база данных, временная аутентификация |
| [Дизайн-система](design-system/index.md) | — | Бренд, токены, компоненты, паттерны экранов |
| [Пагинация](sf-g-pag/index.md) | [FR-G-PAG-001](sf-g-pag/fr.md#fr-g-pag-001) | Постраничная выдача списка (API) |
| | [UI-G-PAG-001](sf-g-pag/ui.md#ui-g-pag-001) | Панель пагинации |
| [Сортировка](sf-g-sort/index.md) | [FR-G-SORT-001](sf-g-sort/fr.md#fr-g-sort-001) | Сортировка списка (API) |
| | [UI-G-SORT-001](sf-g-sort/ui.md#ui-g-sort-001) | Сортировка по заголовку столбца |
| [Поиск](sf-g-search/index.md) | [FR-G-SEARCH-001](sf-g-search/fr.md#fr-g-search-001) | Поиск по вхождению (API) |
| | [UI-G-SEARCH-001](sf-g-search/ui.md#ui-g-search-001) | Поле поиска и «Ничего не найдено» |
| [Фильтрация](sf-g-filter/index.md) | [FR-G-FILTER-001](sf-g-filter/fr.md#fr-g-filter-001) | Фильтрация списка (API) |
| | [UI-G-FILTER-001](sf-g-filter/ui.md#ui-g-filter-001) | Кнопка и панель фильтров |
| | [UI-G-FILTER-002](sf-g-filter/ui.md#ui-g-filter-002) | Чипы применённых фильтров |
| [Уведомления](sf-g-toast/index.md) | [UI-G-TOAST-001](sf-g-toast/ui.md#ui-g-toast-001) | «Готово» и «Ошибка» |
| [Экран](sf-g-dict/index.md) | [UI-G-DICT-001](sf-g-dict/ui.md#ui-g-dict-001) | Раскладка и чек-лист |
| [Каталог](sf-g-catalog/index.md) | [UI-G-CATALOG-001](sf-g-catalog/ui.md#ui-g-catalog-001) | Группы, поиск |
| [Таблица списка](sf-g-table/index.md) | [UI-G-TABLE-001](sf-g-table/ui.md#ui-g-table-001) | Таблица, форматы |
| | [UI-G-TABLE-002](sf-g-table/ui.md#ui-g-table-002) | Загрузка, пусто, ошибка, нет доступа |
| [Столбцы](sf-g-columns/index.md) | [UI-G-COLUMNS-001](sf-g-columns/ui.md#ui-g-columns-001) | Видимость столбцов |
| [Выделение](sf-g-select/index.md) | [UI-G-SELECT-001](sf-g-select/ui.md#ui-g-select-001) | Флажки и панель выделения |
| [Подтверждение](sf-g-confirm/index.md) | [UI-G-CONFIRM-001](sf-g-confirm/ui.md#ui-g-confirm-001) | Окно |
| [Форма записи](sf-g-form/index.md) | [UI-G-FORM-001](sf-g-form/ui.md#ui-g-form-001) | Модальная форма |
| [Блокировка](sf-g-lock/index.md) | [FR-G-LOCK-001](sf-g-lock/fr.md#fr-g-lock-001) | Проверка версии записи (API) |
| | [UI-G-LOCK-001](sf-g-lock/ui.md#ui-g-lock-001) | Форма при одновременном изменении |
| [Сессия](sf-g-session/index.md) | [UI-G-SESSION-001](sf-g-session/ui.md#ui-g-session-001) | Ответ 401 |

Общий эталон отказа `409 RECORD_MODIFIED` — `api/error.409.modified.json`. Общие определения параметров и ответа
списков (`page`, `page_size`, `search`, `sort_order`, `page_envelope`) — в
`api/list.schema.json`.
