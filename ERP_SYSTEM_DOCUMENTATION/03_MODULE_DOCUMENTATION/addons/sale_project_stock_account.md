# Module: sale_project_stock_account

- **Module ID:** MOD-527
- **Path:** `addons/sale_project_stock_account`
- **Manifest:** `addons/sale_project_stock_account/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Technical Bridge

No manifest description declared.

Declared dependencies: `sale_project`, `project_stock_account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "sale_project",
    "project_stock_account"
  ]
}
```

### Representative source files

- `addons/sale_project_stock_account/__init__.py` (3 lines)
- `addons/sale_project_stock_account/__manifest__.py` (11 lines)
- `addons/sale_project_stock_account/i18n/ar.po` (46 lines)
- `addons/sale_project_stock_account/i18n/az.po` (41 lines)
- `addons/sale_project_stock_account/i18n/bg.po` (41 lines)
- `addons/sale_project_stock_account/i18n/bs.po` (41 lines)
- `addons/sale_project_stock_account/i18n/ca.po` (41 lines)
- `addons/sale_project_stock_account/i18n/cs.po` (41 lines)
- `addons/sale_project_stock_account/i18n/da.po` (41 lines)
- `addons/sale_project_stock_account/i18n/de.po` (45 lines)
- `addons/sale_project_stock_account/i18n/el.po` (41 lines)
- `addons/sale_project_stock_account/i18n/es.po` (45 lines)
- `addons/sale_project_stock_account/i18n/es_419.po` (45 lines)
- `addons/sale_project_stock_account/i18n/et.po` (41 lines)
- `addons/sale_project_stock_account/i18n/fa.po` (41 lines)
- `addons/sale_project_stock_account/i18n/fi.po` (45 lines)
- `addons/sale_project_stock_account/i18n/fr.po` (41 lines)
- `addons/sale_project_stock_account/i18n/he.po` (41 lines)
- `addons/sale_project_stock_account/i18n/hi.po` (41 lines)
- `addons/sale_project_stock_account/i18n/hr.po` (41 lines)
- `addons/sale_project_stock_account/i18n/hu.po` (41 lines)
- `addons/sale_project_stock_account/i18n/id.po` (41 lines)
- `addons/sale_project_stock_account/i18n/it.po` (45 lines)
- `addons/sale_project_stock_account/i18n/ja.po` (41 lines)
- `addons/sale_project_stock_account/i18n/kab.po` (41 lines)
- `addons/sale_project_stock_account/i18n/ko.po` (41 lines)
- `addons/sale_project_stock_account/i18n/ku.po` (41 lines)
- `addons/sale_project_stock_account/i18n/lo.po` (41 lines)
- `addons/sale_project_stock_account/i18n/lt.po` (41 lines)
- `addons/sale_project_stock_account/i18n/lv.po` (41 lines)
- `addons/sale_project_stock_account/i18n/mn.po` (41 lines)
- `addons/sale_project_stock_account/i18n/my.po` (41 lines)
- `addons/sale_project_stock_account/i18n/nb.po` (41 lines)
- `addons/sale_project_stock_account/i18n/nl.po` (45 lines)
- `addons/sale_project_stock_account/i18n/pl.po` (41 lines)
- `addons/sale_project_stock_account/i18n/pt.po` (45 lines)
- `addons/sale_project_stock_account/i18n/pt_BR.po` (46 lines)
- `addons/sale_project_stock_account/i18n/ro.po` (41 lines)
- `addons/sale_project_stock_account/i18n/ru.po` (41 lines)
- `addons/sale_project_stock_account/i18n/sale_project_stock_account.pot` (41 lines)
- `addons/sale_project_stock_account/i18n/sk.po` (41 lines)
- `addons/sale_project_stock_account/i18n/sl.po` (41 lines)
- `addons/sale_project_stock_account/i18n/sr@latin.po` (41 lines)
- `addons/sale_project_stock_account/i18n/sv.po` (45 lines)
- `addons/sale_project_stock_account/i18n/th.po` (45 lines)
- `addons/sale_project_stock_account/i18n/tr.po` (45 lines)
- `addons/sale_project_stock_account/i18n/uk.po` (41 lines)
- `addons/sale_project_stock_account/i18n/uz.po` (41 lines)
- `addons/sale_project_stock_account/i18n/vi.po` (41 lines)
- `addons/sale_project_stock_account/i18n/zh_CN.po` (45 lines)
- `addons/sale_project_stock_account/i18n/zh_TW.po` (41 lines)
- `addons/sale_project_stock_account/models/__init__.py` (3 lines)
- `addons/sale_project_stock_account/models/stock_move.py` (16 lines)
- `addons/sale_project_stock_account/tests/__init__.py` (3 lines)
- `addons/sale_project_stock_account/tests/test_analytics_reinvoice.py` (88 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
