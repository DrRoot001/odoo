# Module: pos_account_tax_python

- **Module ID:** MOD-422
- **Path:** `addons/pos_account_tax_python`
- **Manifest:** `addons/pos_account_tax_python/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Add code to manage custom taxes to the POS assets bundle

Declared dependencies: `account_tax_python`, `point_of_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account_tax_python",
    "point_of_sale"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "account_tax_python/static/src/helpers/*.js"
    ],
    "web.assets_unit_tests": [
      "pos_account_tax_python/static/tests/unit/data/**/*"
    ],
    "web.assets_tests": [
      "pos_account_tax_python/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_account_tax_python/__init__.py` (1 lines)
- `addons/pos_account_tax_python/__manifest__.py` (22 lines)
- `addons/pos_account_tax_python/i18n/ar.po` (46 lines)
- `addons/pos_account_tax_python/i18n/az.po` (44 lines)
- `addons/pos_account_tax_python/i18n/bg.po` (44 lines)
- `addons/pos_account_tax_python/i18n/bs.po` (46 lines)
- `addons/pos_account_tax_python/i18n/ca.po` (45 lines)
- `addons/pos_account_tax_python/i18n/cs.po` (45 lines)
- `addons/pos_account_tax_python/i18n/da.po` (44 lines)
- `addons/pos_account_tax_python/i18n/de.po` (47 lines)
- `addons/pos_account_tax_python/i18n/el.po` (44 lines)
- `addons/pos_account_tax_python/i18n/es.po` (47 lines)
- `addons/pos_account_tax_python/i18n/es_419.po` (45 lines)
- `addons/pos_account_tax_python/i18n/et.po` (44 lines)
- `addons/pos_account_tax_python/i18n/fa.po` (44 lines)
- `addons/pos_account_tax_python/i18n/fi.po` (45 lines)
- `addons/pos_account_tax_python/i18n/fr.po` (45 lines)
- `addons/pos_account_tax_python/i18n/he.po` (45 lines)
- `addons/pos_account_tax_python/i18n/hi.po` (44 lines)
- `addons/pos_account_tax_python/i18n/hr.po` (45 lines)
- `addons/pos_account_tax_python/i18n/hu.po` (44 lines)
- `addons/pos_account_tax_python/i18n/id.po` (45 lines)
- `addons/pos_account_tax_python/i18n/it.po` (45 lines)
- `addons/pos_account_tax_python/i18n/ja.po` (45 lines)
- `addons/pos_account_tax_python/i18n/kab.po` (45 lines)
- `addons/pos_account_tax_python/i18n/ko.po` (45 lines)
- `addons/pos_account_tax_python/i18n/ku.po` (44 lines)
- `addons/pos_account_tax_python/i18n/lo.po` (44 lines)
- `addons/pos_account_tax_python/i18n/lt.po` (46 lines)
- `addons/pos_account_tax_python/i18n/lv.po` (45 lines)
- `addons/pos_account_tax_python/i18n/mn.po` (44 lines)
- `addons/pos_account_tax_python/i18n/my.po` (44 lines)
- `addons/pos_account_tax_python/i18n/nb.po` (44 lines)
- `addons/pos_account_tax_python/i18n/nl.po` (46 lines)
- `addons/pos_account_tax_python/i18n/pl.po` (46 lines)
- `addons/pos_account_tax_python/i18n/pos_account_tax_python.pot` (41 lines)
- `addons/pos_account_tax_python/i18n/pt.po` (44 lines)
- `addons/pos_account_tax_python/i18n/pt_BR.po` (48 lines)
- `addons/pos_account_tax_python/i18n/ro.po` (46 lines)
- `addons/pos_account_tax_python/i18n/ru.po` (46 lines)
- `addons/pos_account_tax_python/i18n/sk.po` (44 lines)
- `addons/pos_account_tax_python/i18n/sl.po` (45 lines)
- `addons/pos_account_tax_python/i18n/sr@latin.po` (45 lines)
- `addons/pos_account_tax_python/i18n/sv.po` (45 lines)
- `addons/pos_account_tax_python/i18n/th.po` (45 lines)
- `addons/pos_account_tax_python/i18n/tr.po` (46 lines)
- `addons/pos_account_tax_python/i18n/uk.po` (45 lines)
- `addons/pos_account_tax_python/i18n/uz.po` (55 lines)
- `addons/pos_account_tax_python/i18n/vi.po` (45 lines)
- `addons/pos_account_tax_python/i18n/zh_CN.po` (45 lines)
- `addons/pos_account_tax_python/i18n/zh_TW.po` (45 lines)
- `addons/pos_account_tax_python/models/__init__.py` (1 lines)
- `addons/pos_account_tax_python/models/account_tax.py` (9 lines)
- `addons/pos_account_tax_python/static/tests/tours/test_taxes_tax_totals_summary.js` (51 lines)
- `addons/pos_account_tax_python/static/tests/unit/data/pos_printer.data.js` (8 lines)
- `addons/pos_account_tax_python/tests/__init__.py` (1 lines)
- `addons/pos_account_tax_python/tests/test_taxes_tax_totals_summary.py` (69 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
