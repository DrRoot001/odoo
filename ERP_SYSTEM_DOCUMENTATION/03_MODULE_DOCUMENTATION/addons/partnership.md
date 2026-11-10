# Module: partnership

- **Module ID:** MOD-391
- **Path:** `addons/partnership`
- **Manifest:** `addons/partnership/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This module allows you to manage all operations for managing memberships and partnerships.
==========================================================================================

You can easily assign grade to members/partners, with a specific pricelist.
    

Declared dependencies: `crm`, `sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 13 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 8 | Files under `models/` or `models.py`. |
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
    "crm",
    "sale"
  ],
  "data": [
    "data/res_partner_grade_data.xml",
    "views/res_config_settings_views.xml",
    "views/res_partner_views.xml",
    "views/res_partner_grade_views.xml",
    "views/product_template_views.xml",
    "views/product_pricelist_views.xml",
    "views/partnership_menu.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/partnership/__init__.py` (3 lines)
- `addons/partnership/__manifest__.py` (24 lines)
- `addons/partnership/data/res_partner_grade_data.xml` (15 lines)
- `addons/partnership/i18n/ar.po` (301 lines)
- `addons/partnership/i18n/az.po` (295 lines)
- `addons/partnership/i18n/bg.po` (295 lines)
- `addons/partnership/i18n/bs.po` (297 lines)
- `addons/partnership/i18n/ca.po` (296 lines)
- `addons/partnership/i18n/cs.po` (296 lines)
- `addons/partnership/i18n/da.po` (295 lines)
- `addons/partnership/i18n/de.po` (313 lines)
- `addons/partnership/i18n/el.po` (295 lines)
- `addons/partnership/i18n/es.po` (314 lines)
- `addons/partnership/i18n/es_419.po` (305 lines)
- `addons/partnership/i18n/et.po` (295 lines)
- `addons/partnership/i18n/fa.po` (295 lines)
- `addons/partnership/i18n/fi.po` (306 lines)
- `addons/partnership/i18n/fr.po` (305 lines)
- `addons/partnership/i18n/he.po` (296 lines)
- `addons/partnership/i18n/hi.po` (295 lines)
- `addons/partnership/i18n/hr.po` (296 lines)
- `addons/partnership/i18n/hu.po` (295 lines)
- `addons/partnership/i18n/id.po` (305 lines)
- `addons/partnership/i18n/it.po` (313 lines)
- `addons/partnership/i18n/ja.po` (305 lines)
- `addons/partnership/i18n/kab.po` (296 lines)
- `addons/partnership/i18n/ko.po` (296 lines)
- `addons/partnership/i18n/ku.po` (295 lines)
- `addons/partnership/i18n/lo.po` (304 lines)
- `addons/partnership/i18n/lt.po` (297 lines)
- `addons/partnership/i18n/lv.po` (296 lines)
- `addons/partnership/i18n/mn.po` (295 lines)
- `addons/partnership/i18n/my.po` (296 lines)
- `addons/partnership/i18n/nb.po` (295 lines)
- `addons/partnership/i18n/nl.po` (313 lines)
- `addons/partnership/i18n/partnership.pot` (292 lines)
- `addons/partnership/i18n/pl.po` (305 lines)
- `addons/partnership/i18n/pt.po` (295 lines)
- `addons/partnership/i18n/pt_BR.po` (313 lines)
- `addons/partnership/i18n/ro.po` (307 lines)
- `addons/partnership/i18n/ru.po` (306 lines)
- `addons/partnership/i18n/sk.po` (295 lines)
- `addons/partnership/i18n/sl.po` (296 lines)
- `addons/partnership/i18n/sr@latin.po` (296 lines)
- `addons/partnership/i18n/sv.po` (296 lines)
- `addons/partnership/i18n/th.po` (296 lines)
- `addons/partnership/i18n/tr.po` (306 lines)
- `addons/partnership/i18n/uk.po` (296 lines)
- `addons/partnership/i18n/uz.po` (356 lines)
- `addons/partnership/i18n/vi.po` (297 lines)
- `addons/partnership/i18n/zh_CN.po` (305 lines)
- `addons/partnership/i18n/zh_TW.po` (302 lines)
- `addons/partnership/models/__init__.py` (9 lines)
- `addons/partnership/models/product_pricelist.py` (20 lines)
- `addons/partnership/models/product_template.py` (16 lines)
- `addons/partnership/models/res_company.py` (12 lines)
- `addons/partnership/models/res_config_settings.py` (15 lines)
- `addons/partnership/models/res_partner.py` (24 lines)
- `addons/partnership/models/res_partner_grade.py` (27 lines)
- `addons/partnership/models/sale_order.py` (36 lines)
- `addons/partnership/security/ir.access.csv` (5 lines)
- `addons/partnership/static/description/icon.png` (16 lines)
- `addons/partnership/tests/__init__.py` (3 lines)
- `addons/partnership/tests/common.py` (33 lines)
- `addons/partnership/tests/test_partnership.py` (50 lines)
- `addons/partnership/views/partnership_menu.xml` (12 lines)
- `addons/partnership/views/product_pricelist_views.xml` (16 lines)
- `addons/partnership/views/product_template_views.xml` (16 lines)
- `addons/partnership/views/res_config_settings_views.xml` (16 lines)
- `addons/partnership/views/res_partner_grade_views.xml` (66 lines)
- `addons/partnership/views/res_partner_views.xml` (69 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
