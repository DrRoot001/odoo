# Module: spreadsheet_account

- **Module ID:** MOD-545
- **Path:** `addons/spreadsheet_account`
- **Manifest:** `addons/spreadsheet_account/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

Spreadsheet Accounting formulas

Spreadsheet Accounting formulas

Declared dependencies: `spreadsheet`, `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 12 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 17 | Client behavior/assets. |
| Tests | 7 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "spreadsheet",
    "account"
  ],
  "assets": {
    "spreadsheet.o_spreadsheet_core": [
      [
        "after",
        "spreadsheet/static/src/o_spreadsheet/o_spreadsheet.js",
        "spreadsheet_account/static/src/**/*.js"
      ]
    ],
    "web.assets_unit_tests": [
      "spreadsheet_account/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/spreadsheet_account/__init__.py` (1 lines)
- `addons/spreadsheet_account/__manifest__.py` (23 lines)
- `addons/spreadsheet_account/i18n/ar.po` (378 lines)
- `addons/spreadsheet_account/i18n/az.po` (369 lines)
- `addons/spreadsheet_account/i18n/bg.po` (369 lines)
- `addons/spreadsheet_account/i18n/bs.po` (391 lines)
- `addons/spreadsheet_account/i18n/ca.po` (381 lines)
- `addons/spreadsheet_account/i18n/cs.po` (374 lines)
- `addons/spreadsheet_account/i18n/da.po` (397 lines)
- `addons/spreadsheet_account/i18n/de.po` (385 lines)
- `addons/spreadsheet_account/i18n/el.po` (370 lines)
- `addons/spreadsheet_account/i18n/es.po` (389 lines)
- `addons/spreadsheet_account/i18n/es_419.po` (380 lines)
- `addons/spreadsheet_account/i18n/et.po` (371 lines)
- `addons/spreadsheet_account/i18n/fa.po` (373 lines)
- `addons/spreadsheet_account/i18n/fi.po` (381 lines)
- `addons/spreadsheet_account/i18n/fr.po` (382 lines)
- `addons/spreadsheet_account/i18n/he.po` (370 lines)
- `addons/spreadsheet_account/i18n/hi.po` (369 lines)
- `addons/spreadsheet_account/i18n/hr.po` (405 lines)
- `addons/spreadsheet_account/i18n/hu.po` (370 lines)
- `addons/spreadsheet_account/i18n/id.po` (380 lines)
- `addons/spreadsheet_account/i18n/it.po` (382 lines)
- `addons/spreadsheet_account/i18n/ja.po` (374 lines)
- `addons/spreadsheet_account/i18n/kab.po` (374 lines)
- `addons/spreadsheet_account/i18n/ko.po` (375 lines)
- `addons/spreadsheet_account/i18n/ku.po` (368 lines)
- `addons/spreadsheet_account/i18n/lo.po` (372 lines)
- `addons/spreadsheet_account/i18n/lt.po` (371 lines)
- `addons/spreadsheet_account/i18n/lv.po` (391 lines)
- `addons/spreadsheet_account/i18n/mn.po` (370 lines)
- `addons/spreadsheet_account/i18n/my.po` (369 lines)
- `addons/spreadsheet_account/i18n/nb.po` (370 lines)
- `addons/spreadsheet_account/i18n/nl.po` (381 lines)
- `addons/spreadsheet_account/i18n/pl.po` (378 lines)
- `addons/spreadsheet_account/i18n/pt.po` (378 lines)
- `addons/spreadsheet_account/i18n/pt_BR.po` (379 lines)
- `addons/spreadsheet_account/i18n/ro.po` (381 lines)
- `addons/spreadsheet_account/i18n/ru.po` (381 lines)
- `addons/spreadsheet_account/i18n/sk.po` (390 lines)
- `addons/spreadsheet_account/i18n/sl.po` (371 lines)
- `addons/spreadsheet_account/i18n/spreadsheet_account.pot` (363 lines)
- `addons/spreadsheet_account/i18n/sr@latin.po` (370 lines)
- `addons/spreadsheet_account/i18n/sv.po` (381 lines)
- `addons/spreadsheet_account/i18n/th.po` (374 lines)
- `addons/spreadsheet_account/i18n/tr.po` (379 lines)
- `addons/spreadsheet_account/i18n/uk.po` (374 lines)
- `addons/spreadsheet_account/i18n/uz.po` (433 lines)
- `addons/spreadsheet_account/i18n/vi.po` (376 lines)
- `addons/spreadsheet_account/i18n/zh_CN.po` (374 lines)
- `addons/spreadsheet_account/i18n/zh_TW.po` (377 lines)
- `addons/spreadsheet_account/models/__init__.py` (2 lines)
- `addons/spreadsheet_account/models/account.py` (240 lines)
- `addons/spreadsheet_account/models/res_company.py` (32 lines)
- `addons/spreadsheet_account/static/src/account_group_auto_complete.js` (52 lines)
- `addons/spreadsheet_account/static/src/accounting_functions.js` (542 lines)
- `addons/spreadsheet_account/static/src/fiscal_year_global_filter.js` (66 lines)
- `addons/spreadsheet_account/static/src/index.js` (110 lines)
- `addons/spreadsheet_account/static/src/plugins/accounting_plugin.js` (173 lines)
- `addons/spreadsheet_account/static/src/utils.js` (28 lines)
- `addons/spreadsheet_account/static/tests/accounting_test_data.js` (68 lines)
- `addons/spreadsheet_account/static/tests/mock_server.js` (19 lines)
- `addons/spreadsheet_account/static/tests/model/account_groups.test.js` (35 lines)
- `addons/spreadsheet_account/static/tests/model/account_groups_auto_complete.test.js` (43 lines)
- `addons/spreadsheet_account/static/tests/model/accounting.test.js` (469 lines)
- `addons/spreadsheet_account/static/tests/model/balance_tag.test.js` (70 lines)
- `addons/spreadsheet_account/static/tests/model/fiscal_year.test.js` (126 lines)
- `addons/spreadsheet_account/static/tests/model/fiscal_year_global_filter.test.js` (76 lines)
- `addons/spreadsheet_account/static/tests/model/partner_balance.test.js` (76 lines)
- `addons/spreadsheet_account/static/tests/model/residual_amount.test.js` (70 lines)
- `addons/spreadsheet_account/static/tests/ui/accounting_drilldown.test.js` (155 lines)
- `addons/spreadsheet_account/tests/__init__.py` (9 lines)
- `addons/spreadsheet_account/tests/test_account_group.py` (59 lines)
- `addons/spreadsheet_account/tests/test_balance_tag.py` (125 lines)
- `addons/spreadsheet_account/tests/test_company_fiscal_year.py` (103 lines)
- `addons/spreadsheet_account/tests/test_debit_credit.py` (1,079 lines)
- `addons/spreadsheet_account/tests/test_partner_balance.py` (228 lines)
- `addons/spreadsheet_account/tests/test_residual_amount.py` (196 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
