# Module: project_stock

- **Module ID:** MOD-488
- **Path:** `addons/project_stock`
- **Manifest:** `addons/project_stock/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Link Stock pickings to Project

No manifest description declared.

Declared dependencies: `stock`, `project`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 5 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "stock",
    "project"
  ],
  "data": [
    "views/stock_picking_views.xml",
    "views/project_project_views.xml"
  ]
}
```

### Representative source files

- `addons/project_stock/__init__.py` (3 lines)
- `addons/project_stock/__manifest__.py` (15 lines)
- `addons/project_stock/i18n/ar.po` (79 lines)
- `addons/project_stock/i18n/az.po` (76 lines)
- `addons/project_stock/i18n/bg.po` (76 lines)
- `addons/project_stock/i18n/bs.po` (78 lines)
- `addons/project_stock/i18n/ca.po` (77 lines)
- `addons/project_stock/i18n/cs.po` (78 lines)
- `addons/project_stock/i18n/da.po` (77 lines)
- `addons/project_stock/i18n/de.po` (78 lines)
- `addons/project_stock/i18n/el.po` (77 lines)
- `addons/project_stock/i18n/es.po` (79 lines)
- `addons/project_stock/i18n/es_419.po` (79 lines)
- `addons/project_stock/i18n/et.po` (77 lines)
- `addons/project_stock/i18n/fa.po` (76 lines)
- `addons/project_stock/i18n/fi.po` (78 lines)
- `addons/project_stock/i18n/fr.po` (78 lines)
- `addons/project_stock/i18n/he.po` (77 lines)
- `addons/project_stock/i18n/hi.po` (76 lines)
- `addons/project_stock/i18n/hr.po` (77 lines)
- `addons/project_stock/i18n/hu.po` (77 lines)
- `addons/project_stock/i18n/id.po` (79 lines)
- `addons/project_stock/i18n/it.po` (78 lines)
- `addons/project_stock/i18n/ja.po` (79 lines)
- `addons/project_stock/i18n/kab.po` (77 lines)
- `addons/project_stock/i18n/ko.po` (78 lines)
- `addons/project_stock/i18n/ku.po` (76 lines)
- `addons/project_stock/i18n/lo.po` (76 lines)
- `addons/project_stock/i18n/lt.po` (78 lines)
- `addons/project_stock/i18n/lv.po` (77 lines)
- `addons/project_stock/i18n/mn.po` (76 lines)
- `addons/project_stock/i18n/my.po` (77 lines)
- `addons/project_stock/i18n/nb.po` (77 lines)
- `addons/project_stock/i18n/nl.po` (78 lines)
- `addons/project_stock/i18n/pl.po` (79 lines)
- `addons/project_stock/i18n/project_stock.pot` (73 lines)
- `addons/project_stock/i18n/pt.po` (77 lines)
- `addons/project_stock/i18n/pt_BR.po` (79 lines)
- `addons/project_stock/i18n/ro.po` (78 lines)
- `addons/project_stock/i18n/ru.po` (79 lines)
- `addons/project_stock/i18n/sk.po` (76 lines)
- `addons/project_stock/i18n/sl.po` (78 lines)
- `addons/project_stock/i18n/sr@latin.po` (77 lines)
- `addons/project_stock/i18n/sv.po` (78 lines)
- `addons/project_stock/i18n/th.po` (78 lines)
- `addons/project_stock/i18n/tr.po` (79 lines)
- `addons/project_stock/i18n/uk.po` (77 lines)
- `addons/project_stock/i18n/uz.po` (91 lines)
- `addons/project_stock/i18n/vi.po` (78 lines)
- `addons/project_stock/i18n/zh_CN.po` (78 lines)
- `addons/project_stock/i18n/zh_TW.po` (80 lines)
- `addons/project_stock/models/__init__.py` (4 lines)
- `addons/project_stock/models/project_project.py` (45 lines)
- `addons/project_stock/models/stock_picking.py` (9 lines)
- `addons/project_stock/views/project_project_views.xml` (56 lines)
- `addons/project_stock/views/stock_picking_views.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
