# Реестр требований программного продукта {#registry}

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

## Основные функциональности (F) {#dash-f}

Статус F вычисляется по статусам её SF.

<div class="dash-total" markdown="span">:lucide-files: <span class="dash-total__name">Всего F</span> <b>1</b></div>

<div class="dash-tiles" data-n="4" markdown>

<span class="dash-tile dash-backlog is-zero"><span class="dash-tile__top">:lucide-file: 0</span><span class="dash-tile__name">бэклог</span></span>
<span class="dash-tile dash-in-progress"><span class="dash-tile__top">:lucide-file-clock: 1</span><span class="dash-tile__name">в работе</span></span>
<span class="dash-tile dash-released is-zero"><span class="dash-tile__top">:lucide-file-text: 0</span><span class="dash-tile__name">реализовано</span></span>
<span class="dash-tile dash-archived is-zero"><span class="dash-tile__top">:lucide-file-archive: 0</span><span class="dash-tile__name">архив</span></span>

</div>

## Детальные функциональности (SF) {#dash-sf}

<div class="dash-total" markdown="span">:lucide-files: <span class="dash-total__name">Всего SF</span> <b>6</b></div>

<div class="dash-tiles" data-n="6" markdown>

<span class="dash-tile dash-backlog is-zero"><span class="dash-tile__top">:lucide-file: 0</span><span class="dash-tile__name">бэклог</span></span>
<span class="dash-tile dash-analysis"><span class="dash-tile__top">:lucide-file-pen-line: 6</span><span class="dash-tile__name">анализ</span></span>
<span class="dash-tile dash-ready is-zero"><span class="dash-tile__top">:lucide-file-check: 0</span><span class="dash-tile__name">готово к разработке</span></span>
<span class="dash-tile dash-development is-zero"><span class="dash-tile__top">:lucide-file-braces: 0</span><span class="dash-tile__name">разработка</span></span>
<span class="dash-tile dash-released is-zero"><span class="dash-tile__top">:lucide-file-text: 0</span><span class="dash-tile__name">реализовано</span></span>
<span class="dash-tile dash-archived is-zero"><span class="dash-tile__top">:lucide-file-archive: 0</span><span class="dash-tile__name">архив</span></span>

</div>

## Прогресс по фичам {#dash-progress}

Доля SF фичи в каждом статусе; SF в архиве не учитываются.

<div class="dash-progress"><div class="dash-progress__row"><div class="dash-progress__title">Справочник видов изделий<small>в работе · 6 SF</small></div><div class="dash-bar"><span class="dash-analysis" style="width:100%" title="анализ: 6"></span></div><div class="dash-progress__done">реализовано <b>0 из 6</b></div></div></div>

<div class="dash-legend"><span class="dash-backlog"><i></i>бэклог</span><span class="dash-analysis"><i></i>анализ</span><span class="dash-ready"><i></i>готово к разработке</span><span class="dash-development"><i></i>разработка</span><span class="dash-released"><i></i>реализовано</span></div>

## Приоритет × статус SF {#dash-priority}

Число SF каждого приоритета в каждом статусе.

<table class="dash-matrix"><thead><tr><th>Приоритет</th><th class="dash-backlog"><i></i>бэклог</th><th class="dash-analysis"><i></i>анализ</th><th class="dash-ready"><i></i>готово к разработке</th><th class="dash-development"><i></i>разработка</th><th class="dash-released"><i></i>реализовано</th><th class="dash-archived"><i></i>архив</th><th>Всего</th></tr></thead><tbody><tr><th>must</th><td class="is-empty">—</td><td class="dash-analysis is-value">6</td><td class="is-empty">—</td><td class="is-empty">—</td><td class="is-empty">—</td><td class="is-empty">—</td><td><b>6</b></td></tr><tr><th>should</th><td class="is-empty">—</td><td class="is-empty">—</td><td class="is-empty">—</td><td class="is-empty">—</td><td class="is-empty">—</td><td class="is-empty">—</td><td><b>0</b></td></tr><tr><th>could</th><td class="is-empty">—</td><td class="is-empty">—</td><td class="is-empty">—</td><td class="is-empty">—</td><td class="is-empty">—</td><td class="is-empty">—</td><td><b>0</b></td></tr><tr><th>won&#x27;t</th><td class="is-empty">—</td><td class="is-empty">—</td><td class="is-empty">—</td><td class="is-empty">—</td><td class="is-empty">—</td><td class="is-empty">—</td><td><b>0</b></td></tr><tr class="dash-sum"><th>Всего</th><td>0</td><td>6</td><td>0</td><td>0</td><td>0</td><td>0</td><td>6</td></tr></tbody></table>

## Требует внимания {#dash-attention}

Групп с замечаниями: 1, замечаний: 13.

<details class="success dash-check"><summary>SF без функциональных требований (FR)<span class="dash-ok">Замечаний нет</span></summary></details>

<details class="success dash-check"><summary>FR без критериев приёмки<span class="dash-ok">Замечаний нет</span></summary></details>

<details class="success dash-check"><summary>SF без приоритета<span class="dash-ok">Замечаний нет</span></summary></details>

<details class="success dash-check"><summary>Повторяющиеся коды<span class="dash-ok">Замечаний нет</span></summary></details>

<details class="warning dash-check" open><summary>Неподтверждённые допущения<span class="dash-count">13</span></summary><ul><li><code>DR-PT-001.H01</code> — статус «требует подтверждения», подтверждает: архитектор (Справочник видов изделий (dr.md))</li><li><code>DR-PT-001.H02</code> — статус «требует подтверждения», подтверждает: архитектор (Справочник видов изделий (dr.md))</li><li><code>FR-PT-ACTIVATION-001.H01</code> — статус «требует подтверждения», подтверждает: владелец справочника (Справочник видов изделий → Активация (fr.md))</li><li><code>FR-PT-ACTIVATION-002.H01</code> — статус «требует подтверждения», подтверждает: владелец справочника (Справочник видов изделий → Активация (fr.md))</li><li><code>SF-PT-ACTIVATION.H01</code> — статус «требует подтверждения», подтверждает: архитектор (Справочник видов изделий → Активация)</li><li><code>FR-PT-DELETE-001.H01</code> — статус «требует подтверждения», подтверждает: владелец справочника (Справочник видов изделий → Удаление (fr.md))</li><li><code>FR-PT-DELETE-001.H02</code> — статус «требует подтверждения», подтверждает: архитектор (Справочник видов изделий → Удаление (fr.md))</li><li><code>FR-PT-DELETE-001.H03</code> — статус «требует подтверждения», подтверждает: владелец справочника (Справочник видов изделий → Удаление (fr.md))</li><li><code>FR-PT-DELETE-003.H02</code> — статус «требует подтверждения», подтверждает: владелец справочника (Справочник видов изделий → Удаление (fr.md))</li><li><code>FR-PT-LIST-001.H01</code> — статус «требует подтверждения», подтверждает: владелец справочника (Справочник видов изделий → Список (fr.md))</li><li class="dash-more">…ещё 3</li></ul></details>

<details class="success dash-check"><summary>Битые ссылки (ведут на несуществующий файл или раздел)<span class="dash-ok">Замечаний нет</span></summary></details>

## Последние изменения {#dash-changes}

Последние записи журналов изменений всех разделов реестра; версия — ссылка на коммит.

<table class="dash-changes"><thead><tr><th>Когда</th><th>Раздел</th><th>Версия</th><th>Файлы</th><th>Редактор</th></tr></thead><tbody><tr><td class="dash-when">24.11.2026 22:03</td><td>Справочник видов изделий → Создание</td><td><a href="https://github.com/DmitryKhilko/example-app-requirements-v2/commit/ac44b4e6fc8d5513e8f15b8308f784823dca982e" target="_blank" rel="noopener">0.01.08</a></td><td>api/AR-PT-CREATE-001.response.400.json</td><td>Dmitry Khilko</td></tr><tr><td class="dash-when">24.11.2026 22:02</td><td>Справочник видов изделий → Создание</td><td><a href="https://github.com/DmitryKhilko/example-app-requirements-v2/commit/41f81ed4ac8f0471e643c89276a30f752e16f6e0" target="_blank" rel="noopener">0.01.07</a></td><td>api/AR-PT-CREATE-001.response.201.schema.json</td><td>Dmitry Khilko</td></tr><tr><td class="dash-when">24.11.2026 22:02</td><td>Справочник видов изделий → Создание</td><td><a href="https://github.com/DmitryKhilko/example-app-requirements-v2/commit/7704c3b04a4aaedc4291621a6f4c2ce47e1b395c" target="_blank" rel="noopener">0.01.06</a></td><td>api/AR-PT-CREATE-001.request.schema.json</td><td>Dmitry Khilko</td></tr><tr><td class="dash-when">24.11.2026 22:02</td><td>Справочник видов изделий → Создание</td><td><a href="https://github.com/DmitryKhilko/example-app-requirements-v2/commit/b2a759e1e9cc0a356b5e4eb55ceb30a62374e692" target="_blank" rel="noopener">0.01.05</a></td><td>api/AR-PT-CREATE-001.request.invalid.json</td><td>Dmitry Khilko</td></tr><tr><td class="dash-when">24.11.2026 22:02</td><td>Справочник видов изделий → Создание</td><td><a href="https://github.com/DmitryKhilko/example-app-requirements-v2/commit/e2583e406951c541a29180c559ab553034b7edee" target="_blank" rel="noopener">0.01.04</a></td><td>index.md</td><td>Dmitry Khilko</td></tr></tbody></table>

<!-- END GENERATED DASHBOARD -->
