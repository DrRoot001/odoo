# Module: social_media

- **Module ID:** MOD-543
- **Path:** `addons/social_media`
- **Manifest:** `addons/social_media/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Social media connectors for company settings.


The purpose of this technical module is to provide a front for
social media configuration for any other module that might need it.
    

Declared dependencies: `base`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base"
  ],
  "data": [
    "views/res_company_views.xml"
  ],
  "demo": [
    "demo/res_company_demo.xml"
  ]
}
```

### Representative source files

- `addons/social_media/__init__.py` (3 lines)
- `addons/social_media/__manifest__.py` (22 lines)
- `addons/social_media/demo/res_company_demo.xml` (13 lines)
- `addons/social_media/i18n/ar.po` (98 lines)
- `addons/social_media/i18n/az.po` (97 lines)
- `addons/social_media/i18n/bg.po` (94 lines)
- `addons/social_media/i18n/bs.po` (97 lines)
- `addons/social_media/i18n/ca.po` (100 lines)
- `addons/social_media/i18n/cs.po` (98 lines)
- `addons/social_media/i18n/da.po` (99 lines)
- `addons/social_media/i18n/de.po` (102 lines)
- `addons/social_media/i18n/el.po` (98 lines)
- `addons/social_media/i18n/es.po` (103 lines)
- `addons/social_media/i18n/es_419.po` (96 lines)
- `addons/social_media/i18n/et.po` (98 lines)
- `addons/social_media/i18n/fa.po` (97 lines)
- `addons/social_media/i18n/fi.po` (99 lines)
- `addons/social_media/i18n/fr.po` (100 lines)
- `addons/social_media/i18n/gu.po` (94 lines)
- `addons/social_media/i18n/he.po` (101 lines)
- `addons/social_media/i18n/hi.po` (94 lines)
- `addons/social_media/i18n/hr.po` (100 lines)
- `addons/social_media/i18n/hu.po` (97 lines)
- `addons/social_media/i18n/id.po` (95 lines)
- `addons/social_media/i18n/is.po` (90 lines)
- `addons/social_media/i18n/it.po` (103 lines)
- `addons/social_media/i18n/ja.po` (98 lines)
- `addons/social_media/i18n/kab.po` (94 lines)
- `addons/social_media/i18n/km.po` (93 lines)
- `addons/social_media/i18n/ko.po` (98 lines)
- `addons/social_media/i18n/ku.po` (94 lines)
- `addons/social_media/i18n/lo.po` (93 lines)
- `addons/social_media/i18n/lt.po` (101 lines)
- `addons/social_media/i18n/lv.po` (94 lines)
- `addons/social_media/i18n/mn.po` (97 lines)
- `addons/social_media/i18n/my.po` (94 lines)
- `addons/social_media/i18n/nb.po` (98 lines)
- `addons/social_media/i18n/nl.po` (98 lines)
- `addons/social_media/i18n/pl.po` (101 lines)
- `addons/social_media/i18n/pt.po` (100 lines)
- `addons/social_media/i18n/pt_BR.po` (104 lines)
- `addons/social_media/i18n/ro.po` (101 lines)
- `addons/social_media/i18n/ru.po` (99 lines)
- `addons/social_media/i18n/sk.po` (97 lines)
- `addons/social_media/i18n/sl.po` (96 lines)
- `addons/social_media/i18n/social_media.pot` (90 lines)
- `addons/social_media/i18n/sr@latin.po` (97 lines)
- `addons/social_media/i18n/sv.po` (100 lines)
- `addons/social_media/i18n/th.po` (99 lines)
- `addons/social_media/i18n/tr.po` (101 lines)
- `addons/social_media/i18n/uk.po` (101 lines)
- `addons/social_media/i18n/uz.po` (112 lines)
- `addons/social_media/i18n/vi.po` (98 lines)
- `addons/social_media/i18n/zh_CN.po` (101 lines)
- `addons/social_media/i18n/zh_TW.po` (98 lines)
- `addons/social_media/models/__init__.py` (3 lines)
- `addons/social_media/models/res_company.py` (17 lines)
- `addons/social_media/views/res_company_views.xml` (23 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
