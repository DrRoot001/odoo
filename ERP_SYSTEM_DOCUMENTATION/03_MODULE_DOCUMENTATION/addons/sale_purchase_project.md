# Module: sale_purchase_project

- **Module ID:** MOD-529
- **Path:** `addons/sale_purchase_project`
- **Manifest:** `addons/sale_purchase_project/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Technical Bridge

No manifest description declared.

Declared dependencies: `sale_purchase`, `project_purchase`, `sale_project`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
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
    "sale_purchase",
    "project_purchase",
    "sale_project"
  ]
}
```

### Representative source files

- `addons/sale_purchase_project/__init__.py` (3 lines)
- `addons/sale_purchase_project/__manifest__.py` (11 lines)
- `addons/sale_purchase_project/i18n/ar.po` (61 lines)
- `addons/sale_purchase_project/i18n/az.po` (58 lines)
- `addons/sale_purchase_project/i18n/bg.po` (58 lines)
- `addons/sale_purchase_project/i18n/bs.po` (59 lines)
- `addons/sale_purchase_project/i18n/ca.po` (58 lines)
- `addons/sale_purchase_project/i18n/cs.po` (58 lines)
- `addons/sale_purchase_project/i18n/da.po` (59 lines)
- `addons/sale_purchase_project/i18n/de.po` (58 lines)
- `addons/sale_purchase_project/i18n/el.po` (58 lines)
- `addons/sale_purchase_project/i18n/es.po` (59 lines)
- `addons/sale_purchase_project/i18n/es_419.po` (58 lines)
- `addons/sale_purchase_project/i18n/et.po` (58 lines)
- `addons/sale_purchase_project/i18n/fa.po` (58 lines)
- `addons/sale_purchase_project/i18n/fi.po` (59 lines)
- `addons/sale_purchase_project/i18n/fr.po` (58 lines)
- `addons/sale_purchase_project/i18n/he.po` (59 lines)
- `addons/sale_purchase_project/i18n/hi.po` (58 lines)
- `addons/sale_purchase_project/i18n/hr.po` (59 lines)
- `addons/sale_purchase_project/i18n/hu.po` (58 lines)
- `addons/sale_purchase_project/i18n/id.po` (58 lines)
- `addons/sale_purchase_project/i18n/it.po` (58 lines)
- `addons/sale_purchase_project/i18n/ja.po` (58 lines)
- `addons/sale_purchase_project/i18n/kab.po` (58 lines)
- `addons/sale_purchase_project/i18n/ko.po` (58 lines)
- `addons/sale_purchase_project/i18n/ku.po` (58 lines)
- `addons/sale_purchase_project/i18n/lo.po` (57 lines)
- `addons/sale_purchase_project/i18n/lt.po` (60 lines)
- `addons/sale_purchase_project/i18n/lv.po` (58 lines)
- `addons/sale_purchase_project/i18n/mn.po` (58 lines)
- `addons/sale_purchase_project/i18n/my.po` (58 lines)
- `addons/sale_purchase_project/i18n/nb.po` (58 lines)
- `addons/sale_purchase_project/i18n/nl.po` (59 lines)
- `addons/sale_purchase_project/i18n/pl.po` (59 lines)
- `addons/sale_purchase_project/i18n/pt.po` (59 lines)
- `addons/sale_purchase_project/i18n/pt_BR.po` (61 lines)
- `addons/sale_purchase_project/i18n/ro.po` (59 lines)
- `addons/sale_purchase_project/i18n/ru.po` (59 lines)
- `addons/sale_purchase_project/i18n/sale_purchase_project.pot` (54 lines)
- `addons/sale_purchase_project/i18n/sk.po` (57 lines)
- `addons/sale_purchase_project/i18n/sl.po` (59 lines)
- `addons/sale_purchase_project/i18n/sr@latin.po` (59 lines)
- `addons/sale_purchase_project/i18n/sv.po` (59 lines)
- `addons/sale_purchase_project/i18n/th.po` (58 lines)
- `addons/sale_purchase_project/i18n/tr.po` (58 lines)
- `addons/sale_purchase_project/i18n/uk.po` (59 lines)
- `addons/sale_purchase_project/i18n/uz.po` (68 lines)
- `addons/sale_purchase_project/i18n/vi.po` (59 lines)
- `addons/sale_purchase_project/i18n/zh_CN.po` (60 lines)
- `addons/sale_purchase_project/i18n/zh_TW.po` (59 lines)
- `addons/sale_purchase_project/models/__init__.py` (4 lines)
- `addons/sale_purchase_project/models/account_analytic_line.py` (17 lines)
- `addons/sale_purchase_project/models/sale_order_line.py` (20 lines)
- `addons/sale_purchase_project/tests/__init__.py` (3 lines)
- `addons/sale_purchase_project/tests/test_sale_purchase_project.py` (67 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
