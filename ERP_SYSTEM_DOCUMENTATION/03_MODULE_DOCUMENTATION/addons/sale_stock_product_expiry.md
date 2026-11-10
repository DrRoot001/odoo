# Module: sale_stock_product_expiry

- **Module ID:** MOD-535
- **Path:** `addons/sale_stock_product_expiry`
- **Manifest:** `addons/sale_stock_product_expiry/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Modifications to the forecast widget on SO lines to show fresh stock, i.e. ignoring stock to be removed due to expiration.

Declared dependencies: `sale_stock`, `product_expiry`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "sale_stock",
    "product_expiry"
  ],
  "assets": {
    "web.assets_tests": [
      "sale_stock_product_expiry/static/tests/tours/*.js"
    ],
    "web.assets_backend": [
      "sale_stock_product_expiry/static/src/**/*"
    ]
  }
}
```

### Representative source files

- `addons/sale_stock_product_expiry/__init__.py` (3 lines)
- `addons/sale_stock_product_expiry/__manifest__.py` (17 lines)
- `addons/sale_stock_product_expiry/i18n/ar.po` (89 lines)
- `addons/sale_stock_product_expiry/i18n/az.po` (85 lines)
- `addons/sale_stock_product_expiry/i18n/bg.po` (85 lines)
- `addons/sale_stock_product_expiry/i18n/bs.po` (86 lines)
- `addons/sale_stock_product_expiry/i18n/ca.po` (88 lines)
- `addons/sale_stock_product_expiry/i18n/cs.po` (88 lines)
- `addons/sale_stock_product_expiry/i18n/da.po` (89 lines)
- `addons/sale_stock_product_expiry/i18n/de.po` (91 lines)
- `addons/sale_stock_product_expiry/i18n/el.po` (85 lines)
- `addons/sale_stock_product_expiry/i18n/es.po` (91 lines)
- `addons/sale_stock_product_expiry/i18n/es_419.po` (92 lines)
- `addons/sale_stock_product_expiry/i18n/et.po` (87 lines)
- `addons/sale_stock_product_expiry/i18n/fa.po` (85 lines)
- `addons/sale_stock_product_expiry/i18n/fi.po` (91 lines)
- `addons/sale_stock_product_expiry/i18n/fr.po` (90 lines)
- `addons/sale_stock_product_expiry/i18n/he.po` (86 lines)
- `addons/sale_stock_product_expiry/i18n/hi.po` (85 lines)
- `addons/sale_stock_product_expiry/i18n/hr.po` (86 lines)
- `addons/sale_stock_product_expiry/i18n/hu.po` (85 lines)
- `addons/sale_stock_product_expiry/i18n/id.po` (90 lines)
- `addons/sale_stock_product_expiry/i18n/it.po` (87 lines)
- `addons/sale_stock_product_expiry/i18n/ja.po` (87 lines)
- `addons/sale_stock_product_expiry/i18n/kab.po` (85 lines)
- `addons/sale_stock_product_expiry/i18n/ko.po` (88 lines)
- `addons/sale_stock_product_expiry/i18n/ku.po` (85 lines)
- `addons/sale_stock_product_expiry/i18n/lo.po` (84 lines)
- `addons/sale_stock_product_expiry/i18n/lt.po` (87 lines)
- `addons/sale_stock_product_expiry/i18n/lv.po` (85 lines)
- `addons/sale_stock_product_expiry/i18n/mn.po` (87 lines)
- `addons/sale_stock_product_expiry/i18n/my.po` (85 lines)
- `addons/sale_stock_product_expiry/i18n/nb.po` (85 lines)
- `addons/sale_stock_product_expiry/i18n/nl.po` (89 lines)
- `addons/sale_stock_product_expiry/i18n/pl.po` (90 lines)
- `addons/sale_stock_product_expiry/i18n/pt.po` (89 lines)
- `addons/sale_stock_product_expiry/i18n/pt_BR.po` (93 lines)
- `addons/sale_stock_product_expiry/i18n/ro.po` (89 lines)
- `addons/sale_stock_product_expiry/i18n/ru.po` (90 lines)
- `addons/sale_stock_product_expiry/i18n/sale_stock_product_expiry.pot` (81 lines)
- `addons/sale_stock_product_expiry/i18n/sk.po` (84 lines)
- `addons/sale_stock_product_expiry/i18n/sl.po` (86 lines)
- `addons/sale_stock_product_expiry/i18n/sr@latin.po` (86 lines)
- `addons/sale_stock_product_expiry/i18n/sv.po` (88 lines)
- `addons/sale_stock_product_expiry/i18n/th.po` (88 lines)
- `addons/sale_stock_product_expiry/i18n/tr.po` (90 lines)
- `addons/sale_stock_product_expiry/i18n/uk.po` (88 lines)
- `addons/sale_stock_product_expiry/i18n/uz.po` (103 lines)
- `addons/sale_stock_product_expiry/i18n/vi.po` (88 lines)
- `addons/sale_stock_product_expiry/i18n/zh_CN.po` (88 lines)
- `addons/sale_stock_product_expiry/i18n/zh_TW.po` (86 lines)
- `addons/sale_stock_product_expiry/models/__init__.py` (4 lines)
- `addons/sale_stock_product_expiry/models/account_move.py` (12 lines)
- `addons/sale_stock_product_expiry/models/sale_order_line.py` (16 lines)
- `addons/sale_stock_product_expiry/static/src/widgets/qty_at_date_widget.js` (27 lines)
- `addons/sale_stock_product_expiry/static/src/widgets/qty_at_date_widget.xml` (7 lines)
- `addons/sale_stock_product_expiry/static/tests/tours/perishable_qty_at_date_tour.js` (20 lines)
- `addons/sale_stock_product_expiry/tests/__init__.py` (4 lines)
- `addons/sale_stock_product_expiry/tests/test_account_move.py` (39 lines)
- `addons/sale_stock_product_expiry/tests/test_perishable_qty_at_date.py` (57 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
