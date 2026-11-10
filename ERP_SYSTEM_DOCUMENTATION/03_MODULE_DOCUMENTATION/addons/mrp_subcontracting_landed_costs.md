# Module: mrp_subcontracting_landed_costs

- **Module ID:** MOD-386
- **Path:** `addons/mrp_subcontracting_landed_costs`
- **Manifest:** `addons/mrp_subcontracting_landed_costs/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Advanced views to manage landed cost for subcontracting orders


This module allows users to more easily identify subcontracting orders when applying landed costs,
by also displaying the associated picking reference in the search view.
    

Declared dependencies: `mrp_landed_costs`, `mrp_subcontracting`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mrp_landed_costs",
    "mrp_subcontracting"
  ],
  "data": [
    "views/stock_landed_cost_views.xml"
  ]
}
```

### Representative source files

- `addons/mrp_subcontracting_landed_costs/__init__.py` (3 lines)
- `addons/mrp_subcontracting_landed_costs/__manifest__.py` (18 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/ar.po` (56 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/az.po` (57 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/bg.po` (57 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/bs.po` (57 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/ca.po` (57 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/cs.po` (57 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/da.po` (56 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/de.po` (61 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/el.po` (56 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/es.po` (61 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/es_419.po` (54 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/et.po` (57 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/fa.po` (57 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/fi.po` (58 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/fr.po` (54 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/he.po` (58 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/hi.po` (56 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/hr.po` (58 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/hu.po` (57 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/id.po` (54 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/it.po` (58 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/ja.po` (54 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/kab.po` (57 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/ko.po` (57 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/ku.po` (55 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/lo.po` (57 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/lt.po` (59 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/lv.po` (57 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/mn.po` (57 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/mrp_subcontracting_landed_costs.pot` (49 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/my.po` (56 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/nb.po` (56 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/nl.po` (54 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/pl.po` (55 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/pt.po` (57 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/pt_BR.po` (63 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/ro.po` (58 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/ru.po` (56 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/sk.po` (57 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/sl.po` (58 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/sr@latin.po` (57 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/sv.po` (54 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/th.po` (54 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/tr.po` (57 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/uk.po` (58 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/uz.po` (53 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/vi.po` (57 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/zh_CN.po` (58 lines)
- `addons/mrp_subcontracting_landed_costs/i18n/zh_TW.po` (54 lines)
- `addons/mrp_subcontracting_landed_costs/models/__init__.py` (3 lines)
- `addons/mrp_subcontracting_landed_costs/models/stock_landed_cost.py` (18 lines)
- `addons/mrp_subcontracting_landed_costs/tests/__init__.py` (1 lines)
- `addons/mrp_subcontracting_landed_costs/tests/test_subcontracting_landed_costs.py` (210 lines)
- `addons/mrp_subcontracting_landed_costs/views/stock_landed_cost_views.xml` (16 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
