# Module: website_partner

- **Module ID:** MOD-629
- **Path:** `addons/website_partner`
- **Manifest:** `addons/website_partner/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Partner module for website


This is a base module. It holds website-related stuff for Contact model (res.partner).
    

Declared dependencies: `website`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website"
  ],
  "data": [
    "views/res_partner_views.xml",
    "views/website_partner_templates.xml",
    "data/website_partner_data.xml"
  ],
  "demo": [
    "data/website_partner_demo.xml"
  ]
}
```

### Representative source files

- `addons/website_partner/__init__.py` (5 lines)
- `addons/website_partner/__manifest__.py` (20 lines)
- `addons/website_partner/controllers/__init__.py` (3 lines)
- `addons/website_partner/controllers/main.py` (32 lines)
- `addons/website_partner/data/website_partner_data.xml` (22 lines)
- `addons/website_partner/data/website_partner_demo.xml` (97 lines)
- `addons/website_partner/i18n/af.po` (143 lines)
- `addons/website_partner/i18n/ar.po` (150 lines)
- `addons/website_partner/i18n/az.po` (146 lines)
- `addons/website_partner/i18n/bg.po` (146 lines)
- `addons/website_partner/i18n/bs.po` (146 lines)
- `addons/website_partner/i18n/ca.po` (148 lines)
- `addons/website_partner/i18n/cs.po` (148 lines)
- `addons/website_partner/i18n/da.po` (148 lines)
- `addons/website_partner/i18n/de.po` (150 lines)
- `addons/website_partner/i18n/el.po` (146 lines)
- `addons/website_partner/i18n/es.po` (152 lines)
- `addons/website_partner/i18n/es_419.po` (147 lines)
- `addons/website_partner/i18n/et.po` (147 lines)
- `addons/website_partner/i18n/fa.po` (146 lines)
- `addons/website_partner/i18n/fi.po` (150 lines)
- `addons/website_partner/i18n/fr.po` (151 lines)
- `addons/website_partner/i18n/gu.po` (143 lines)
- `addons/website_partner/i18n/he.po` (152 lines)
- `addons/website_partner/i18n/hi.po` (143 lines)
- `addons/website_partner/i18n/hr.po` (147 lines)
- `addons/website_partner/i18n/hu.po` (147 lines)
- `addons/website_partner/i18n/id.po` (148 lines)
- `addons/website_partner/i18n/is.po` (139 lines)
- `addons/website_partner/i18n/it.po` (151 lines)
- `addons/website_partner/i18n/ja.po` (148 lines)
- `addons/website_partner/i18n/kab.po` (143 lines)
- `addons/website_partner/i18n/km.po` (142 lines)
- `addons/website_partner/i18n/ko.po` (147 lines)
- `addons/website_partner/i18n/ku.po` (143 lines)
- `addons/website_partner/i18n/lo.po` (145 lines)
- `addons/website_partner/i18n/lt.po` (150 lines)
- `addons/website_partner/i18n/lv.po` (147 lines)
- `addons/website_partner/i18n/mk.po` (146 lines)
- `addons/website_partner/i18n/mn.po` (147 lines)
- `addons/website_partner/i18n/my.po` (143 lines)
- `addons/website_partner/i18n/nb.po` (147 lines)
- `addons/website_partner/i18n/nl.po` (149 lines)
- `addons/website_partner/i18n/pl.po` (151 lines)
- `addons/website_partner/i18n/pt.po` (149 lines)
- `addons/website_partner/i18n/pt_BR.po` (153 lines)
- `addons/website_partner/i18n/ro.po` (150 lines)
- `addons/website_partner/i18n/ru.po` (148 lines)
- `addons/website_partner/i18n/sk.po` (146 lines)
- `addons/website_partner/i18n/sl.po` (150 lines)
- `addons/website_partner/i18n/sr@latin.po` (146 lines)
- `addons/website_partner/i18n/sv.po` (148 lines)
- `addons/website_partner/i18n/th.po` (146 lines)
- `addons/website_partner/i18n/tr.po` (151 lines)
- `addons/website_partner/i18n/uk.po` (149 lines)
- `addons/website_partner/i18n/uz.po` (167 lines)
- `addons/website_partner/i18n/vi.po` (148 lines)
- `addons/website_partner/i18n/website_partner.pot` (138 lines)
- `addons/website_partner/i18n/zh_CN.po` (151 lines)
- `addons/website_partner/i18n/zh_TW.po` (147 lines)
- `addons/website_partner/models/__init__.py` (3 lines)
- `addons/website_partner/models/res_partner.py` (80 lines)
- `addons/website_partner/static/description/icon.png` (20 lines)
- `addons/website_partner/static/description/icon.svg` (1 lines)
- `addons/website_partner/static/description/icon_hi.png` (67 lines)
- `addons/website_partner/views/res_partner_views.xml` (16 lines)
- `addons/website_partner/views/website_partner_templates.xml` (50 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
