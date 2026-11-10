# Module: mrp_landed_costs

- **Module ID:** MOD-380
- **Path:** `addons/mrp_landed_costs`
- **Manifest:** `addons/mrp_landed_costs/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Landed Costs on Manufacturing Order


This module allows you to easily add extra costs on manufacturing order
and decide the split of these costs among their stock moves in order to
take them into account in your stock valuation.
    

Declared dependencies: `stock_landed_costs`, `mrp`.

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
    "stock_landed_costs",
    "mrp"
  ],
  "data": [
    "views/stock_landed_cost_views.xml"
  ]
}
```

### Representative source files

- `addons/mrp_landed_costs/__init__.py` (4 lines)
- `addons/mrp_landed_costs/__manifest__.py` (19 lines)
- `addons/mrp_landed_costs/i18n/ar.po` (83 lines)
- `addons/mrp_landed_costs/i18n/az.po` (80 lines)
- `addons/mrp_landed_costs/i18n/bg.po` (80 lines)
- `addons/mrp_landed_costs/i18n/bs.po` (82 lines)
- `addons/mrp_landed_costs/i18n/ca.po` (81 lines)
- `addons/mrp_landed_costs/i18n/cs.po` (82 lines)
- `addons/mrp_landed_costs/i18n/da.po` (81 lines)
- `addons/mrp_landed_costs/i18n/de.po` (88 lines)
- `addons/mrp_landed_costs/i18n/el.po` (81 lines)
- `addons/mrp_landed_costs/i18n/es.po` (83 lines)
- `addons/mrp_landed_costs/i18n/es_419.po` (83 lines)
- `addons/mrp_landed_costs/i18n/et.po` (81 lines)
- `addons/mrp_landed_costs/i18n/fa.po` (80 lines)
- `addons/mrp_landed_costs/i18n/fi.po` (87 lines)
- `addons/mrp_landed_costs/i18n/fr.po` (82 lines)
- `addons/mrp_landed_costs/i18n/he.po` (81 lines)
- `addons/mrp_landed_costs/i18n/hi.po` (80 lines)
- `addons/mrp_landed_costs/i18n/hr.po` (81 lines)
- `addons/mrp_landed_costs/i18n/hu.po` (81 lines)
- `addons/mrp_landed_costs/i18n/id.po` (83 lines)
- `addons/mrp_landed_costs/i18n/it.po` (88 lines)
- `addons/mrp_landed_costs/i18n/ja.po` (82 lines)
- `addons/mrp_landed_costs/i18n/kab.po` (81 lines)
- `addons/mrp_landed_costs/i18n/ko.po` (82 lines)
- `addons/mrp_landed_costs/i18n/ku.po` (80 lines)
- `addons/mrp_landed_costs/i18n/lo.po` (80 lines)
- `addons/mrp_landed_costs/i18n/lt.po` (82 lines)
- `addons/mrp_landed_costs/i18n/lv.po` (81 lines)
- `addons/mrp_landed_costs/i18n/mn.po` (80 lines)
- `addons/mrp_landed_costs/i18n/mrp_landed_costs.pot` (77 lines)
- `addons/mrp_landed_costs/i18n/my.po` (80 lines)
- `addons/mrp_landed_costs/i18n/nb.po` (81 lines)
- `addons/mrp_landed_costs/i18n/nl.po` (82 lines)
- `addons/mrp_landed_costs/i18n/pl.po` (83 lines)
- `addons/mrp_landed_costs/i18n/pt.po` (81 lines)
- `addons/mrp_landed_costs/i18n/pt_BR.po` (89 lines)
- `addons/mrp_landed_costs/i18n/ro.po` (82 lines)
- `addons/mrp_landed_costs/i18n/ru.po` (84 lines)
- `addons/mrp_landed_costs/i18n/sk.po` (80 lines)
- `addons/mrp_landed_costs/i18n/sl.po` (82 lines)
- `addons/mrp_landed_costs/i18n/sr@latin.po` (81 lines)
- `addons/mrp_landed_costs/i18n/sv.po` (82 lines)
- `addons/mrp_landed_costs/i18n/th.po` (82 lines)
- `addons/mrp_landed_costs/i18n/tr.po` (81 lines)
- `addons/mrp_landed_costs/i18n/uk.po` (81 lines)
- `addons/mrp_landed_costs/i18n/uz.po` (94 lines)
- `addons/mrp_landed_costs/i18n/vi.po` (82 lines)
- `addons/mrp_landed_costs/i18n/zh_CN.po` (87 lines)
- `addons/mrp_landed_costs/i18n/zh_TW.po` (84 lines)
- `addons/mrp_landed_costs/models/__init__.py` (4 lines)
- `addons/mrp_landed_costs/models/stock_landed_cost.py` (53 lines)
- `addons/mrp_landed_costs/tests/__init__.py` (4 lines)
- `addons/mrp_landed_costs/tests/test_stock_landed_costs_mrp.py` (222 lines)
- `addons/mrp_landed_costs/views/stock_landed_cost_views.xml` (28 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
