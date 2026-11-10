# Module: project_purchase_stock

- **Module ID:** MOD-485
- **Path:** `addons/project_purchase_stock`
- **Manifest:** `addons/project_purchase_stock/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Add a project link between POs and their generated stock pickings.

Declared dependencies: `project_purchase`, `project_stock`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "project_purchase",
    "project_stock"
  ]
}
```

### Representative source files

- `addons/project_purchase_stock/__init__.py` (3 lines)
- `addons/project_purchase_stock/__manifest__.py` (11 lines)
- `addons/project_purchase_stock/i18n/ar.po` (61 lines)
- `addons/project_purchase_stock/i18n/az.po` (58 lines)
- `addons/project_purchase_stock/i18n/bg.po` (58 lines)
- `addons/project_purchase_stock/i18n/bs.po` (60 lines)
- `addons/project_purchase_stock/i18n/ca.po` (58 lines)
- `addons/project_purchase_stock/i18n/cs.po` (59 lines)
- `addons/project_purchase_stock/i18n/da.po` (58 lines)
- `addons/project_purchase_stock/i18n/de.po` (61 lines)
- `addons/project_purchase_stock/i18n/el.po` (58 lines)
- `addons/project_purchase_stock/i18n/es.po` (60 lines)
- `addons/project_purchase_stock/i18n/es_419.po` (61 lines)
- `addons/project_purchase_stock/i18n/et.po` (59 lines)
- `addons/project_purchase_stock/i18n/fa.po` (58 lines)
- `addons/project_purchase_stock/i18n/fi.po` (59 lines)
- `addons/project_purchase_stock/i18n/fr.po` (59 lines)
- `addons/project_purchase_stock/i18n/he.po` (59 lines)
- `addons/project_purchase_stock/i18n/hi.po` (58 lines)
- `addons/project_purchase_stock/i18n/hr.po` (59 lines)
- `addons/project_purchase_stock/i18n/hu.po` (58 lines)
- `addons/project_purchase_stock/i18n/id.po` (59 lines)
- `addons/project_purchase_stock/i18n/it.po` (59 lines)
- `addons/project_purchase_stock/i18n/ja.po` (59 lines)
- `addons/project_purchase_stock/i18n/kab.po` (59 lines)
- `addons/project_purchase_stock/i18n/ko.po` (59 lines)
- `addons/project_purchase_stock/i18n/ku.po` (58 lines)
- `addons/project_purchase_stock/i18n/lo.po` (58 lines)
- `addons/project_purchase_stock/i18n/lt.po` (60 lines)
- `addons/project_purchase_stock/i18n/lv.po` (59 lines)
- `addons/project_purchase_stock/i18n/mn.po` (58 lines)
- `addons/project_purchase_stock/i18n/my.po` (59 lines)
- `addons/project_purchase_stock/i18n/nb.po` (58 lines)
- `addons/project_purchase_stock/i18n/nl.po` (60 lines)
- `addons/project_purchase_stock/i18n/pl.po` (59 lines)
- `addons/project_purchase_stock/i18n/project_purchase_stock.pot` (55 lines)
- `addons/project_purchase_stock/i18n/pt.po` (58 lines)
- `addons/project_purchase_stock/i18n/pt_BR.po` (62 lines)
- `addons/project_purchase_stock/i18n/ro.po` (60 lines)
- `addons/project_purchase_stock/i18n/ru.po` (60 lines)
- `addons/project_purchase_stock/i18n/sk.po` (58 lines)
- `addons/project_purchase_stock/i18n/sl.po` (59 lines)
- `addons/project_purchase_stock/i18n/sr@latin.po` (59 lines)
- `addons/project_purchase_stock/i18n/sv.po` (59 lines)
- `addons/project_purchase_stock/i18n/th.po` (59 lines)
- `addons/project_purchase_stock/i18n/tr.po` (59 lines)
- `addons/project_purchase_stock/i18n/uk.po` (59 lines)
- `addons/project_purchase_stock/i18n/uz.po` (69 lines)
- `addons/project_purchase_stock/i18n/vi.po` (59 lines)
- `addons/project_purchase_stock/i18n/zh_CN.po` (59 lines)
- `addons/project_purchase_stock/i18n/zh_TW.po` (59 lines)
- `addons/project_purchase_stock/models/__init__.py` (5 lines)
- `addons/project_purchase_stock/models/purchase_order_line.py` (18 lines)
- `addons/project_purchase_stock/models/stock_move.py` (13 lines)
- `addons/project_purchase_stock/models/stock_rule.py` (20 lines)
- `addons/project_purchase_stock/tests/__init__.py` (2 lines)
- `addons/project_purchase_stock/tests/test_reordering_rule.py` (66 lines)
- `addons/project_purchase_stock/tests/test_subcontracting_project.py` (126 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
