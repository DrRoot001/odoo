# Module: project_mrp_stock_landed_costs

- **Module ID:** MOD-483
- **Path:** `addons/project_mrp_stock_landed_costs`
- **Manifest:** `addons/project_mrp_stock_landed_costs/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Technical Bridge

No manifest description declared.

Declared dependencies: `project_mrp_account`, `mrp_landed_costs`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "project_mrp_account",
    "mrp_landed_costs"
  ]
}
```

### Representative source files

- `addons/project_mrp_stock_landed_costs/__init__.py` (3 lines)
- `addons/project_mrp_stock_landed_costs/__manifest__.py` (11 lines)
- `addons/project_mrp_stock_landed_costs/i18n/ar.po` (46 lines)
- `addons/project_mrp_stock_landed_costs/i18n/az.po` (44 lines)
- `addons/project_mrp_stock_landed_costs/i18n/bg.po` (44 lines)
- `addons/project_mrp_stock_landed_costs/i18n/bs.po` (46 lines)
- `addons/project_mrp_stock_landed_costs/i18n/ca.po` (44 lines)
- `addons/project_mrp_stock_landed_costs/i18n/cs.po` (45 lines)
- `addons/project_mrp_stock_landed_costs/i18n/da.po` (44 lines)
- `addons/project_mrp_stock_landed_costs/i18n/de.po` (45 lines)
- `addons/project_mrp_stock_landed_costs/i18n/el.po` (44 lines)
- `addons/project_mrp_stock_landed_costs/i18n/es.po` (45 lines)
- `addons/project_mrp_stock_landed_costs/i18n/es_419.po` (45 lines)
- `addons/project_mrp_stock_landed_costs/i18n/et.po` (45 lines)
- `addons/project_mrp_stock_landed_costs/i18n/fa.po` (44 lines)
- `addons/project_mrp_stock_landed_costs/i18n/fi.po` (45 lines)
- `addons/project_mrp_stock_landed_costs/i18n/fr.po` (45 lines)
- `addons/project_mrp_stock_landed_costs/i18n/he.po` (45 lines)
- `addons/project_mrp_stock_landed_costs/i18n/hi.po` (44 lines)
- `addons/project_mrp_stock_landed_costs/i18n/hr.po` (45 lines)
- `addons/project_mrp_stock_landed_costs/i18n/hu.po` (44 lines)
- `addons/project_mrp_stock_landed_costs/i18n/id.po` (45 lines)
- `addons/project_mrp_stock_landed_costs/i18n/it.po` (45 lines)
- `addons/project_mrp_stock_landed_costs/i18n/ja.po` (45 lines)
- `addons/project_mrp_stock_landed_costs/i18n/kab.po` (45 lines)
- `addons/project_mrp_stock_landed_costs/i18n/ko.po` (45 lines)
- `addons/project_mrp_stock_landed_costs/i18n/ku.po` (44 lines)
- `addons/project_mrp_stock_landed_costs/i18n/lo.po` (44 lines)
- `addons/project_mrp_stock_landed_costs/i18n/lt.po` (46 lines)
- `addons/project_mrp_stock_landed_costs/i18n/lv.po` (45 lines)
- `addons/project_mrp_stock_landed_costs/i18n/mn.po` (44 lines)
- `addons/project_mrp_stock_landed_costs/i18n/my.po` (44 lines)
- `addons/project_mrp_stock_landed_costs/i18n/nb.po` (44 lines)
- `addons/project_mrp_stock_landed_costs/i18n/nl.po` (46 lines)
- `addons/project_mrp_stock_landed_costs/i18n/pl.po` (45 lines)
- `addons/project_mrp_stock_landed_costs/i18n/project_mrp_stock_landed_costs.pot` (41 lines)
- `addons/project_mrp_stock_landed_costs/i18n/pt.po` (44 lines)
- `addons/project_mrp_stock_landed_costs/i18n/pt_BR.po` (46 lines)
- `addons/project_mrp_stock_landed_costs/i18n/ro.po` (46 lines)
- `addons/project_mrp_stock_landed_costs/i18n/ru.po` (46 lines)
- `addons/project_mrp_stock_landed_costs/i18n/sk.po` (44 lines)
- `addons/project_mrp_stock_landed_costs/i18n/sl.po` (45 lines)
- `addons/project_mrp_stock_landed_costs/i18n/sr@latin.po` (45 lines)
- `addons/project_mrp_stock_landed_costs/i18n/sv.po` (45 lines)
- `addons/project_mrp_stock_landed_costs/i18n/th.po` (45 lines)
- `addons/project_mrp_stock_landed_costs/i18n/tr.po` (45 lines)
- `addons/project_mrp_stock_landed_costs/i18n/uk.po` (45 lines)
- `addons/project_mrp_stock_landed_costs/i18n/uz.po` (54 lines)
- `addons/project_mrp_stock_landed_costs/i18n/vi.po` (45 lines)
- `addons/project_mrp_stock_landed_costs/i18n/zh_CN.po` (45 lines)
- `addons/project_mrp_stock_landed_costs/i18n/zh_TW.po` (45 lines)
- `addons/project_mrp_stock_landed_costs/models/__init__.py` (3 lines)
- `addons/project_mrp_stock_landed_costs/models/stock_landed_costs.py` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
