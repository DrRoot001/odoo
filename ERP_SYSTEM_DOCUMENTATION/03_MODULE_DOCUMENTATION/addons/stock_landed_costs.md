# Module: stock_landed_costs

- **Module ID:** MOD-564
- **Path:** `addons/stock_landed_costs`
- **Manifest:** `addons/stock_landed_costs/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Landed Costs


Landed Costs Management
=======================
This module allows you to easily add extra costs on pickings and decide the split of these costs among their stock moves in order to take them into account in your stock valuation.
    

Declared dependencies: `stock_account`, `purchase_stock`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 18 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 8 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 8 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "stock_account",
    "purchase_stock"
  ],
  "data": [
    "data/stock_landed_cost_data.xml",
    "views/account_move_views.xml",
    "views/product_views.xml",
    "views/stock_landed_cost_views.xml",
    "views/res_config_settings_views.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/stock_landed_costs/__init__.py` (4 lines)
- `addons/stock_landed_costs/__manifest__.py` (25 lines)
- `addons/stock_landed_costs/data/stock_landed_cost_data.xml` (19 lines)
- `addons/stock_landed_costs/i18n/af.po` (776 lines)
- `addons/stock_landed_costs/i18n/am.po` (772 lines)
- `addons/stock_landed_costs/i18n/ar.po` (802 lines)
- `addons/stock_landed_costs/i18n/az.po` (792 lines)
- `addons/stock_landed_costs/i18n/bg.po` (805 lines)
- `addons/stock_landed_costs/i18n/bs.po` (783 lines)
- `addons/stock_landed_costs/i18n/ca.po` (813 lines)
- `addons/stock_landed_costs/i18n/cs.po` (799 lines)
- `addons/stock_landed_costs/i18n/da.po` (794 lines)
- `addons/stock_landed_costs/i18n/de.po` (823 lines)
- `addons/stock_landed_costs/i18n/el.po` (794 lines)
- `addons/stock_landed_costs/i18n/es.po` (813 lines)
- `addons/stock_landed_costs/i18n/es_419.po` (808 lines)
- `addons/stock_landed_costs/i18n/es_CL.po` (184 lines)
- `addons/stock_landed_costs/i18n/et.po` (813 lines)
- `addons/stock_landed_costs/i18n/eu.po` (774 lines)
- `addons/stock_landed_costs/i18n/fa.po` (797 lines)
- `addons/stock_landed_costs/i18n/fi.po` (826 lines)
- `addons/stock_landed_costs/i18n/fo.po` (774 lines)
- `addons/stock_landed_costs/i18n/fr.po` (812 lines)
- `addons/stock_landed_costs/i18n/fr_BE.po` (91 lines)
- `addons/stock_landed_costs/i18n/fr_CA.po` (152 lines)
- `addons/stock_landed_costs/i18n/gl.po` (774 lines)
- `addons/stock_landed_costs/i18n/gu.po` (786 lines)
- `addons/stock_landed_costs/i18n/he.po` (804 lines)
- `addons/stock_landed_costs/i18n/hi.po` (787 lines)
- `addons/stock_landed_costs/i18n/hr.po` (807 lines)
- `addons/stock_landed_costs/i18n/hu.po` (806 lines)
- `addons/stock_landed_costs/i18n/hy.po` (774 lines)
- `addons/stock_landed_costs/i18n/id.po` (808 lines)
- `addons/stock_landed_costs/i18n/is.po` (783 lines)
- `addons/stock_landed_costs/i18n/it.po` (814 lines)
- `addons/stock_landed_costs/i18n/ja.po` (807 lines)
- `addons/stock_landed_costs/i18n/ka.po` (774 lines)
- `addons/stock_landed_costs/i18n/kab.po` (777 lines)
- `addons/stock_landed_costs/i18n/kk.po` (774 lines)
- `addons/stock_landed_costs/i18n/km.po` (784 lines)
- `addons/stock_landed_costs/i18n/ko.po` (803 lines)
- `addons/stock_landed_costs/i18n/ku.po` (788 lines)
- `addons/stock_landed_costs/i18n/lo.po` (808 lines)
- `addons/stock_landed_costs/i18n/lt.po` (813 lines)
- `addons/stock_landed_costs/i18n/lv.po` (793 lines)
- `addons/stock_landed_costs/i18n/mk.po` (776 lines)
- `addons/stock_landed_costs/i18n/mn.po` (799 lines)
- `addons/stock_landed_costs/i18n/my.po` (777 lines)
- `addons/stock_landed_costs/i18n/nb.po` (795 lines)
- `addons/stock_landed_costs/i18n/nl.po` (809 lines)
- `addons/stock_landed_costs/i18n/pl.po` (815 lines)
- `addons/stock_landed_costs/i18n/pt.po` (812 lines)
- `addons/stock_landed_costs/i18n/pt_BR.po` (823 lines)
- `addons/stock_landed_costs/i18n/ro.po` (812 lines)
- `addons/stock_landed_costs/i18n/ru.po` (811 lines)
- `addons/stock_landed_costs/i18n/sk.po` (796 lines)
- `addons/stock_landed_costs/i18n/sl.po` (799 lines)
- `addons/stock_landed_costs/i18n/sq.po` (774 lines)
- `addons/stock_landed_costs/i18n/sr@latin.po` (791 lines)
- `addons/stock_landed_costs/i18n/stock_landed_costs.pot` (765 lines)
- `addons/stock_landed_costs/i18n/sv.po` (815 lines)
- `addons/stock_landed_costs/i18n/ta.po` (776 lines)
- `addons/stock_landed_costs/i18n/te.po` (774 lines)
- `addons/stock_landed_costs/i18n/th.po` (801 lines)
- `addons/stock_landed_costs/i18n/tr.po` (820 lines)
- `addons/stock_landed_costs/i18n/uk.po` (804 lines)
- `addons/stock_landed_costs/i18n/uz.po` (922 lines)
- `addons/stock_landed_costs/i18n/vi.po` (803 lines)
- `addons/stock_landed_costs/i18n/zh_CN.po` (806 lines)
- `addons/stock_landed_costs/i18n/zh_TW.po` (794 lines)
- `addons/stock_landed_costs/models/__init__.py` (10 lines)
- `addons/stock_landed_costs/models/account_move.py` (79 lines)
- `addons/stock_landed_costs/models/product.py` (28 lines)
- `addons/stock_landed_costs/models/purchase.py` (10 lines)
- `addons/stock_landed_costs/models/res_company.py` (10 lines)
- `addons/stock_landed_costs/models/res_config_settings.py` (10 lines)
- `addons/stock_landed_costs/models/stock_landed_cost.py` (426 lines)
- `addons/stock_landed_costs/models/stock_move.py` (54 lines)
- `addons/stock_landed_costs/security/ir.access.csv` (5 lines)
- `addons/stock_landed_costs/tests/__init__.py` (8 lines)
- `addons/stock_landed_costs/tests/common.py` (60 lines)
- `addons/stock_landed_costs/tests/test_stock_landed_costs.py` (78 lines)
- `addons/stock_landed_costs/tests/test_stock_landed_costs_branches.py` (95 lines)
- `addons/stock_landed_costs/tests/test_stock_landed_costs_lots.py` (185 lines)
- `addons/stock_landed_costs/tests/test_stock_landed_costs_purchase.py` (772 lines)
- `addons/stock_landed_costs/tests/test_stock_landed_costs_rounding.py` (316 lines)
- `addons/stock_landed_costs/tests/test_stockvaluationlayer.py` (734 lines)
- `addons/stock_landed_costs/views/account_move_views.xml` (37 lines)
- `addons/stock_landed_costs/views/product_views.xml` (25 lines)
- `addons/stock_landed_costs/views/res_config_settings_views.xml` (20 lines)
- `addons/stock_landed_costs/views/stock_landed_cost_views.xml` (226 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
