# Module: website_mail_group

- **Module ID:** MOD-625
- **Path:** `addons/website_mail_group`
- **Manifest:** `addons/website_mail_group/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Add a website snippet for the mail groups.

No manifest description declared.

Declared dependencies: `mail_group`, `website`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 3 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mail_group",
    "website"
  ],
  "data": [
    "views/snippets/s_group.xml",
    "views/snippets/snippets.xml",
    "views/mail_group_views.xml",
    "views/website_mail_group_menus.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "website_mail_group/static/src/snippets/**/*.js",
      [
        "remove",
        "website_mail_group/static/src/**/*.edit.js"
      ]
    ],
    "website.assets_inside_builder_iframe": [
      "website_mail_group/static/src/**/*.edit.js"
    ],
    "website.website_builder_assets": [
      "website_mail_group/static/src/website_builder/**/*"
    ]
  }
}
```

### Representative source files

- `addons/website_mail_group/__init__.py` (5 lines)
- `addons/website_mail_group/__manifest__.py` (28 lines)
- `addons/website_mail_group/controllers/__init__.py` (4 lines)
- `addons/website_mail_group/controllers/main.py` (38 lines)
- `addons/website_mail_group/i18n/ar.po` (110 lines)
- `addons/website_mail_group/i18n/az.po` (106 lines)
- `addons/website_mail_group/i18n/bg.po` (106 lines)
- `addons/website_mail_group/i18n/bs.po` (107 lines)
- `addons/website_mail_group/i18n/ca.po` (110 lines)
- `addons/website_mail_group/i18n/cs.po` (106 lines)
- `addons/website_mail_group/i18n/da.po` (109 lines)
- `addons/website_mail_group/i18n/de.po` (109 lines)
- `addons/website_mail_group/i18n/el.po` (107 lines)
- `addons/website_mail_group/i18n/es.po` (109 lines)
- `addons/website_mail_group/i18n/es_419.po` (109 lines)
- `addons/website_mail_group/i18n/et.po` (106 lines)
- `addons/website_mail_group/i18n/fa.po` (106 lines)
- `addons/website_mail_group/i18n/fi.po` (109 lines)
- `addons/website_mail_group/i18n/fr.po` (109 lines)
- `addons/website_mail_group/i18n/he.po` (107 lines)
- `addons/website_mail_group/i18n/hi.po` (106 lines)
- `addons/website_mail_group/i18n/hr.po` (107 lines)
- `addons/website_mail_group/i18n/hu.po` (107 lines)
- `addons/website_mail_group/i18n/id.po` (109 lines)
- `addons/website_mail_group/i18n/it.po` (109 lines)
- `addons/website_mail_group/i18n/ja.po` (109 lines)
- `addons/website_mail_group/i18n/kab.po` (106 lines)
- `addons/website_mail_group/i18n/ko.po` (109 lines)
- `addons/website_mail_group/i18n/ku.po` (106 lines)
- `addons/website_mail_group/i18n/lo.po` (105 lines)
- `addons/website_mail_group/i18n/lt.po` (108 lines)
- `addons/website_mail_group/i18n/lv.po` (106 lines)
- `addons/website_mail_group/i18n/mn.po` (106 lines)
- `addons/website_mail_group/i18n/my.po` (106 lines)
- `addons/website_mail_group/i18n/nb.po` (106 lines)
- `addons/website_mail_group/i18n/nl.po` (109 lines)
- `addons/website_mail_group/i18n/pl.po` (108 lines)
- `addons/website_mail_group/i18n/pt.po` (109 lines)
- `addons/website_mail_group/i18n/pt_BR.po` (110 lines)
- `addons/website_mail_group/i18n/ro.po` (107 lines)
- `addons/website_mail_group/i18n/ru.po` (110 lines)
- `addons/website_mail_group/i18n/sk.po` (105 lines)
- `addons/website_mail_group/i18n/sl.po` (107 lines)
- `addons/website_mail_group/i18n/sr@latin.po` (107 lines)
- `addons/website_mail_group/i18n/sv.po` (107 lines)
- `addons/website_mail_group/i18n/th.po` (107 lines)
- `addons/website_mail_group/i18n/tr.po` (111 lines)
- `addons/website_mail_group/i18n/uk.po` (107 lines)
- `addons/website_mail_group/i18n/uz.po` (125 lines)
- `addons/website_mail_group/i18n/vi.po` (106 lines)
- `addons/website_mail_group/i18n/website_mail_group.pot` (102 lines)
- `addons/website_mail_group/i18n/zh_CN.po` (109 lines)
- `addons/website_mail_group/i18n/zh_TW.po` (112 lines)
- `addons/website_mail_group/models/__init__.py` (4 lines)
- `addons/website_mail_group/models/mail_group.py` (16 lines)
- `addons/website_mail_group/static/src/snippets/s_group/mail_group.edit.js` (25 lines)
- `addons/website_mail_group/static/src/snippets/s_group/mail_group.js` (59 lines)
- `addons/website_mail_group/static/src/website_builder/mail_group_option.xml` (24 lines)
- `addons/website_mail_group/static/src/website_builder/mail_group_option_plugin.js` (103 lines)
- `addons/website_mail_group/tests/__init__.py` (1 lines)
- `addons/website_mail_group/tests/test_website_groups_technical_page.py` (9 lines)
- `addons/website_mail_group/views/mail_group_views.xml` (18 lines)
- `addons/website_mail_group/views/snippets/s_group.xml` (16 lines)
- `addons/website_mail_group/views/snippets/snippets.xml` (12 lines)
- `addons/website_mail_group/views/website_mail_group_menus.xml` (18 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
