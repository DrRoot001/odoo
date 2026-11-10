# Module: account_edi

- **Module ID:** MOD-004
- **Path:** `addons/account_edi`
- **Manifest:** `addons/account_edi/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Electronic Data Interchange
=======================================
EDI is the electronic interchange of business information using a standardized format.

This is the base module for import and export of invoices in various EDI formats, and the
the transmission of said documents to various parties involved in the exchange (other company,
governements, etc.)
    

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 16 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 8 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
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
    "views/account_edi_document_views.xml",
    "views/account_move_views.xml",
    "views/account_journal_views.xml",
    "data/cron.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/account_edi/__init__.py` (4 lines)
- `addons/account_edi/__manifest__.py` (23 lines)
- `addons/account_edi/data/cron.xml` (11 lines)
- `addons/account_edi/i18n/account_edi.pot` (474 lines)
- `addons/account_edi/i18n/ar.po` (508 lines)
- `addons/account_edi/i18n/az.po` (484 lines)
- `addons/account_edi/i18n/bg.po` (484 lines)
- `addons/account_edi/i18n/bs.po` (486 lines)
- `addons/account_edi/i18n/ca.po` (511 lines)
- `addons/account_edi/i18n/cs.po` (508 lines)
- `addons/account_edi/i18n/da.po` (508 lines)
- `addons/account_edi/i18n/de.po` (525 lines)
- `addons/account_edi/i18n/el.po` (484 lines)
- `addons/account_edi/i18n/es.po` (522 lines)
- `addons/account_edi/i18n/es_419.po` (522 lines)
- `addons/account_edi/i18n/et.po` (506 lines)
- `addons/account_edi/i18n/fa.po` (498 lines)
- `addons/account_edi/i18n/fi.po` (518 lines)
- `addons/account_edi/i18n/fr.po` (524 lines)
- `addons/account_edi/i18n/he.po` (492 lines)
- `addons/account_edi/i18n/hi.po` (500 lines)
- `addons/account_edi/i18n/hr.po` (485 lines)
- `addons/account_edi/i18n/hu.po` (484 lines)
- `addons/account_edi/i18n/id.po` (506 lines)
- `addons/account_edi/i18n/it.po` (522 lines)
- `addons/account_edi/i18n/ja.po` (513 lines)
- `addons/account_edi/i18n/kab.po` (485 lines)
- `addons/account_edi/i18n/ko.po` (499 lines)
- `addons/account_edi/i18n/ku.po` (484 lines)
- `addons/account_edi/i18n/lo.po` (509 lines)
- `addons/account_edi/i18n/lt.po` (488 lines)
- `addons/account_edi/i18n/lv.po` (486 lines)
- `addons/account_edi/i18n/mn.po` (484 lines)
- `addons/account_edi/i18n/my.po` (485 lines)
- `addons/account_edi/i18n/nb.po` (484 lines)
- `addons/account_edi/i18n/nl.po` (524 lines)
- `addons/account_edi/i18n/pl.po` (522 lines)
- `addons/account_edi/i18n/pt.po` (509 lines)
- `addons/account_edi/i18n/pt_BR.po` (520 lines)
- `addons/account_edi/i18n/ro.po` (511 lines)
- `addons/account_edi/i18n/ru.po` (510 lines)
- `addons/account_edi/i18n/sk.po` (485 lines)
- `addons/account_edi/i18n/sl.po` (509 lines)
- `addons/account_edi/i18n/sr@latin.po` (485 lines)
- `addons/account_edi/i18n/sv.po` (525 lines)
- `addons/account_edi/i18n/th.po` (495 lines)
- `addons/account_edi/i18n/tr.po` (517 lines)
- `addons/account_edi/i18n/uk.po` (519 lines)
- `addons/account_edi/i18n/uz.po` (582 lines)
- `addons/account_edi/i18n/vi.po` (505 lines)
- `addons/account_edi/i18n/zh_CN.po` (500 lines)
- `addons/account_edi/i18n/zh_TW.po` (495 lines)
- `addons/account_edi/models/__init__.py` (7 lines)
- `addons/account_edi/models/account_edi_document.py` (282 lines)
- `addons/account_edi/models/account_edi_format.py` (128 lines)
- `addons/account_edi/models/account_journal.py` (83 lines)
- `addons/account_edi/models/account_move.py` (389 lines)
- `addons/account_edi/models/account_move_send.py` (19 lines)
- `addons/account_edi/models/ir_actions_report.py` (47 lines)
- `addons/account_edi/models/ir_attachment.py` (16 lines)
- `addons/account_edi/security/ir.access.csv` (5 lines)
- `addons/account_edi/tests/__init__.py` (6 lines)
- `addons/account_edi/tests/common.py` (141 lines)
- `addons/account_edi/tests/test_edi.py` (175 lines)
- `addons/account_edi/tests/test_import_vendor_bill.py` (23 lines)
- `addons/account_edi/views/account_edi_document_views.xml` (19 lines)
- `addons/account_edi/views/account_journal_views.xml` (19 lines)
- `addons/account_edi/views/account_move_views.xml` (172 lines)
- `addons/account_edi/wizard/__init__.py` (1 lines)
- `addons/account_edi/wizard/account_resequence.py` (23 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
