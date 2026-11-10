# Module: mrp_subcontracting_dropshipping

- **Module ID:** MOD-385
- **Path:** `addons/mrp_subcontracting_dropshipping`
- **Manifest:** `addons/mrp_subcontracting_dropshipping/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This bridge module allows to manage subcontracting with the dropshipping module.
    

Declared dependencies: `mrp_subcontracting`, `stock_dropshipping`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 18 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 10 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mrp_subcontracting",
    "stock_dropshipping"
  ],
  "data": [
    "data/mrp_subcontracting_dropshipping_data.xml",
    "views/purchase_order_views.xml"
  ]
}
```

### Representative source files

- `addons/mrp_subcontracting_dropshipping/__init__.py` (5 lines)
- `addons/mrp_subcontracting_dropshipping/__manifest__.py` (19 lines)
- `addons/mrp_subcontracting_dropshipping/data/mrp_subcontracting_dropshipping_data.xml` (15 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/ar.po` (140 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/az.po` (136 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/bg.po` (136 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/bs.po` (138 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/ca.po` (137 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/cs.po` (139 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/da.po` (137 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/de.po` (143 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/el.po` (137 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/es.po` (144 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/es_419.po` (141 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/et.po` (137 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/fa.po` (136 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/fi.po` (141 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/fr.po` (140 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/he.po` (137 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/hi.po` (136 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/hr.po` (137 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/hu.po` (137 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/id.po` (139 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/it.po` (143 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/ja.po` (138 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/kab.po` (137 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/ko.po` (138 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/ku.po` (136 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/lo.po` (136 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/lt.po` (138 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/lv.po` (137 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/mn.po` (136 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/mrp_subcontracting_dropshipping.pot` (132 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/my.po` (137 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/nb.po` (137 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/nl.po` (138 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/pl.po` (140 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/pt.po` (137 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/pt_BR.po` (143 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/ro.po` (139 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/ru.po` (141 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/sk.po` (136 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/sl.po` (138 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/sr@latin.po` (137 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/sv.po` (138 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/th.po` (138 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/tr.po` (139 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/uk.po` (137 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/uz.po` (161 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/vi.po` (138 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/zh_CN.po` (138 lines)
- `addons/mrp_subcontracting_dropshipping/i18n/zh_TW.po` (140 lines)
- `addons/mrp_subcontracting_dropshipping/models/__init__.py` (12 lines)
- `addons/mrp_subcontracting_dropshipping/models/account_move_line.py` (14 lines)
- `addons/mrp_subcontracting_dropshipping/models/purchase.py` (44 lines)
- `addons/mrp_subcontracting_dropshipping/models/res_company.py` (105 lines)
- `addons/mrp_subcontracting_dropshipping/models/stock_move.py` (66 lines)
- `addons/mrp_subcontracting_dropshipping/models/stock_orderpoint.py` (14 lines)
- `addons/mrp_subcontracting_dropshipping/models/stock_picking.py` (34 lines)
- `addons/mrp_subcontracting_dropshipping/models/stock_replenish_mixin.py` (12 lines)
- `addons/mrp_subcontracting_dropshipping/models/stock_rule.py` (23 lines)
- `addons/mrp_subcontracting_dropshipping/models/stock_warehouse.py` (89 lines)
- `addons/mrp_subcontracting_dropshipping/report/__init__.py` (3 lines)
- `addons/mrp_subcontracting_dropshipping/report/stock_traceability.py` (15 lines)
- `addons/mrp_subcontracting_dropshipping/tests/__init__.py` (6 lines)
- `addons/mrp_subcontracting_dropshipping/tests/test_anglo_saxon_valuation.py` (323 lines)
- `addons/mrp_subcontracting_dropshipping/tests/test_purchase_subcontracting.py` (653 lines)
- `addons/mrp_subcontracting_dropshipping/tests/test_sale_dropshipping.py` (387 lines)
- `addons/mrp_subcontracting_dropshipping/views/purchase_order_views.xml` (16 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
