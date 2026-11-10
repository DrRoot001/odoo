# Module: base_address_extended

- **Module ID:** MOD-034
- **Path:** `addons/base_address_extended`
- **Manifest:** `addons/base_address_extended/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Add extra fields on addresses


Extended Addresses Management
=============================

This module provides the ability to choose a city from a list (in specific countries).

It is primarily used for EDIs that might need a special city code.
        

Declared dependencies: `web`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "web"
  ],
  "data": [
    "views/res_city_view.xml",
    "views/res_country_view.xml",
    "views/res_partner_views.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/base_address_extended/__init__.py` (4 lines)
- `addons/base_address_extended/__manifest__.py` (25 lines)
- `addons/base_address_extended/i18n/af.po` (238 lines)
- `addons/base_address_extended/i18n/ar.po` (232 lines)
- `addons/base_address_extended/i18n/az.po` (215 lines)
- `addons/base_address_extended/i18n/base_address_extended.pot` (197 lines)
- `addons/base_address_extended/i18n/bg.po` (225 lines)
- `addons/base_address_extended/i18n/bs.po` (216 lines)
- `addons/base_address_extended/i18n/ca.po` (237 lines)
- `addons/base_address_extended/i18n/cs.po` (234 lines)
- `addons/base_address_extended/i18n/da.po` (235 lines)
- `addons/base_address_extended/i18n/de.po` (245 lines)
- `addons/base_address_extended/i18n/el.po` (216 lines)
- `addons/base_address_extended/i18n/es.po` (244 lines)
- `addons/base_address_extended/i18n/es_419.po` (240 lines)
- `addons/base_address_extended/i18n/et.po` (238 lines)
- `addons/base_address_extended/i18n/fa.po` (233 lines)
- `addons/base_address_extended/i18n/fi.po` (250 lines)
- `addons/base_address_extended/i18n/fr.po` (245 lines)
- `addons/base_address_extended/i18n/gu.po` (238 lines)
- `addons/base_address_extended/i18n/he.po` (238 lines)
- `addons/base_address_extended/i18n/hi.po` (212 lines)
- `addons/base_address_extended/i18n/hr.po` (234 lines)
- `addons/base_address_extended/i18n/hu.po` (231 lines)
- `addons/base_address_extended/i18n/id.po` (234 lines)
- `addons/base_address_extended/i18n/is.po` (234 lines)
- `addons/base_address_extended/i18n/it.po` (245 lines)
- `addons/base_address_extended/i18n/ja.po` (242 lines)
- `addons/base_address_extended/i18n/kab.po` (205 lines)
- `addons/base_address_extended/i18n/km.po` (237 lines)
- `addons/base_address_extended/i18n/ko.po` (233 lines)
- `addons/base_address_extended/i18n/ku.po` (209 lines)
- `addons/base_address_extended/i18n/lo.po` (218 lines)
- `addons/base_address_extended/i18n/lt.po` (240 lines)
- `addons/base_address_extended/i18n/lv.po` (216 lines)
- `addons/base_address_extended/i18n/mn.po` (233 lines)
- `addons/base_address_extended/i18n/my.po` (213 lines)
- `addons/base_address_extended/i18n/nb.po` (222 lines)
- `addons/base_address_extended/i18n/nl.po` (233 lines)
- `addons/base_address_extended/i18n/pl.po` (243 lines)
- `addons/base_address_extended/i18n/pt.po` (239 lines)
- `addons/base_address_extended/i18n/pt_BR.po` (244 lines)
- `addons/base_address_extended/i18n/ro.po` (233 lines)
- `addons/base_address_extended/i18n/ru.po` (232 lines)
- `addons/base_address_extended/i18n/sk.po` (221 lines)
- `addons/base_address_extended/i18n/sl.po` (235 lines)
- `addons/base_address_extended/i18n/sr@latin.po` (233 lines)
- `addons/base_address_extended/i18n/sv.po` (239 lines)
- `addons/base_address_extended/i18n/th.po` (231 lines)
- `addons/base_address_extended/i18n/tr.po` (235 lines)
- `addons/base_address_extended/i18n/uk.po` (233 lines)
- `addons/base_address_extended/i18n/uz.po` (265 lines)
- `addons/base_address_extended/i18n/vi.po` (233 lines)
- `addons/base_address_extended/i18n/zh_CN.po` (240 lines)
- `addons/base_address_extended/i18n/zh_TW.po` (228 lines)
- `addons/base_address_extended/models/__init__.py` (5 lines)
- `addons/base_address_extended/models/res_city.py` (26 lines)
- `addons/base_address_extended/models/res_country.py` (12 lines)
- `addons/base_address_extended/models/res_partner.py` (78 lines)
- `addons/base_address_extended/security/ir.access.csv` (3 lines)
- `addons/base_address_extended/tests/__init__.py` (4 lines)
- `addons/base_address_extended/tests/test_street_fields.py` (101 lines)
- `addons/base_address_extended/views/res_city_view.xml` (64 lines)
- `addons/base_address_extended/views/res_country_view.xml` (25 lines)
- `addons/base_address_extended/views/res_partner_views.xml` (54 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
