# Module: mrp_account

- **Module ID:** MOD-378
- **Path:** `addons/mrp_account`
- **Manifest:** `addons/mrp_account/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Analytic accounting in Manufacturing


Analytic Accounting in MRP
==========================

* Cost structure report

Also, allows to compute the cost of the product based on its BoM, using the costs of its components and work center operations.
It adds a button on the product itself but also an action in the list view of the products.
If the automated inventory valuation is active, the necessary accounting entries will be created.



Declared dependencies: `mrp`, `stock_account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 24 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 10 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 13 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 4 | Client behavior/assets. |
| Tests | 6 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mrp",
    "stock_account"
  ],
  "data": [
    "views/product_views.xml",
    "views/mrp_bom_views.xml",
    "views/mrp_production_views.xml",
    "views/analytic_account_views.xml",
    "views/account_move_views.xml",
    "views/mrp_workcenter_views.xml",
    "report/report_mrp_templates.xml",
    "report/mrp_report_mo_overview.xml",
    "wizard/mrp_wip_accounting.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/mrp_account_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "mrp_account/static/src/**/*"
    ]
  }
}
```

### Representative source files

- `addons/mrp_account/__init__.py` (5 lines)
- `addons/mrp_account/__manifest__.py` (43 lines)
- `addons/mrp_account/data/mrp_account_demo.xml` (73 lines)
- `addons/mrp_account/i18n/ar.po` (706 lines)
- `addons/mrp_account/i18n/az.po` (671 lines)
- `addons/mrp_account/i18n/bg.po` (678 lines)
- `addons/mrp_account/i18n/bs.po` (665 lines)
- `addons/mrp_account/i18n/ca.po` (701 lines)
- `addons/mrp_account/i18n/cs.po` (677 lines)
- `addons/mrp_account/i18n/da.po` (691 lines)
- `addons/mrp_account/i18n/de.po` (712 lines)
- `addons/mrp_account/i18n/el.po` (673 lines)
- `addons/mrp_account/i18n/es.po` (708 lines)
- `addons/mrp_account/i18n/es_419.po` (707 lines)
- `addons/mrp_account/i18n/es_CL.po` (601 lines)
- `addons/mrp_account/i18n/et.po` (698 lines)
- `addons/mrp_account/i18n/eu.po` (618 lines)
- `addons/mrp_account/i18n/fa.po` (686 lines)
- `addons/mrp_account/i18n/fi.po` (712 lines)
- `addons/mrp_account/i18n/fr.po` (699 lines)
- `addons/mrp_account/i18n/gl.po` (618 lines)
- `addons/mrp_account/i18n/gu.po` (620 lines)
- `addons/mrp_account/i18n/he.po` (685 lines)
- `addons/mrp_account/i18n/hi.po` (664 lines)
- `addons/mrp_account/i18n/hr.po` (677 lines)
- `addons/mrp_account/i18n/hu.po` (676 lines)
- `addons/mrp_account/i18n/id.po` (693 lines)
- `addons/mrp_account/i18n/is.po` (616 lines)
- `addons/mrp_account/i18n/it.po` (697 lines)
- `addons/mrp_account/i18n/ja.po` (689 lines)
- `addons/mrp_account/i18n/kab.po` (663 lines)
- `addons/mrp_account/i18n/km.po` (619 lines)
- `addons/mrp_account/i18n/ko.po` (690 lines)
- `addons/mrp_account/i18n/ku.po` (663 lines)
- `addons/mrp_account/i18n/lo.po` (683 lines)
- `addons/mrp_account/i18n/lt.po` (679 lines)
- `addons/mrp_account/i18n/lv.po` (666 lines)
- `addons/mrp_account/i18n/mk.po` (619 lines)
- `addons/mrp_account/i18n/mn.po` (674 lines)
- `addons/mrp_account/i18n/mrp_account.pot` (656 lines)
- `addons/mrp_account/i18n/my.po` (667 lines)
- `addons/mrp_account/i18n/nb.po` (678 lines)
- `addons/mrp_account/i18n/nl.po` (692 lines)
- `addons/mrp_account/i18n/pl.po` (702 lines)
- `addons/mrp_account/i18n/pt.po` (686 lines)
- `addons/mrp_account/i18n/pt_BR.po` (720 lines)
- `addons/mrp_account/i18n/ro.po` (696 lines)
- `addons/mrp_account/i18n/ru.po` (710 lines)
- `addons/mrp_account/i18n/sk.po` (672 lines)
- `addons/mrp_account/i18n/sl.po` (674 lines)
- `addons/mrp_account/i18n/sr@latin.po` (671 lines)
- `addons/mrp_account/i18n/sv.po` (697 lines)
- `addons/mrp_account/i18n/th.po` (685 lines)
- `addons/mrp_account/i18n/tr.po` (722 lines)
- `addons/mrp_account/i18n/uk.po` (688 lines)
- `addons/mrp_account/i18n/uz.po` (790 lines)
- `addons/mrp_account/i18n/vi.po` (690 lines)
- `addons/mrp_account/i18n/zh_CN.po` (696 lines)
- `addons/mrp_account/i18n/zh_TW.po` (683 lines)
- `addons/mrp_account/models/__init__.py` (10 lines)
- `addons/mrp_account/models/account_move.py` (67 lines)
- `addons/mrp_account/models/analytic_account.py` (90 lines)
- `addons/mrp_account/models/mrp_bom.py` (8 lines)
- `addons/mrp_account/models/mrp_production.py` (177 lines)
- `addons/mrp_account/models/mrp_workcenter.py` (26 lines)
- `addons/mrp_account/models/mrp_workorder.py` (76 lines)
- `addons/mrp_account/models/product.py` (128 lines)
- `addons/mrp_account/models/res_company.py` (13 lines)
- `addons/mrp_account/models/stock_move.py` (95 lines)
- `addons/mrp_account/report/__init__.py` (3 lines)
- `addons/mrp_account/report/mrp_report_bom_structure.py` (38 lines)
- `addons/mrp_account/report/mrp_report_mo_overview.py` (48 lines)
- `addons/mrp_account/report/mrp_report_mo_overview.xml` (21 lines)
- `addons/mrp_account/report/report_mrp_templates.xml` (79 lines)
- `addons/mrp_account/report/stock_valuation_report.py` (47 lines)
- `addons/mrp_account/security/ir.access.csv` (7 lines)
- `addons/mrp_account/static/src/components/bom_overview_extra_bom_cost_line/bom_overview_extra_bom_cost_line.js` (14 lines)
- `addons/mrp_account/static/src/components/bom_overview_extra_bom_cost_line/bom_overview_extra_bom_cost_line.xml` (19 lines)
- `addons/mrp_account/static/src/components/mo_overview_extra_bom_cost_line/mo_overview_extra_bom_cost_line.js` (14 lines)
- `addons/mrp_account/static/src/components/mo_overview_extra_bom_cost_line/mo_overview_extra_bom_cost_line.xml` (17 lines)
- `addons/mrp_account/static/src/stock_valuation/controller.js` (16 lines)
- `addons/mrp_account/static/src/stock_valuation/stock_valuation_report.js` (11 lines)
- `addons/mrp_account/static/src/stock_valuation/stock_valuation_report.xml` (19 lines)
- `addons/mrp_account/tests/__init__.py` (6 lines)
- `addons/mrp_account/tests/common.py` (288 lines)
- `addons/mrp_account/tests/test_analytic_account.py` (68 lines)
- `addons/mrp_account/tests/test_mrp_account.py` (742 lines)
- `addons/mrp_account/tests/test_valuation_layers.py` (635 lines)
- `addons/mrp_account/tests/test_valuation_operation.py` (114 lines)
- `addons/mrp_account/views/account_move_views.xml` (17 lines)
- `addons/mrp_account/views/analytic_account_views.xml` (24 lines)
- `addons/mrp_account/views/mrp_bom_views.xml` (19 lines)
- `addons/mrp_account/views/mrp_production_views.xml` (43 lines)
- `addons/mrp_account/views/mrp_workcenter_views.xml` (13 lines)
- `addons/mrp_account/views/product_views.xml` (69 lines)
- `addons/mrp_account/wizard/__init__.py` (3 lines)
- `addons/mrp_account/wizard/mrp_wip_accounting.py` (146 lines)
- `addons/mrp_account/wizard/mrp_wip_accounting.xml` (46 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
