# Module: purchase_requisition

- **Module ID:** MOD-501
- **Path:** `addons/purchase_requisition`
- **Manifest:** `addons/purchase_requisition/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This module allows you to manage your Purchase Agreements.
===========================================================

Manage calls for tenders and blanket orders. Calls for tenders are used to get
competing offers from different vendors and select the best ones. Blanket orders
are agreements you have with vendors to benefit from a predetermined pricing.


Declared dependencies: `purchase`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 7 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "purchase"
  ],
  "data": [
    "data/purchase_requisition_data.xml",
    "views/product_views.xml",
    "views/purchase_views.xml",
    "views/purchase_requisition_views.xml",
    "report/purchase_requisition_report.xml",
    "report/report_purchaserequisition.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/purchase_requisition_demo.xml"
  ]
}
```

### Representative source files

- `addons/purchase_requisition/__init__.py` (3 lines)
- `addons/purchase_requisition/__manifest__.py` (27 lines)
- `addons/purchase_requisition/data/purchase_requisition_data.xml` (19 lines)
- `addons/purchase_requisition/data/purchase_requisition_demo.xml` (53 lines)
- `addons/purchase_requisition/i18n/af.po` (895 lines)
- `addons/purchase_requisition/i18n/am.po` (891 lines)
- `addons/purchase_requisition/i18n/ar.po` (922 lines)
- `addons/purchase_requisition/i18n/az.po` (900 lines)
- `addons/purchase_requisition/i18n/bg.po` (914 lines)
- `addons/purchase_requisition/i18n/bs.po` (894 lines)
- `addons/purchase_requisition/i18n/ca.po` (922 lines)
- `addons/purchase_requisition/i18n/cs.po` (914 lines)
- `addons/purchase_requisition/i18n/da.po` (931 lines)
- `addons/purchase_requisition/i18n/de.po` (946 lines)
- `addons/purchase_requisition/i18n/el.po` (906 lines)
- `addons/purchase_requisition/i18n/es.po` (940 lines)
- `addons/purchase_requisition/i18n/es_419.po` (937 lines)
- `addons/purchase_requisition/i18n/es_CL.po` (154 lines)
- `addons/purchase_requisition/i18n/et.po` (950 lines)
- `addons/purchase_requisition/i18n/eu.po` (893 lines)
- `addons/purchase_requisition/i18n/fa.po` (906 lines)
- `addons/purchase_requisition/i18n/fi.po` (944 lines)
- `addons/purchase_requisition/i18n/fo.po` (893 lines)
- `addons/purchase_requisition/i18n/fr.po` (938 lines)
- `addons/purchase_requisition/i18n/fr_BE.po` (84 lines)
- `addons/purchase_requisition/i18n/fr_CA.po` (116 lines)
- `addons/purchase_requisition/i18n/gl.po` (893 lines)
- `addons/purchase_requisition/i18n/gu.po` (905 lines)
- `addons/purchase_requisition/i18n/he.po` (933 lines)
- `addons/purchase_requisition/i18n/hi.po` (898 lines)
- `addons/purchase_requisition/i18n/hr.po` (911 lines)
- `addons/purchase_requisition/i18n/hu.po` (908 lines)
- `addons/purchase_requisition/i18n/id.po` (933 lines)
- `addons/purchase_requisition/i18n/is.po` (897 lines)
- `addons/purchase_requisition/i18n/it.po` (942 lines)
- `addons/purchase_requisition/i18n/ja.po` (920 lines)
- `addons/purchase_requisition/i18n/ka.po` (893 lines)
- `addons/purchase_requisition/i18n/kab.po` (887 lines)
- `addons/purchase_requisition/i18n/km.po` (903 lines)
- `addons/purchase_requisition/i18n/ko.po` (918 lines)
- `addons/purchase_requisition/i18n/ku.po` (897 lines)
- `addons/purchase_requisition/i18n/lo.po` (914 lines)
- `addons/purchase_requisition/i18n/lt.po` (916 lines)
- `addons/purchase_requisition/i18n/lv.po` (906 lines)
- `addons/purchase_requisition/i18n/mk.po` (899 lines)
- `addons/purchase_requisition/i18n/mn.po` (915 lines)
- `addons/purchase_requisition/i18n/my.po` (889 lines)
- `addons/purchase_requisition/i18n/nb.po` (904 lines)
- `addons/purchase_requisition/i18n/nl.po` (944 lines)
- `addons/purchase_requisition/i18n/pl.po` (949 lines)
- `addons/purchase_requisition/i18n/pt.po` (918 lines)
- `addons/purchase_requisition/i18n/pt_BR.po` (943 lines)
- `addons/purchase_requisition/i18n/purchase_requisition.pot` (878 lines)
- `addons/purchase_requisition/i18n/ro.po` (929 lines)
- `addons/purchase_requisition/i18n/ru.po` (929 lines)
- `addons/purchase_requisition/i18n/sk.po` (905 lines)
- `addons/purchase_requisition/i18n/sl.po` (908 lines)
- `addons/purchase_requisition/i18n/sq.po` (893 lines)
- `addons/purchase_requisition/i18n/sr@latin.po` (903 lines)
- `addons/purchase_requisition/i18n/sv.po` (941 lines)
- `addons/purchase_requisition/i18n/th.po` (917 lines)
- `addons/purchase_requisition/i18n/tr.po` (942 lines)
- `addons/purchase_requisition/i18n/uk.po` (913 lines)
- `addons/purchase_requisition/i18n/uz.po` (1,064 lines)
- `addons/purchase_requisition/i18n/vi.po` (923 lines)
- `addons/purchase_requisition/i18n/zh_CN.po` (926 lines)
- `addons/purchase_requisition/i18n/zh_TW.po` (916 lines)
- `addons/purchase_requisition/models/__init__.py` (5 lines)
- `addons/purchase_requisition/models/product.py` (22 lines)
- `addons/purchase_requisition/models/purchase.py` (130 lines)
- `addons/purchase_requisition/models/purchase_requisition.py` (377 lines)
- `addons/purchase_requisition/report/purchase_requisition_report.xml` (12 lines)
- `addons/purchase_requisition/report/report_purchaserequisition.xml` (163 lines)
- `addons/purchase_requisition/security/ir.access.csv` (5 lines)
- `addons/purchase_requisition/tests/__init__.py` (5 lines)
- `addons/purchase_requisition/tests/common.py` (66 lines)
- `addons/purchase_requisition/tests/test_purchase_requisition.py` (276 lines)
- `addons/purchase_requisition/views/product_views.xml` (27 lines)
- `addons/purchase_requisition/views/purchase_requisition_views.xml` (251 lines)
- `addons/purchase_requisition/views/purchase_views.xml` (32 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
