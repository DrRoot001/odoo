# Module: account_test

- **Module ID:** MOD-015
- **Path:** `addons/account_test`
- **Manifest:** `addons/account_test/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Asserts on accounting.
======================
With this module you can manually check consistencies and inconsistencies of accounting module from menu Reporting/Accounting/Accounting Tests.

You can write a query in order to create Consistency Test and you will get the result of the test
in PDF format which can be accessed by Menu Reporting -> Accounting Tests, then select the test
and print the report from Print button in header area.


Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
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
    "views/accounting_assert_test_views.xml",
    "report/accounting_assert_test_reports.xml",
    "data/accounting_assert_test_data.xml",
    "report/report_account_test_templates.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/account_test/__init__.py` (5 lines)
- `addons/account_test/__manifest__.py` (28 lines)
- `addons/account_test/data/accounting_assert_test_data.xml` (140 lines)
- `addons/account_test/i18n/account_test.pot` (257 lines)
- `addons/account_test/i18n/af.po` (267 lines)
- `addons/account_test/i18n/am.po` (266 lines)
- `addons/account_test/i18n/ar.po` (286 lines)
- `addons/account_test/i18n/az.po` (263 lines)
- `addons/account_test/i18n/bg.po` (266 lines)
- `addons/account_test/i18n/bs.po` (269 lines)
- `addons/account_test/i18n/ca.po` (283 lines)
- `addons/account_test/i18n/cs.po` (271 lines)
- `addons/account_test/i18n/da.po` (280 lines)
- `addons/account_test/i18n/de.po` (277 lines)
- `addons/account_test/i18n/el.po` (274 lines)
- `addons/account_test/i18n/es.po` (279 lines)
- `addons/account_test/i18n/es_CL.po` (69 lines)
- `addons/account_test/i18n/et.po` (283 lines)
- `addons/account_test/i18n/eu.po` (266 lines)
- `addons/account_test/i18n/fa.po` (269 lines)
- `addons/account_test/i18n/fi.po` (274 lines)
- `addons/account_test/i18n/fo.po` (266 lines)
- `addons/account_test/i18n/fr.po` (276 lines)
- `addons/account_test/i18n/fr_BE.po` (61 lines)
- `addons/account_test/i18n/fr_CA.po` (69 lines)
- `addons/account_test/i18n/gl.po` (266 lines)
- `addons/account_test/i18n/gu.po` (268 lines)
- `addons/account_test/i18n/he.po` (268 lines)
- `addons/account_test/i18n/hr.po` (274 lines)
- `addons/account_test/i18n/hu.po` (286 lines)
- `addons/account_test/i18n/id.po` (273 lines)
- `addons/account_test/i18n/is.po` (269 lines)
- `addons/account_test/i18n/it.po` (283 lines)
- `addons/account_test/i18n/ja.po` (271 lines)
- `addons/account_test/i18n/ka.po` (266 lines)
- `addons/account_test/i18n/kab.po` (266 lines)
- `addons/account_test/i18n/kk.po` (265 lines)
- `addons/account_test/i18n/km.po` (267 lines)
- `addons/account_test/i18n/ko.po` (277 lines)
- `addons/account_test/i18n/lo.po` (266 lines)
- `addons/account_test/i18n/lt.po` (273 lines)
- `addons/account_test/i18n/lv.po` (267 lines)
- `addons/account_test/i18n/mk.po` (266 lines)
- `addons/account_test/i18n/ml_IN.po` (266 lines)
- `addons/account_test/i18n/mn.po` (279 lines)
- `addons/account_test/i18n/nb.po` (271 lines)
- `addons/account_test/i18n/nl.po` (281 lines)
- `addons/account_test/i18n/pl.po` (285 lines)
- `addons/account_test/i18n/pt.po` (284 lines)
- `addons/account_test/i18n/pt_BR.po` (283 lines)
- `addons/account_test/i18n/ro.po` (279 lines)
- `addons/account_test/i18n/ru.po` (283 lines)
- `addons/account_test/i18n/sk.po` (278 lines)
- `addons/account_test/i18n/sl.po` (264 lines)
- `addons/account_test/i18n/sq.po` (266 lines)
- `addons/account_test/i18n/sr@latin.po` (268 lines)
- `addons/account_test/i18n/sv.po` (271 lines)
- `addons/account_test/i18n/ta.po` (270 lines)
- `addons/account_test/i18n/th.po` (271 lines)
- `addons/account_test/i18n/tr.po` (282 lines)
- `addons/account_test/i18n/uk.po` (285 lines)
- `addons/account_test/i18n/vi.po` (268 lines)
- `addons/account_test/i18n/zh_CN.po` (272 lines)
- `addons/account_test/i18n/zh_TW.po` (272 lines)
- `addons/account_test/models/__init__.py` (4 lines)
- `addons/account_test/models/accounting_assert_test.py` (24 lines)
- `addons/account_test/report/__init__.py` (4 lines)
- `addons/account_test/report/accounting_assert_test_reports.xml` (11 lines)
- `addons/account_test/report/report_account_test.py` (75 lines)
- `addons/account_test/report/report_account_test_templates.xml` (21 lines)
- `addons/account_test/security/ir.access.csv` (3 lines)
- `addons/account_test/views/accounting_assert_test_views.xml` (92 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
