# Observatory Content Model

## Purpose

The Observatory interface must grow as evidence accumulates. Its navigation and rendering logic must not depend on the current number of signals or themes.

The current implementation is a static, Git-backed site. The record blocks in `index.html` are the canonical content source; the interface discovers them from their metadata. This is a data-driven first stage, not yet a database-backed CMS.

## Signal records

Each signal is one canonical record. Add exactly one record block per signal and assign it a stable, unique identifier.

Required metadata:

- `data-signal-record`: marks the block as a signal record.
- `data-signal-id`: canonical identifier, for example `UAE-HI-009` or `KSA-HI-001`.
- `data-primary-radar`: exactly one primary radar key.
- `data-radars`: comma-separated radar keys. Must include the primary radar.
- The first `h2` inside the record is used as its display title.

Allowed radar keys:

- `regulatory`
- `reimbursement`
- `payer`
- `provider`
- `digital`
- `capital`
- `workforce`

The existing `id` attribute may be retained for in-page navigation, but signal discovery and routing must use `data-signal-id`, not a hard-coded list of element IDs.

### Signal rules

1. A signal has one canonical record and may appear in multiple radar lists through its `data-radars` tags.
2. Never duplicate a signal record to make it appear in another radar.
3. Radar lists, linked-record counts and Observatory signal totals are derived from the records present in the page.
4. Adding a signal must not require editing JavaScript mapping tables or title dictionaries.
5. Keep evidence, jurisdiction, status, confidence, research boundaries and source links inside the canonical record.
6. Do not infer a signal's existence from a radar category; an empty radar is a research gap, not proof of no market activity.

## Cross-radar themes

Each theme is one canonical article marked with:

- `data-theme-record`
- A unique `data-theme-id`, for example `UAE-THEME-009`

Theme totals are derived from the theme records present in the page. A theme may link to existing signals using buttons with `data-signal-open="UAE-HI-009"`. Those links must point to canonical signal IDs.

Themes are analytical syntheses, not duplicate signal records. Keep their evidence base, emerging interpretation and next test explicit.

## Derived interface elements

The following are generated from the records, not maintained as independent counts or mapping tables:

- Signal lists inside each radar
- Number of signals linked to each radar
- Total documented signal count
- Total cross-radar theme count
- Total radar count

The radar catalogue itself defines the seven observation lenses. Signal-to-radar relationships belong to the signal record, not to a separate hard-coded mapping object.

## Current scope and next architecture phase

- UAE currently contains the eight initial signal records.
- The seven radar lenses are shared across GCC countries.
- Other GCC markets must remain visibly unpopulated until evidence is documented.
- Cross-radar themes currently represent UAE analysis.
- Evidence is currently documented within signal records. A separate reusable Evidence Registry, with stable evidence IDs and many-to-many links to signals, remains a planned next phase.
- The site has no backend or CMS yet. New content is added to the Git-backed source, while the interface logic remains unchanged.

## Change-control checklist

Before accepting a new signal or theme:

- Confirm the identifier is unique.
- Confirm the primary radar is included in all radar tags.
- Confirm jurisdiction and evidence scope are explicit.
- Keep verified facts separate from interpretation and hypotheses.
- Verify every cross-radar link resolves to an existing signal.
- Confirm totals and radar lists update from the record metadata.
- Run JavaScript syntax and structural checks.
- Deploy to Preview and verify before any Production release.
