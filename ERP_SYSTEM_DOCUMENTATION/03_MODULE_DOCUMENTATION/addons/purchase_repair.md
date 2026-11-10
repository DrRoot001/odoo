# Module: purchase_repair

- **Module ID:** MOD-500
- **Path:** `addons/purchase_repair`
- **Manifest:** `addons/purchase_repair/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Keep track of linked purchase and repair orders

No manifest description declared.

Declared dependencies: `repair`, `purchase_stock`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "repair",
    "purchase_stock"
  ],
  "data": [
    "views/purchase_views.xml",
    "views/repair_views.xml"
  ]
}
```

### Representative source files

- `addons/purchase_repair/__init__.py` (3 lines)
- `addons/purchase_repair/__manifest__.py` (15 lines)
- `addons/purchase_repair/i18n/ar.po` (82 lines)
- `addons/purchase_repair/i18n/az.po` (80 lines)
- `addons/purchase_repair/i18n/bg.po` (80 lines)
- `addons/purchase_repair/i18n/bs.po` (81 lines)
- `addons/purchase_repair/i18n/ca.po` (81 lines)
- `addons/purchase_repair/i18n/cs.po` (81 lines)
- `addons/purchase_repair/i18n/da.po` (82 lines)
- `addons/purchase_repair/i18n/de.po` (81 lines)
- `addons/purchase_repair/i18n/el.po` (81 lines)
- `addons/purchase_repair/i18n/es.po` (83 lines)
- `addons/purchase_repair/i18n/es_419.po` (81 lines)
- `addons/purchase_repair/i18n/et.po` (80 lines)
- `addons/purchase_repair/i18n/fa.po` (80 lines)
- `addons/purchase_repair/i18n/fi.po` (81 lines)
- `addons/purchase_repair/i18n/fr.po` (81 lines)
- `addons/purchase_repair/i18n/he.po` (81 lines)
- `addons/purchase_repair/i18n/hi.po` (80 lines)
- `addons/purchase_repair/i18n/hr.po` (81 lines)
- `addons/purchase_repair/i18n/hu.po` (81 lines)
- `addons/purchase_repair/i18n/id.po` (81 lines)
- `addons/purchase_repair/i18n/it.po` (81 lines)
- `addons/purchase_repair/i18n/ja.po` (81 lines)
- `addons/purchase_repair/i18n/kab.po` (80 lines)
- `addons/purchase_repair/i18n/ko.po` (82 lines)
- `addons/purchase_repair/i18n/ku.po` (80 lines)
- `addons/purchase_repair/i18n/lo.po` (79 lines)
- `addons/purchase_repair/i18n/lt.po` (82 lines)
- `addons/purchase_repair/i18n/lv.po` (80 lines)
- `addons/purchase_repair/i18n/mn.po` (80 lines)
- `addons/purchase_repair/i18n/my.po` (80 lines)
- `addons/purchase_repair/i18n/nb.po` (81 lines)
- `addons/purchase_repair/i18n/nl.po` (81 lines)
- `addons/purchase_repair/i18n/pl.po` (83 lines)
- `addons/purchase_repair/i18n/pt.po` (82 lines)
- `addons/purchase_repair/i18n/pt_BR.po` (82 lines)
- `addons/purchase_repair/i18n/purchase_repair.pot` (76 lines)
- `addons/purchase_repair/i18n/ro.po` (81 lines)
- `addons/purchase_repair/i18n/ru.po` (83 lines)
- `addons/purchase_repair/i18n/sk.po` (79 lines)
- `addons/purchase_repair/i18n/sl.po` (82 lines)
- `addons/purchase_repair/i18n/sr@latin.po` (81 lines)
- `addons/purchase_repair/i18n/sv.po` (83 lines)
- `addons/purchase_repair/i18n/th.po` (82 lines)
- `addons/purchase_repair/i18n/tr.po` (80 lines)
- `addons/purchase_repair/i18n/uk.po` (81 lines)
- `addons/purchase_repair/i18n/uz.po` (96 lines)
- `addons/purchase_repair/i18n/vi.po` (82 lines)
- `addons/purchase_repair/i18n/zh_CN.po` (82 lines)
- `addons/purchase_repair/i18n/zh_TW.po` (83 lines)
- `addons/purchase_repair/models/__init__.py` (4 lines)
- `addons/purchase_repair/models/purchase_order.py` (33 lines)
- `addons/purchase_repair/models/repair_order.py` (33 lines)
- `addons/purchase_repair/tests/__init__.py` (3 lines)
- `addons/purchase_repair/tests/test_repair_purchase_flow.py` (123 lines)
- `addons/purchase_repair/views/purchase_views.xml` (20 lines)
- `addons/purchase_repair/views/repair_views.xml` (20 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
