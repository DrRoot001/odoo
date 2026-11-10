# Module: mrp_product_expiry

- **Module ID:** MOD-381
- **Path:** `addons/mrp_product_expiry`
- **Manifest:** `addons/mrp_product_expiry/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Manufacturing Expiry


Technical module.
    

Declared dependencies: `mrp`, `product_expiry`.

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
    "mrp",
    "product_expiry"
  ],
  "data": [
    "wizard/confirm_expiry_view.xml"
  ]
}
```

### Representative source files

- `addons/mrp_product_expiry/__init__.py` (5 lines)
- `addons/mrp_product_expiry/__manifest__.py` (17 lines)
- `addons/mrp_product_expiry/i18n/ar.po` (100 lines)
- `addons/mrp_product_expiry/i18n/az.po` (92 lines)
- `addons/mrp_product_expiry/i18n/bg.po` (92 lines)
- `addons/mrp_product_expiry/i18n/bs.po` (94 lines)
- `addons/mrp_product_expiry/i18n/ca.po` (95 lines)
- `addons/mrp_product_expiry/i18n/cs.po` (94 lines)
- `addons/mrp_product_expiry/i18n/da.po` (99 lines)
- `addons/mrp_product_expiry/i18n/de.po` (101 lines)
- `addons/mrp_product_expiry/i18n/el.po` (93 lines)
- `addons/mrp_product_expiry/i18n/es.po` (102 lines)
- `addons/mrp_product_expiry/i18n/es_419.po` (99 lines)
- `addons/mrp_product_expiry/i18n/et.po` (98 lines)
- `addons/mrp_product_expiry/i18n/fa.po` (92 lines)
- `addons/mrp_product_expiry/i18n/fi.po` (100 lines)
- `addons/mrp_product_expiry/i18n/fr.po` (99 lines)
- `addons/mrp_product_expiry/i18n/he.po` (93 lines)
- `addons/mrp_product_expiry/i18n/hi.po` (92 lines)
- `addons/mrp_product_expiry/i18n/hr.po` (93 lines)
- `addons/mrp_product_expiry/i18n/hu.po` (93 lines)
- `addons/mrp_product_expiry/i18n/id.po` (99 lines)
- `addons/mrp_product_expiry/i18n/it.po` (99 lines)
- `addons/mrp_product_expiry/i18n/ja.po` (98 lines)
- `addons/mrp_product_expiry/i18n/kab.po` (93 lines)
- `addons/mrp_product_expiry/i18n/ko.po` (99 lines)
- `addons/mrp_product_expiry/i18n/ku.po` (92 lines)
- `addons/mrp_product_expiry/i18n/lo.po` (92 lines)
- `addons/mrp_product_expiry/i18n/lt.po` (94 lines)
- `addons/mrp_product_expiry/i18n/lv.po` (93 lines)
- `addons/mrp_product_expiry/i18n/mn.po` (92 lines)
- `addons/mrp_product_expiry/i18n/mrp_product_expiry.pot` (88 lines)
- `addons/mrp_product_expiry/i18n/my.po` (92 lines)
- `addons/mrp_product_expiry/i18n/nb.po` (93 lines)
- `addons/mrp_product_expiry/i18n/nl.po` (99 lines)
- `addons/mrp_product_expiry/i18n/pl.po` (100 lines)
- `addons/mrp_product_expiry/i18n/pt.po` (98 lines)
- `addons/mrp_product_expiry/i18n/pt_BR.po` (102 lines)
- `addons/mrp_product_expiry/i18n/ro.po` (99 lines)
- `addons/mrp_product_expiry/i18n/ru.po` (102 lines)
- `addons/mrp_product_expiry/i18n/sk.po` (92 lines)
- `addons/mrp_product_expiry/i18n/sl.po` (94 lines)
- `addons/mrp_product_expiry/i18n/sr@latin.po` (93 lines)
- `addons/mrp_product_expiry/i18n/sv.po` (101 lines)
- `addons/mrp_product_expiry/i18n/th.po` (98 lines)
- `addons/mrp_product_expiry/i18n/tr.po` (101 lines)
- `addons/mrp_product_expiry/i18n/uk.po` (93 lines)
- `addons/mrp_product_expiry/i18n/uz.po` (114 lines)
- `addons/mrp_product_expiry/i18n/vi.po` (98 lines)
- `addons/mrp_product_expiry/i18n/zh_CN.po` (98 lines)
- `addons/mrp_product_expiry/i18n/zh_TW.po` (100 lines)
- `addons/mrp_product_expiry/models/__init__.py` (4 lines)
- `addons/mrp_product_expiry/models/mrp_production.py` (39 lines)
- `addons/mrp_product_expiry/tests/__init__.py` (4 lines)
- `addons/mrp_product_expiry/tests/test_mrp_product_expiry.py` (109 lines)
- `addons/mrp_product_expiry/wizard/__init__.py` (4 lines)
- `addons/mrp_product_expiry/wizard/confirm_expiry.py` (43 lines)
- `addons/mrp_product_expiry/wizard/confirm_expiry_view.xml` (41 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
