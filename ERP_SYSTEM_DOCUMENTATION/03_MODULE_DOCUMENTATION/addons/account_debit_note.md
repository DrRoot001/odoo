# Module: account_debit_note

- **Module ID:** MOD-003
- **Path:** `addons/account_debit_note`
- **Manifest:** `addons/account_debit_note/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Debit Notes


In a lot of countries, a debit note is used as an increase of the amounts of an existing invoice
or in some specific cases to cancel a credit note.
It is like a regular invoice, but we need to keep track of the link with the original invoice.
The wizard used is similar as the one for the credit note.
    

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account"
  ],
  "data": [
    "wizard/account_debit_note_view.xml",
    "views/account_move_view.xml",
    "views/account_journal_views.xml",
    "views/report_invoice.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/account_debit_note/__init__.py` (5 lines)
- `addons/account_debit_note/__manifest__.py` (23 lines)
- `addons/account_debit_note/i18n/account_debit_note.pot` (310 lines)
- `addons/account_debit_note/i18n/ar.po` (352 lines)
- `addons/account_debit_note/i18n/az.po` (322 lines)
- `addons/account_debit_note/i18n/bg.po` (324 lines)
- `addons/account_debit_note/i18n/bs.po` (322 lines)
- `addons/account_debit_note/i18n/ca.po` (335 lines)
- `addons/account_debit_note/i18n/cs.po` (349 lines)
- `addons/account_debit_note/i18n/da.po` (347 lines)
- `addons/account_debit_note/i18n/de.po` (367 lines)
- `addons/account_debit_note/i18n/el.po` (320 lines)
- `addons/account_debit_note/i18n/es.po` (369 lines)
- `addons/account_debit_note/i18n/es_419.po` (367 lines)
- `addons/account_debit_note/i18n/et.po` (331 lines)
- `addons/account_debit_note/i18n/fa.po` (333 lines)
- `addons/account_debit_note/i18n/fi.po` (365 lines)
- `addons/account_debit_note/i18n/fr.po` (367 lines)
- `addons/account_debit_note/i18n/fr_BE.po` (27 lines)
- `addons/account_debit_note/i18n/he.po` (332 lines)
- `addons/account_debit_note/i18n/hi.po` (336 lines)
- `addons/account_debit_note/i18n/hr.po` (323 lines)
- `addons/account_debit_note/i18n/hu.po` (322 lines)
- `addons/account_debit_note/i18n/id.po` (357 lines)
- `addons/account_debit_note/i18n/it.po` (368 lines)
- `addons/account_debit_note/i18n/ja.po` (364 lines)
- `addons/account_debit_note/i18n/kab.po` (321 lines)
- `addons/account_debit_note/i18n/ko.po` (336 lines)
- `addons/account_debit_note/i18n/ku.po` (322 lines)
- `addons/account_debit_note/i18n/lo.po` (344 lines)
- `addons/account_debit_note/i18n/lt.po` (334 lines)
- `addons/account_debit_note/i18n/lv.po` (324 lines)
- `addons/account_debit_note/i18n/mn.po` (322 lines)
- `addons/account_debit_note/i18n/my.po` (321 lines)
- `addons/account_debit_note/i18n/nb.po` (322 lines)
- `addons/account_debit_note/i18n/nl.po` (357 lines)
- `addons/account_debit_note/i18n/pl.po` (347 lines)
- `addons/account_debit_note/i18n/pt.po` (339 lines)
- `addons/account_debit_note/i18n/pt_BR.po` (367 lines)
- `addons/account_debit_note/i18n/ro.po` (340 lines)
- `addons/account_debit_note/i18n/ru.po` (341 lines)
- `addons/account_debit_note/i18n/sk.po` (323 lines)
- `addons/account_debit_note/i18n/sl.po` (339 lines)
- `addons/account_debit_note/i18n/sr@latin.po` (323 lines)
- `addons/account_debit_note/i18n/sv.po` (370 lines)
- `addons/account_debit_note/i18n/th.po` (329 lines)
- `addons/account_debit_note/i18n/tr.po` (355 lines)
- `addons/account_debit_note/i18n/uk.po` (352 lines)
- `addons/account_debit_note/i18n/uz.po` (381 lines)
- `addons/account_debit_note/i18n/vi.po` (336 lines)
- `addons/account_debit_note/i18n/zh_CN.po` (355 lines)
- `addons/account_debit_note/i18n/zh_TW.po` (344 lines)
- `addons/account_debit_note/models/__init__.py` (5 lines)
- `addons/account_debit_note/models/account_journal.py` (18 lines)
- `addons/account_debit_note/models/account_move.py` (52 lines)
- `addons/account_debit_note/security/ir.access.csv` (2 lines)
- `addons/account_debit_note/tests/__init__.py` (3 lines)
- `addons/account_debit_note/tests/test_out_debit_note.py` (48 lines)
- `addons/account_debit_note/views/account_journal_views.xml` (13 lines)
- `addons/account_debit_note/views/account_move_view.xml` (76 lines)
- `addons/account_debit_note/views/report_invoice.xml` (55 lines)
- `addons/account_debit_note/wizard/__init__.py` (4 lines)
- `addons/account_debit_note/wizard/account_debit_note.py` (96 lines)
- `addons/account_debit_note/wizard/account_debit_note_view.xml` (40 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
