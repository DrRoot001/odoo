# Module: purchase_requisition_stock

- **Module ID:** MOD-502
- **Path:** `addons/purchase_requisition_stock`
- **Manifest:** `addons/purchase_requisition_stock/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

No manifest description declared.

Declared dependencies: `purchase_requisition`, `purchase_stock`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "purchase_requisition",
    "purchase_stock"
  ],
  "data": [
    "data/purchase_requisition_stock_data.xml",
    "views/purchase_requisition_views.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/purchase_requisition_stock/__init__.py` (3 lines)
- `addons/purchase_requisition_stock/__manifest__.py` (17 lines)
- `addons/purchase_requisition_stock/data/purchase_requisition_stock_data.xml` (8 lines)
- `addons/purchase_requisition_stock/i18n/ar.po` (93 lines)
- `addons/purchase_requisition_stock/i18n/az.po` (88 lines)
- `addons/purchase_requisition_stock/i18n/bg.po` (88 lines)
- `addons/purchase_requisition_stock/i18n/bs.po` (89 lines)
- `addons/purchase_requisition_stock/i18n/ca.po` (89 lines)
- `addons/purchase_requisition_stock/i18n/cs.po` (94 lines)
- `addons/purchase_requisition_stock/i18n/da.po` (93 lines)
- `addons/purchase_requisition_stock/i18n/de.po` (93 lines)
- `addons/purchase_requisition_stock/i18n/el.po` (89 lines)
- `addons/purchase_requisition_stock/i18n/es.po` (93 lines)
- `addons/purchase_requisition_stock/i18n/es_419.po` (88 lines)
- `addons/purchase_requisition_stock/i18n/et.po` (88 lines)
- `addons/purchase_requisition_stock/i18n/fa.po` (88 lines)
- `addons/purchase_requisition_stock/i18n/fi.po` (89 lines)
- `addons/purchase_requisition_stock/i18n/fr.po` (94 lines)
- `addons/purchase_requisition_stock/i18n/he.po` (96 lines)
- `addons/purchase_requisition_stock/i18n/hi.po` (88 lines)
- `addons/purchase_requisition_stock/i18n/hr.po` (93 lines)
- `addons/purchase_requisition_stock/i18n/hu.po` (94 lines)
- `addons/purchase_requisition_stock/i18n/id.po` (90 lines)
- `addons/purchase_requisition_stock/i18n/it.po` (93 lines)
- `addons/purchase_requisition_stock/i18n/ja.po` (89 lines)
- `addons/purchase_requisition_stock/i18n/kab.po` (88 lines)
- `addons/purchase_requisition_stock/i18n/ko.po` (88 lines)
- `addons/purchase_requisition_stock/i18n/ku.po` (88 lines)
- `addons/purchase_requisition_stock/i18n/lo.po` (87 lines)
- `addons/purchase_requisition_stock/i18n/lt.po` (96 lines)
- `addons/purchase_requisition_stock/i18n/lv.po` (88 lines)
- `addons/purchase_requisition_stock/i18n/mn.po` (92 lines)
- `addons/purchase_requisition_stock/i18n/my.po` (89 lines)
- `addons/purchase_requisition_stock/i18n/nb.po` (92 lines)
- `addons/purchase_requisition_stock/i18n/nl.po` (93 lines)
- `addons/purchase_requisition_stock/i18n/pl.po` (96 lines)
- `addons/purchase_requisition_stock/i18n/pt.po` (97 lines)
- `addons/purchase_requisition_stock/i18n/pt_BR.po` (94 lines)
- `addons/purchase_requisition_stock/i18n/purchase_requisition_stock.pot` (84 lines)
- `addons/purchase_requisition_stock/i18n/ro.po` (93 lines)
- `addons/purchase_requisition_stock/i18n/ru.po` (93 lines)
- `addons/purchase_requisition_stock/i18n/sk.po` (87 lines)
- `addons/purchase_requisition_stock/i18n/sl.po` (89 lines)
- `addons/purchase_requisition_stock/i18n/sr@latin.po` (89 lines)
- `addons/purchase_requisition_stock/i18n/sv.po` (89 lines)
- `addons/purchase_requisition_stock/i18n/th.po` (88 lines)
- `addons/purchase_requisition_stock/i18n/tr.po` (96 lines)
- `addons/purchase_requisition_stock/i18n/uk.po` (95 lines)
- `addons/purchase_requisition_stock/i18n/uz.po` (106 lines)
- `addons/purchase_requisition_stock/i18n/vi.po` (94 lines)
- `addons/purchase_requisition_stock/i18n/zh_CN.po` (92 lines)
- `addons/purchase_requisition_stock/i18n/zh_TW.po` (90 lines)
- `addons/purchase_requisition_stock/models/__init__.py` (5 lines)
- `addons/purchase_requisition_stock/models/purchase.py` (13 lines)
- `addons/purchase_requisition_stock/models/purchase_requisition.py` (30 lines)
- `addons/purchase_requisition_stock/models/stock.py` (46 lines)
- `addons/purchase_requisition_stock/security/ir.access.csv` (3 lines)
- `addons/purchase_requisition_stock/tests/__init__.py` (3 lines)
- `addons/purchase_requisition_stock/tests/test_purchase_requisition_stock.py` (186 lines)
- `addons/purchase_requisition_stock/views/purchase_requisition_views.xml` (15 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
