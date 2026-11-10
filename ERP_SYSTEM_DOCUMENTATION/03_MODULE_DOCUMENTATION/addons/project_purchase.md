# Module: project_purchase

- **Module ID:** MOD-484
- **Path:** `addons/project_purchase`
- **Manifest:** `addons/project_purchase/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Monitor purchase in project

No manifest description declared.

Declared dependencies: `purchase`, `project_account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 12 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "purchase",
    "project_account"
  ],
  "data": [
    "views/project_project.xml",
    "views/purchase_order.xml"
  ],
  "demo": [
    "data/project_purchase_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "project_purchase/static/src/product_catalog/kanban_record.js"
    ]
  }
}
```

### Representative source files

- `addons/project_purchase/__init__.py` (6 lines)
- `addons/project_purchase/__manifest__.py` (23 lines)
- `addons/project_purchase/controllers/__init__.py` (1 lines)
- `addons/project_purchase/controllers/catalog.py` (14 lines)
- `addons/project_purchase/data/project_purchase_demo.xml` (78 lines)
- `addons/project_purchase/i18n/ar.po` (92 lines)
- `addons/project_purchase/i18n/az.po` (89 lines)
- `addons/project_purchase/i18n/bg.po` (89 lines)
- `addons/project_purchase/i18n/bs.po` (91 lines)
- `addons/project_purchase/i18n/ca.po` (90 lines)
- `addons/project_purchase/i18n/cs.po` (91 lines)
- `addons/project_purchase/i18n/da.po` (90 lines)
- `addons/project_purchase/i18n/de.po` (91 lines)
- `addons/project_purchase/i18n/el.po` (90 lines)
- `addons/project_purchase/i18n/es.po` (92 lines)
- `addons/project_purchase/i18n/es_419.po` (92 lines)
- `addons/project_purchase/i18n/et.po` (90 lines)
- `addons/project_purchase/i18n/fa.po` (89 lines)
- `addons/project_purchase/i18n/fi.po` (91 lines)
- `addons/project_purchase/i18n/fr.po` (91 lines)
- `addons/project_purchase/i18n/he.po` (90 lines)
- `addons/project_purchase/i18n/hi.po` (89 lines)
- `addons/project_purchase/i18n/hr.po` (90 lines)
- `addons/project_purchase/i18n/hu.po` (90 lines)
- `addons/project_purchase/i18n/id.po` (91 lines)
- `addons/project_purchase/i18n/it.po` (91 lines)
- `addons/project_purchase/i18n/ja.po` (91 lines)
- `addons/project_purchase/i18n/kab.po` (90 lines)
- `addons/project_purchase/i18n/ko.po` (91 lines)
- `addons/project_purchase/i18n/ku.po` (89 lines)
- `addons/project_purchase/i18n/lo.po` (89 lines)
- `addons/project_purchase/i18n/lt.po` (91 lines)
- `addons/project_purchase/i18n/lv.po` (90 lines)
- `addons/project_purchase/i18n/mn.po` (89 lines)
- `addons/project_purchase/i18n/my.po` (90 lines)
- `addons/project_purchase/i18n/nb.po` (90 lines)
- `addons/project_purchase/i18n/nl.po` (91 lines)
- `addons/project_purchase/i18n/pl.po` (93 lines)
- `addons/project_purchase/i18n/project_purchase.pot` (86 lines)
- `addons/project_purchase/i18n/pt.po` (90 lines)
- `addons/project_purchase/i18n/pt_BR.po` (94 lines)
- `addons/project_purchase/i18n/ro.po` (91 lines)
- `addons/project_purchase/i18n/ru.po` (94 lines)
- `addons/project_purchase/i18n/sk.po` (89 lines)
- `addons/project_purchase/i18n/sl.po` (91 lines)
- `addons/project_purchase/i18n/sr@latin.po` (90 lines)
- `addons/project_purchase/i18n/sv.po` (91 lines)
- `addons/project_purchase/i18n/th.po` (91 lines)
- `addons/project_purchase/i18n/tr.po` (91 lines)
- `addons/project_purchase/i18n/uk.po` (90 lines)
- `addons/project_purchase/i18n/uz.po` (106 lines)
- `addons/project_purchase/i18n/vi.po` (91 lines)
- `addons/project_purchase/i18n/zh_CN.po` (91 lines)
- `addons/project_purchase/i18n/zh_TW.po` (93 lines)
- `addons/project_purchase/models/__init__.py` (5 lines)
- `addons/project_purchase/models/project_project.py` (57 lines)
- `addons/project_purchase/models/purchase_order.py` (9 lines)
- `addons/project_purchase/models/purchase_order_line.py` (35 lines)
- `addons/project_purchase/report/__init__.py` (2 lines)
- `addons/project_purchase/report/purchase_report.py` (19 lines)
- `addons/project_purchase/static/src/product_catalog/kanban_record.js` (12 lines)
- `addons/project_purchase/tests/__init__.py` (3 lines)
- `addons/project_purchase/tests/test_project_purchase.py` (131 lines)
- `addons/project_purchase/views/project_project.xml` (36 lines)
- `addons/project_purchase/views/purchase_order.xml` (14 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
