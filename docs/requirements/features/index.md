# Требования к программному продукту {#registry}

<!-- BEGIN GENERATED DASHBOARD — не редактируйте вручную -->

<details class="info dash-info" markdown>
<summary>Статусы функциональностей</summary>

- :lucide-file: бэклог: зафиксированное сырое требование или идея
- :lucide-file-pen-line: анализ: детализация и согласование требования
- :lucide-file-check: готово к разработке: утверждённое требование, готовое к реализации
- :lucide-file-braces: разработка: требование в работе у команды разработки и тестирования
- :lucide-file-text: реализовано: код, связанный с требованием, успешно развёрнут на проде
- :lucide-file-archive: архив: отклонённое или устаревшее требование
- :lucide-file-clock: в работе: только у F: часть её SF уже в работе, но реализованы ещё не все

</details>

## Прогресс по F {#dash-progress}

Доля SF, включенных в F, в каждом статусе; SF в архиве не учитываются.

<div class="dash-progress" markdown="block"><div class="dash-progress__row" markdown="block"><div class="dash-progress__title" markdown="span">[Справочник видов изделий](dict-product-type/index.md#f-pt)<small>в работе · 6 SF</small></div><div class="dash-bar"><span class="dash-analysis" style="width:100%" title="анализ: 6"></span></div><div class="dash-progress__done">реализовано <b>0 из 6</b></div></div></div>

<div class="dash-legend"><span class="dash-backlog"><i></i>бэклог</span><span class="dash-analysis"><i></i>анализ</span><span class="dash-ready"><i></i>готово к разработке</span><span class="dash-development"><i></i>разработка</span><span class="dash-released"><i></i>реализовано</span></div>

## Приоритет × статус SF {#dash-priority}

Число SF каждого приоритета в каждом статусе.

<table class="dash-matrix"><thead><tr><th>Приоритет</th><th class="dash-backlog"><i></i>бэклог</th><th class="dash-analysis"><i></i>анализ</th><th class="dash-ready"><i></i>готово к разработке</th><th class="dash-development"><i></i>разработка</th><th class="dash-released"><i></i>реализовано</th><th class="dash-archived"><i></i>архив</th><th>Всего</th></tr></thead><tbody><tr><th>must</th><td class="is-empty">—</td><td class="dash-analysis is-value">6</td><td class="is-empty">—</td><td class="is-empty">—</td><td class="is-empty">—</td><td class="is-empty">—</td><td><b>6</b></td></tr><tr><th>should</th><td class="is-empty">—</td><td class="is-empty">—</td><td class="is-empty">—</td><td class="is-empty">—</td><td class="is-empty">—</td><td class="is-empty">—</td><td><b>0</b></td></tr><tr><th>could</th><td class="is-empty">—</td><td class="is-empty">—</td><td class="is-empty">—</td><td class="is-empty">—</td><td class="is-empty">—</td><td class="is-empty">—</td><td><b>0</b></td></tr><tr><th>won&#x27;t</th><td class="is-empty">—</td><td class="is-empty">—</td><td class="is-empty">—</td><td class="is-empty">—</td><td class="is-empty">—</td><td class="is-empty">—</td><td><b>0</b></td></tr><tr class="dash-sum"><th>Всего</th><td>0</td><td>6</td><td>0</td><td>0</td><td>0</td><td>0</td><td>6</td></tr></tbody></table>

## Требует внимания {#dash-attention}

Групп с замечаниями: 1, замечаний: 41.

<details class="success dash-check"><summary>SF без функциональных требований (FR)<span class="dash-ok">Замечаний нет</span></summary></details>

<details class="success dash-check"><summary>FR без критериев приёмки<span class="dash-ok">Замечаний нет</span></summary></details>

<details class="success dash-check"><summary>SF без приоритета<span class="dash-ok">Замечаний нет</span></summary></details>

<details class="success dash-check"><summary>Повторяющиеся коды<span class="dash-ok">Замечаний нет</span></summary></details>

<details class="warning dash-check" open markdown>
<summary>Неподтверждённые вопросы и допущения<span class="dash-count">41</span></summary>

- [`DR-PT-001.Q01`](dict-product-type/dr.md#dr-pt-001-questions) — вопрос, статус «открыт», решает: владелец справочника (Справочник видов изделий (dr.md))
- [`DR-PT-001.H01`](dict-product-type/dr.md#dr-pt-001-assumptions) — допущение, статус «требует подтверждения», подтверждает: архитектор (Справочник видов изделий (dr.md))
- [`DR-PT-001.H02`](dict-product-type/dr.md#dr-pt-001-assumptions) — допущение, статус «требует подтверждения», подтверждает: архитектор (Справочник видов изделий (dr.md))
- [`FR-PT-ACTIVATION-001.H01`](dict-product-type/sf-activation/fr.md#fr-pt-activation-001-assumptions) — допущение, статус «требует подтверждения», подтверждает: владелец справочника (Справочник видов изделий → Активация (fr.md))
- [`FR-PT-ACTIVATION-002.H01`](dict-product-type/sf-activation/fr.md#fr-pt-activation-002-assumptions) — допущение, статус «требует подтверждения», подтверждает: владелец справочника (Справочник видов изделий → Активация (fr.md))
- [`SF-PT-ACTIVATION.H01`](dict-product-type/sf-activation/index.md#sf-pt-activation-assumptions) — допущение, статус «требует подтверждения», подтверждает: архитектор (Справочник видов изделий → Активация)
- [`FR-PT-DELETE-001.H01`](dict-product-type/sf-delete/fr.md#fr-pt-delete-001-assumptions) — допущение, статус «требует подтверждения», подтверждает: владелец справочника (Справочник видов изделий → Удаление (fr.md))
- [`FR-PT-DELETE-001.H02`](dict-product-type/sf-delete/fr.md#fr-pt-delete-001-assumptions) — допущение, статус «требует подтверждения», подтверждает: архитектор (Справочник видов изделий → Удаление (fr.md))
- [`FR-PT-DELETE-001.H03`](dict-product-type/sf-delete/fr.md#fr-pt-delete-001-assumptions) — допущение, статус «требует подтверждения», подтверждает: владелец справочника (Справочник видов изделий → Удаление (fr.md))
- [`FR-PT-DELETE-003.H02`](dict-product-type/sf-delete/fr.md#fr-pt-delete-003-assumptions) — допущение, статус «требует подтверждения», подтверждает: владелец справочника (Справочник видов изделий → Удаление (fr.md))
- [`FR-PT-LIST-001.H01`](dict-product-type/sf-list/fr.md#fr-pt-list-001-assumptions) — допущение, статус «требует подтверждения», подтверждает: владелец справочника (Справочник видов изделий → Список (fr.md))
- [`FR-PT-LIST-006.H01`](dict-product-type/sf-list/fr.md#fr-pt-list-006-assumptions) — допущение, статус «требует подтверждения», подтверждает: владелец справочника (Справочник видов изделий → Список (fr.md))
- [`SF-PT-READ.H01`](dict-product-type/sf-read/index.md#sf-pt-read-assumptions) — допущение, статус «требует подтверждения», подтверждает: владелец справочника (Справочник видов изделий → Карточка)
- [`DR-PT-UPDATE-001.H02`](dict-product-type/sf-update/dr.md#dr-pt-update-001-assumptions) — допущение, статус «требует подтверждения», подтверждает: владелец справочника (Справочник видов изделий → Изменение (dr.md))
- [`NFR-001.Q01`](../global/nfr.md#nfr-001-questions) — вопрос, статус «открыт», решает: архитектор (Глобальные требования (nfr.md))
- [`NFR-003.Q01`](../global/nfr.md#nfr-003-questions) — вопрос, статус «открыт», решает: заказчик (Глобальные требования (nfr.md))
- [`NFR-004.H01`](../global/nfr.md#nfr-004-assumptions) — допущение, статус «требует подтверждения», подтверждает: владелец продукта (Глобальные требования (nfr.md))
- [`NFR-005.H01`](../global/nfr.md#nfr-005-assumptions) — допущение, статус «требует подтверждения», подтверждает: аналитик (Глобальные требования (nfr.md))
- [`UI-G-CATALOG-001.H01`](../global/sf-g-catalog/ui.md#ui-g-catalog-001-assumptions) — допущение, статус «требует подтверждения», подтверждает: архитектор (Глобальные требования → Каталог справочников (ui.md))
- [`UI-G-CATALOG-001.H02`](../global/sf-g-catalog/ui.md#ui-g-catalog-001-assumptions) — допущение, статус «требует подтверждения», подтверждает: владелец продукта (Глобальные требования → Каталог справочников (ui.md))
- [`UI-G-CATALOG-001.H03`](../global/sf-g-catalog/ui.md#ui-g-catalog-001-assumptions) — допущение, статус «требует подтверждения», подтверждает: владелец продукта (Глобальные требования → Каталог справочников (ui.md))
- [`UI-G-COLUMNS-001.H01`](../global/sf-g-columns/ui.md#ui-g-columns-001-assumptions) — допущение, статус «требует подтверждения», подтверждает: владелец продукта (Глобальные требования → Настройка столбцов таблицы (ui.md))
- [`UI-G-COLUMNS-001.H02`](../global/sf-g-columns/ui.md#ui-g-columns-001-assumptions) — допущение, статус «требует подтверждения», подтверждает: архитектор (Глобальные требования → Настройка столбцов таблицы (ui.md))
- [`UI-G-CONFIRM-001.H01`](../global/sf-g-confirm/ui.md#ui-g-confirm-001-assumptions) — допущение, статус «требует подтверждения», подтверждает: владелец продукта (Глобальные требования → Подтверждение необратимого действия (ui.md))
- [`UI-G-DICT-001.H01`](../global/sf-g-dict/ui.md#ui-g-dict-001-assumptions) — допущение, статус «требует подтверждения», подтверждает: архитектор (Глобальные требования → Типовой экран справочника (ui.md))
- [`UI-G-FILTER-001.H01`](../global/sf-g-filter/ui.md#ui-g-filter-001-assumptions) — допущение, статус «требует подтверждения», подтверждает: владелец продукта (Глобальные требования → Фильтрация (ui.md))
- [`UI-G-FILTER-001.H02`](../global/sf-g-filter/ui.md#ui-g-filter-001-assumptions) — допущение, статус «требует подтверждения», подтверждает: владелец продукта (Глобальные требования → Фильтрация (ui.md))
- [`UI-G-FORM-001.Q01`](../global/sf-g-form/ui.md#ui-g-form-001-questions) — вопрос, статус «открыт», решает: владелец продукта (Глобальные требования → Модальная форма записи (ui.md))
- [`UI-G-LOCK-001.H01`](../global/sf-g-lock/ui.md#ui-g-lock-001-assumptions) — допущение, статус «требует подтверждения», подтверждает: владелец продукта (Глобальные требования → Защита от одновременного изменения (ui.md))
- [`UI-G-LOCK-001.H02`](../global/sf-g-lock/ui.md#ui-g-lock-001-assumptions) — допущение, статус «требует подтверждения», подтверждает: владелец продукта (Глобальные требования → Защита от одновременного изменения (ui.md))
- [`FR-G-PAG-001.H01`](../global/sf-g-pag/fr.md#fr-g-pag-001-assumptions) — допущение, статус «требует подтверждения», подтверждает: владелец продукта (Глобальные требования → Пагинация (fr.md))
- [`UI-G-PAG-001.H01`](../global/sf-g-pag/ui.md#ui-g-pag-001-assumptions) — допущение, статус «требует подтверждения», подтверждает: владелец продукта (Глобальные требования → Пагинация (ui.md))
- [`UI-G-SELECT-001.H01`](../global/sf-g-select/ui.md#ui-g-select-001-assumptions) — допущение, статус «требует подтверждения», подтверждает: владелец продукта (Глобальные требования → Выделение строк и массовые действия (ui.md))
- [`UI-G-SESSION-001.H01`](../global/sf-g-session/ui.md#ui-g-session-001-assumptions) — допущение, статус «требует подтверждения», подтверждает: владелец продукта (Глобальные требования → Истёкшая сессия (ui.md))
- [`UI-G-SESSION-001.H02`](../global/sf-g-session/ui.md#ui-g-session-001-assumptions) — допущение, статус «требует подтверждения», подтверждает: владелец продукта (Глобальные требования → Истёкшая сессия (ui.md))
- [`UI-G-SESSION-001.H03`](../global/sf-g-session/ui.md#ui-g-session-001-assumptions) — допущение, статус «требует подтверждения», подтверждает: архитектор (Глобальные требования → Истёкшая сессия (ui.md))
- [`UI-G-TABLE-002.H01`](../global/sf-g-table/ui.md#ui-g-table-002-assumptions) — допущение, статус «требует подтверждения», подтверждает: владелец продукта (Глобальные требования → Таблица списка и её состояния (ui.md))
- [`UI-G-TOAST-001.H01`](../global/sf-g-toast/ui.md#ui-g-toast-001-assumptions) — допущение, статус «требует подтверждения», подтверждает: владелец продукта (Глобальные требования → Всплывающие уведомления (ui.md))
- [`UI-G-TOAST-001.H02`](../global/sf-g-toast/ui.md#ui-g-toast-001-assumptions) — допущение, статус «требует подтверждения», подтверждает: владелец продукта (Глобальные требования → Всплывающие уведомления (ui.md))
- [`UI-G-TOAST-001.H03`](../global/sf-g-toast/ui.md#ui-g-toast-001-assumptions) — допущение, статус «требует подтверждения», подтверждает: владелец продукта (Глобальные требования → Всплывающие уведомления (ui.md))
- [`SR-001.H01`](../global/sr.md#sr-001-assumptions) — допущение, статус «требует подтверждения», подтверждает: заказчик (Глобальные требования (sr.md))

</details>

<details class="success dash-check"><summary>Битые ссылки (ведут на несуществующий файл или раздел)<span class="dash-ok">Замечаний нет</span></summary></details>

## Последние изменения {#dash-changes}

Записей в журналах изменений пока нет.

<!-- END GENERATED DASHBOARD -->
