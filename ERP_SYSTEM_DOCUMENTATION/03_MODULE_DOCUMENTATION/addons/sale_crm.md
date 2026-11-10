# Module: sale_crm

- **Module ID:** MOD-510
- **Path:** `addons/sale_crm`
- **Manifest:** `addons/sale_crm/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This module adds a shortcut on one or several opportunity cases in the CRM.
===========================================================================

This shortcut allows you to generate a sales order based on the selected case.
If different cases are open (a list), it generates one sales order by case.
The case is then closed and linked to the generated sales order.

We suggest you to install this module, if you installed both the sale and the crm
modules.
    

Declared dependencies: `sale`, `crm`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 13 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "sale",
    "crm"
  ],
  "data": [
    "data/crm_lead_merge_template.xml",
    "views/sale_order_views.xml",
    "views/crm_lead_views.xml",
    "views/crm_team_views.xml",
    "wizard/crm_opportunity_to_quotation_views.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/sale_crm/__init__.py` (9 lines)
- `addons/sale_crm/__manifest__.py` (30 lines)
- `addons/sale_crm/data/crm_lead_merge_template.xml` (18 lines)
- `addons/sale_crm/i18n/af.po` (227 lines)
- `addons/sale_crm/i18n/ar.po` (231 lines)
- `addons/sale_crm/i18n/az.po` (232 lines)
- `addons/sale_crm/i18n/bg.po` (238 lines)
- `addons/sale_crm/i18n/bs.po` (249 lines)
- `addons/sale_crm/i18n/ca.po` (238 lines)
- `addons/sale_crm/i18n/cs.po` (234 lines)
- `addons/sale_crm/i18n/da.po` (233 lines)
- `addons/sale_crm/i18n/de.po` (248 lines)
- `addons/sale_crm/i18n/el.po` (237 lines)
- `addons/sale_crm/i18n/es.po` (248 lines)
- `addons/sale_crm/i18n/es_419.po` (243 lines)
- `addons/sale_crm/i18n/es_CL.po` (39 lines)
- `addons/sale_crm/i18n/et.po` (238 lines)
- `addons/sale_crm/i18n/eu.po` (229 lines)
- `addons/sale_crm/i18n/fa.po` (233 lines)
- `addons/sale_crm/i18n/fi.po` (248 lines)
- `addons/sale_crm/i18n/fr.po` (236 lines)
- `addons/sale_crm/i18n/fr_CA.po` (39 lines)
- `addons/sale_crm/i18n/gl.po` (225 lines)
- `addons/sale_crm/i18n/gu.po` (227 lines)
- `addons/sale_crm/i18n/he.po` (237 lines)
- `addons/sale_crm/i18n/hi.po` (234 lines)
- `addons/sale_crm/i18n/hr.po` (240 lines)
- `addons/sale_crm/i18n/hu.po` (237 lines)
- `addons/sale_crm/i18n/id.po` (247 lines)
- `addons/sale_crm/i18n/is.po` (223 lines)
- `addons/sale_crm/i18n/it.po` (248 lines)
- `addons/sale_crm/i18n/ja.po` (231 lines)
- `addons/sale_crm/i18n/kab.po` (237 lines)
- `addons/sale_crm/i18n/km.po` (227 lines)
- `addons/sale_crm/i18n/ko.po` (231 lines)
- `addons/sale_crm/i18n/ku.po` (227 lines)
- `addons/sale_crm/i18n/lo.po` (258 lines)
- `addons/sale_crm/i18n/lt.po` (244 lines)
- `addons/sale_crm/i18n/lv.po` (246 lines)
- `addons/sale_crm/i18n/mk.po` (227 lines)
- `addons/sale_crm/i18n/mn.po` (234 lines)
- `addons/sale_crm/i18n/my.po` (230 lines)
- `addons/sale_crm/i18n/nb.po` (233 lines)
- `addons/sale_crm/i18n/nl.po` (248 lines)
- `addons/sale_crm/i18n/pl.po` (246 lines)
- `addons/sale_crm/i18n/pt.po` (239 lines)
- `addons/sale_crm/i18n/pt_BR.po` (248 lines)
- `addons/sale_crm/i18n/ro.po` (234 lines)
- `addons/sale_crm/i18n/ru.po` (247 lines)
- `addons/sale_crm/i18n/sale_crm.pot` (221 lines)
- `addons/sale_crm/i18n/sk.po` (242 lines)
- `addons/sale_crm/i18n/sl.po` (238 lines)
- `addons/sale_crm/i18n/sr@latin.po` (232 lines)
- `addons/sale_crm/i18n/sv.po` (240 lines)
- `addons/sale_crm/i18n/th.po` (233 lines)
- `addons/sale_crm/i18n/tr.po` (241 lines)
- `addons/sale_crm/i18n/uk.po` (237 lines)
- `addons/sale_crm/i18n/uz.po` (266 lines)
- `addons/sale_crm/i18n/vi.po` (231 lines)
- `addons/sale_crm/i18n/zh_CN.po` (241 lines)
- `addons/sale_crm/i18n/zh_TW.po` (230 lines)
- `addons/sale_crm/models/__init__.py` (6 lines)
- `addons/sale_crm/models/crm_lead.py` (111 lines)
- `addons/sale_crm/models/crm_team.py` (18 lines)
- `addons/sale_crm/models/sale_order.py` (18 lines)
- `addons/sale_crm/security/ir.access.csv` (2 lines)
- `addons/sale_crm/tests/__init__.py` (7 lines)
- `addons/sale_crm/tests/test_crm_lead_convert_quotation.py` (120 lines)
- `addons/sale_crm/tests/test_crm_lead_merge.py` (41 lines)
- `addons/sale_crm/tests/test_res_partner.py` (114 lines)
- `addons/sale_crm/tests/test_sale_crm.py` (63 lines)
- `addons/sale_crm/views/crm_lead_views.xml` (42 lines)
- `addons/sale_crm/views/crm_team_views.xml` (15 lines)
- `addons/sale_crm/views/sale_order_views.xml` (47 lines)
- `addons/sale_crm/wizard/__init__.py` (4 lines)
- `addons/sale_crm/wizard/crm_opportunity_to_quotation.py` (52 lines)
- `addons/sale_crm/wizard/crm_opportunity_to_quotation_views.xml` (31 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
