# Module: account_check_printing

- **Module ID:** MOD-002
- **Path:** `addons/account_check_printing`
- **Manifest:** `addons/account_check_printing/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Check printing basic features


This module offers the basic functionalities to make payments by printing checks.
It must be used as a dependency for modules that provide country-specific check templates.
The check settings are located in the accounting journals configuration page.
    

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 12 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
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
    "data/account_check_printing_data.xml",
    "views/account_journal_views.xml",
    "views/account_payment_views.xml",
    "views/res_config_settings_views.xml",
    "wizard/print_prenumbered_checks_views.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/account_check_printing/__init__.py` (8 lines)
- `addons/account_check_printing/__manifest__.py` (24 lines)
- `addons/account_check_printing/data/account_check_printing_data.xml` (25 lines)
- `addons/account_check_printing/i18n/account_check_printing.pot` (458 lines)
- `addons/account_check_printing/i18n/af.po` (478 lines)
- `addons/account_check_printing/i18n/am.po` (474 lines)
- `addons/account_check_printing/i18n/ar.po` (523 lines)
- `addons/account_check_printing/i18n/az.po` (478 lines)
- `addons/account_check_printing/i18n/bg.po` (506 lines)
- `addons/account_check_printing/i18n/bs.po` (481 lines)
- `addons/account_check_printing/i18n/ca.po` (513 lines)
- `addons/account_check_printing/i18n/cs.po` (508 lines)
- `addons/account_check_printing/i18n/da.po` (525 lines)
- `addons/account_check_printing/i18n/de.po` (544 lines)
- `addons/account_check_printing/i18n/el.po` (485 lines)
- `addons/account_check_printing/i18n/en_AU.po` (270 lines)
- `addons/account_check_printing/i18n/en_CA.po` (494 lines)
- `addons/account_check_printing/i18n/es.po` (529 lines)
- `addons/account_check_printing/i18n/es_419.po` (530 lines)
- `addons/account_check_printing/i18n/es_CL.po` (65 lines)
- `addons/account_check_printing/i18n/et.po` (504 lines)
- `addons/account_check_printing/i18n/eu.po` (477 lines)
- `addons/account_check_printing/i18n/fa.po` (507 lines)
- `addons/account_check_printing/i18n/fi.po` (535 lines)
- `addons/account_check_printing/i18n/fo.po` (477 lines)
- `addons/account_check_printing/i18n/fr.po` (539 lines)
- `addons/account_check_printing/i18n/fr_BE.po` (49 lines)
- `addons/account_check_printing/i18n/fr_CA.po` (65 lines)
- `addons/account_check_printing/i18n/gl.po` (477 lines)
- `addons/account_check_printing/i18n/gu.po` (478 lines)
- `addons/account_check_printing/i18n/he.po` (504 lines)
- `addons/account_check_printing/i18n/hi.po` (496 lines)
- `addons/account_check_printing/i18n/hr.po` (487 lines)
- `addons/account_check_printing/i18n/hu.po` (506 lines)
- `addons/account_check_printing/i18n/id.po` (524 lines)
- `addons/account_check_printing/i18n/is.po` (479 lines)
- `addons/account_check_printing/i18n/it.po` (537 lines)
- `addons/account_check_printing/i18n/ja.po` (527 lines)
- `addons/account_check_printing/i18n/ka.po` (477 lines)
- `addons/account_check_printing/i18n/kab.po` (475 lines)
- `addons/account_check_printing/i18n/km.po` (477 lines)
- `addons/account_check_printing/i18n/ko.po` (517 lines)
- `addons/account_check_printing/i18n/ku.po` (482 lines)
- `addons/account_check_printing/i18n/lo.po` (508 lines)
- `addons/account_check_printing/i18n/lt.po` (505 lines)
- `addons/account_check_printing/i18n/lv.po` (486 lines)
- `addons/account_check_printing/i18n/mk.po` (477 lines)
- `addons/account_check_printing/i18n/ml_IN.po` (477 lines)
- `addons/account_check_printing/i18n/mn.po` (502 lines)
- `addons/account_check_printing/i18n/my.po` (477 lines)
- `addons/account_check_printing/i18n/nb.po` (482 lines)
- `addons/account_check_printing/i18n/nl.po` (531 lines)
- `addons/account_check_printing/i18n/pl.po` (544 lines)
- `addons/account_check_printing/i18n/pt.po` (518 lines)
- `addons/account_check_printing/i18n/pt_BR.po` (531 lines)
- `addons/account_check_printing/i18n/ro.po` (524 lines)
- `addons/account_check_printing/i18n/ru.po` (525 lines)
- `addons/account_check_printing/i18n/sk.po` (504 lines)
- `addons/account_check_printing/i18n/sl.po` (514 lines)
- `addons/account_check_printing/i18n/sq.po` (478 lines)
- `addons/account_check_printing/i18n/sr@latin.po` (511 lines)
- `addons/account_check_printing/i18n/sv.po` (544 lines)
- `addons/account_check_printing/i18n/ta.po` (478 lines)
- `addons/account_check_printing/i18n/th.po` (508 lines)
- `addons/account_check_printing/i18n/tr.po` (541 lines)
- `addons/account_check_printing/i18n/uk.po` (534 lines)
- `addons/account_check_printing/i18n/uz.po` (587 lines)
- `addons/account_check_printing/i18n/vi.po` (519 lines)
- `addons/account_check_printing/i18n/zh_CN.po` (507 lines)
- `addons/account_check_printing/i18n/zh_TW.po` (489 lines)
- `addons/account_check_printing/models/__init__.py` (8 lines)
- `addons/account_check_printing/models/account_journal.py` (120 lines)
- `addons/account_check_printing/models/account_payment.py` (367 lines)
- `addons/account_check_printing/models/account_payment_method.py` (14 lines)
- `addons/account_check_printing/models/res_company.py` (44 lines)
- `addons/account_check_printing/models/res_config_settings.py` (47 lines)
- `addons/account_check_printing/security/ir.access.csv` (2 lines)
- `addons/account_check_printing/static/description/icon.png` (6 lines)
- `addons/account_check_printing/static/description/icon.svg` (1 lines)
- `addons/account_check_printing/static/description/icon_hi.png` (9 lines)
- `addons/account_check_printing/tests/__init__.py` (1 lines)
- `addons/account_check_printing/tests/test_print_check.py` (610 lines)
- `addons/account_check_printing/views/account_journal_views.xml` (41 lines)
- `addons/account_check_printing/views/account_payment_views.xml` (37 lines)
- `addons/account_check_printing/views/res_config_settings_views.xml` (38 lines)
- `addons/account_check_printing/wizard/__init__.py` (4 lines)
- `addons/account_check_printing/wizard/print_prenumbered_checks.py` (32 lines)
- `addons/account_check_printing/wizard/print_prenumbered_checks_views.xml` (22 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
