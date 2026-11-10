# Module: purchase_alternative_sale

- **Module ID:** MOD-495
- **Path:** `addons/purchase_alternative_sale`
- **Manifest:** `addons/purchase_alternative_sale/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Bridge module for Purchase Alternative and Sales.

Declared dependencies: `purchase_alternative`, `sale_purchase`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
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
    "purchase_alternative",
    "sale_purchase"
  ]
}
```

### Representative source files

- `addons/purchase_alternative_sale/__init__.py` (3 lines)
- `addons/purchase_alternative_sale/__manifest__.py` (12 lines)
- `addons/purchase_alternative_sale/i18n/ar.po` (45 lines)
- `addons/purchase_alternative_sale/i18n/az.po` (44 lines)
- `addons/purchase_alternative_sale/i18n/bg.po` (44 lines)
- `addons/purchase_alternative_sale/i18n/bs.po` (45 lines)
- `addons/purchase_alternative_sale/i18n/ca.po` (44 lines)
- `addons/purchase_alternative_sale/i18n/cs.po` (44 lines)
- `addons/purchase_alternative_sale/i18n/da.po` (44 lines)
- `addons/purchase_alternative_sale/i18n/de.po` (45 lines)
- `addons/purchase_alternative_sale/i18n/el.po` (44 lines)
- `addons/purchase_alternative_sale/i18n/es.po` (45 lines)
- `addons/purchase_alternative_sale/i18n/es_419.po` (47 lines)
- `addons/purchase_alternative_sale/i18n/et.po` (45 lines)
- `addons/purchase_alternative_sale/i18n/fa.po` (44 lines)
- `addons/purchase_alternative_sale/i18n/fi.po` (46 lines)
- `addons/purchase_alternative_sale/i18n/fr.po` (46 lines)
- `addons/purchase_alternative_sale/i18n/he.po` (45 lines)
- `addons/purchase_alternative_sale/i18n/hi.po` (44 lines)
- `addons/purchase_alternative_sale/i18n/hr.po` (45 lines)
- `addons/purchase_alternative_sale/i18n/hu.po` (44 lines)
- `addons/purchase_alternative_sale/i18n/id.po` (45 lines)
- `addons/purchase_alternative_sale/i18n/it.po` (46 lines)
- `addons/purchase_alternative_sale/i18n/ja.po` (45 lines)
- `addons/purchase_alternative_sale/i18n/kab.po` (44 lines)
- `addons/purchase_alternative_sale/i18n/ko.po` (45 lines)
- `addons/purchase_alternative_sale/i18n/ku.po` (44 lines)
- `addons/purchase_alternative_sale/i18n/lo.po` (44 lines)
- `addons/purchase_alternative_sale/i18n/lt.po` (46 lines)
- `addons/purchase_alternative_sale/i18n/lv.po` (45 lines)
- `addons/purchase_alternative_sale/i18n/mn.po` (44 lines)
- `addons/purchase_alternative_sale/i18n/my.po` (44 lines)
- `addons/purchase_alternative_sale/i18n/nb.po` (44 lines)
- `addons/purchase_alternative_sale/i18n/nl.po` (45 lines)
- `addons/purchase_alternative_sale/i18n/pl.po` (45 lines)
- `addons/purchase_alternative_sale/i18n/pt.po` (44 lines)
- `addons/purchase_alternative_sale/i18n/pt_BR.po` (47 lines)
- `addons/purchase_alternative_sale/i18n/purchase_alternative_sale.pot` (41 lines)
- `addons/purchase_alternative_sale/i18n/ro.po` (45 lines)
- `addons/purchase_alternative_sale/i18n/ru.po` (45 lines)
- `addons/purchase_alternative_sale/i18n/sk.po` (44 lines)
- `addons/purchase_alternative_sale/i18n/sl.po` (45 lines)
- `addons/purchase_alternative_sale/i18n/sr@latin.po` (45 lines)
- `addons/purchase_alternative_sale/i18n/sv.po` (45 lines)
- `addons/purchase_alternative_sale/i18n/th.po` (45 lines)
- `addons/purchase_alternative_sale/i18n/tr.po` (44 lines)
- `addons/purchase_alternative_sale/i18n/uk.po` (45 lines)
- `addons/purchase_alternative_sale/i18n/uz.po` (44 lines)
- `addons/purchase_alternative_sale/i18n/vi.po` (44 lines)
- `addons/purchase_alternative_sale/i18n/zh_CN.po` (45 lines)
- `addons/purchase_alternative_sale/i18n/zh_TW.po` (44 lines)
- `addons/purchase_alternative_sale/tests/__init__.py` (3 lines)
- `addons/purchase_alternative_sale/tests/test_purchase_alternative_sale.py` (60 lines)
- `addons/purchase_alternative_sale/wizard/__init__.py` (3 lines)
- `addons/purchase_alternative_sale/wizard/purchase_alternative_create.py` (14 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
