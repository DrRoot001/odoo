# Module: purchase_alternative_stock

- **Module ID:** MOD-496
- **Path:** `addons/purchase_alternative_stock`
- **Manifest:** `addons/purchase_alternative_stock/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

No manifest description declared.

Declared dependencies: `purchase_alternative`, `purchase_stock`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
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
    "purchase_alternative",
    "purchase_stock"
  ],
  "data": [
    "views/purchase_views.xml"
  ]
}
```

### Representative source files

- `addons/purchase_alternative_stock/__init__.py` (4 lines)
- `addons/purchase_alternative_stock/__manifest__.py` (15 lines)
- `addons/purchase_alternative_stock/i18n/ar.po` (60 lines)
- `addons/purchase_alternative_stock/i18n/az.po` (59 lines)
- `addons/purchase_alternative_stock/i18n/bg.po` (59 lines)
- `addons/purchase_alternative_stock/i18n/bs.po` (60 lines)
- `addons/purchase_alternative_stock/i18n/ca.po` (59 lines)
- `addons/purchase_alternative_stock/i18n/cs.po` (59 lines)
- `addons/purchase_alternative_stock/i18n/da.po` (59 lines)
- `addons/purchase_alternative_stock/i18n/de.po` (60 lines)
- `addons/purchase_alternative_stock/i18n/el.po` (59 lines)
- `addons/purchase_alternative_stock/i18n/es.po` (60 lines)
- `addons/purchase_alternative_stock/i18n/es_419.po` (62 lines)
- `addons/purchase_alternative_stock/i18n/et.po` (60 lines)
- `addons/purchase_alternative_stock/i18n/fa.po` (59 lines)
- `addons/purchase_alternative_stock/i18n/fi.po` (60 lines)
- `addons/purchase_alternative_stock/i18n/fr.po` (61 lines)
- `addons/purchase_alternative_stock/i18n/he.po` (60 lines)
- `addons/purchase_alternative_stock/i18n/hi.po` (59 lines)
- `addons/purchase_alternative_stock/i18n/hr.po` (60 lines)
- `addons/purchase_alternative_stock/i18n/hu.po` (59 lines)
- `addons/purchase_alternative_stock/i18n/id.po` (60 lines)
- `addons/purchase_alternative_stock/i18n/it.po` (61 lines)
- `addons/purchase_alternative_stock/i18n/ja.po` (60 lines)
- `addons/purchase_alternative_stock/i18n/kab.po` (59 lines)
- `addons/purchase_alternative_stock/i18n/ko.po` (60 lines)
- `addons/purchase_alternative_stock/i18n/ku.po` (59 lines)
- `addons/purchase_alternative_stock/i18n/lo.po` (59 lines)
- `addons/purchase_alternative_stock/i18n/lt.po` (61 lines)
- `addons/purchase_alternative_stock/i18n/lv.po` (60 lines)
- `addons/purchase_alternative_stock/i18n/mn.po` (59 lines)
- `addons/purchase_alternative_stock/i18n/my.po` (59 lines)
- `addons/purchase_alternative_stock/i18n/nb.po` (59 lines)
- `addons/purchase_alternative_stock/i18n/nl.po` (60 lines)
- `addons/purchase_alternative_stock/i18n/pl.po` (60 lines)
- `addons/purchase_alternative_stock/i18n/pt.po` (59 lines)
- `addons/purchase_alternative_stock/i18n/pt_BR.po` (61 lines)
- `addons/purchase_alternative_stock/i18n/purchase_alternative_stock.pot` (56 lines)
- `addons/purchase_alternative_stock/i18n/ro.po` (60 lines)
- `addons/purchase_alternative_stock/i18n/ru.po` (60 lines)
- `addons/purchase_alternative_stock/i18n/sk.po` (59 lines)
- `addons/purchase_alternative_stock/i18n/sl.po` (60 lines)
- `addons/purchase_alternative_stock/i18n/sr@latin.po` (60 lines)
- `addons/purchase_alternative_stock/i18n/sv.po` (60 lines)
- `addons/purchase_alternative_stock/i18n/th.po` (60 lines)
- `addons/purchase_alternative_stock/i18n/tr.po` (59 lines)
- `addons/purchase_alternative_stock/i18n/uk.po` (60 lines)
- `addons/purchase_alternative_stock/i18n/uz.po` (59 lines)
- `addons/purchase_alternative_stock/i18n/vi.po` (59 lines)
- `addons/purchase_alternative_stock/i18n/zh_CN.po` (60 lines)
- `addons/purchase_alternative_stock/i18n/zh_TW.po` (59 lines)
- `addons/purchase_alternative_stock/models/__init__.py` (3 lines)
- `addons/purchase_alternative_stock/models/purchase.py` (23 lines)
- `addons/purchase_alternative_stock/tests/__init__.py` (3 lines)
- `addons/purchase_alternative_stock/tests/test_purchase_alternative_stock.py` (141 lines)
- `addons/purchase_alternative_stock/views/purchase_views.xml` (24 lines)
- `addons/purchase_alternative_stock/wizard/__init__.py` (1 lines)
- `addons/purchase_alternative_stock/wizard/purchase_alternative_create.py` (23 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
