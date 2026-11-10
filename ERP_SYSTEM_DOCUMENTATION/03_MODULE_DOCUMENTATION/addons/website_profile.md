# Module: website_profile

- **Module ID:** MOD-632
- **Path:** `addons/website_profile`
- **Manifest:** `addons/website_profile/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Access the website profile of the users

Allows to access the website profile of the users and see their statistics (karma, badges, etc..)

Declared dependencies: `html_editor`, `website_partner`, `gamification`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 12 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 5 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 8 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "html_editor",
    "website_partner",
    "gamification"
  ],
  "data": [
    "data/mail_template_data.xml",
    "views/gamification_badge_views.xml",
    "views/website_profile.xml",
    "views/website_views.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_frontend": [
      "web/static/src/views/fields/file_handler.*",
      "website_profile/static/src/scss/website_profile.scss",
      "website_profile/static/src/components/**/*",
      "website_profile/static/src/interactions/**/*",
      [
        "remove",
        "website_profile/static/src/interactions/**/*.edit.js"
      ],
      [
        "include",
        "html_editor.assets_editor"
      ]
    ],
    "website.assets_inside_builder_iframe": [
      "website_profile/static/src/**/*.edit.js"
    ],
    "web.assets_tests": [
      "website_profile/static/tests/tours/tour_website_profile_description.js"
    ]
  }
}
```

### Representative source files

- `addons/website_profile/__init__.py` (5 lines)
- `addons/website_profile/__manifest__.py` (38 lines)
- `addons/website_profile/controllers/__init__.py` (5 lines)
- `addons/website_profile/controllers/main.py` (338 lines)
- `addons/website_profile/controllers/portal.py` (19 lines)
- `addons/website_profile/data/mail_template_data.xml` (33 lines)
- `addons/website_profile/i18n/ar.po` (704 lines)
- `addons/website_profile/i18n/az.po` (679 lines)
- `addons/website_profile/i18n/bg.po` (679 lines)
- `addons/website_profile/i18n/bs.po` (681 lines)
- `addons/website_profile/i18n/ca.po` (737 lines)
- `addons/website_profile/i18n/cs.po` (699 lines)
- `addons/website_profile/i18n/da.po` (698 lines)
- `addons/website_profile/i18n/de.po` (757 lines)
- `addons/website_profile/i18n/el.po` (681 lines)
- `addons/website_profile/i18n/es.po` (754 lines)
- `addons/website_profile/i18n/es_419.po` (747 lines)
- `addons/website_profile/i18n/et.po` (680 lines)
- `addons/website_profile/i18n/fa.po` (679 lines)
- `addons/website_profile/i18n/fi.po` (745 lines)
- `addons/website_profile/i18n/fr.po` (752 lines)
- `addons/website_profile/i18n/he.po` (691 lines)
- `addons/website_profile/i18n/hi.po` (679 lines)
- `addons/website_profile/i18n/hr.po` (694 lines)
- `addons/website_profile/i18n/hu.po` (704 lines)
- `addons/website_profile/i18n/id.po` (741 lines)
- `addons/website_profile/i18n/it.po` (749 lines)
- `addons/website_profile/i18n/ja.po` (740 lines)
- `addons/website_profile/i18n/kab.po` (680 lines)
- `addons/website_profile/i18n/ko.po` (696 lines)
- `addons/website_profile/i18n/ku.po` (679 lines)
- `addons/website_profile/i18n/lo.po` (739 lines)
- `addons/website_profile/i18n/lt.po` (693 lines)
- `addons/website_profile/i18n/lv.po` (680 lines)
- `addons/website_profile/i18n/mn.po` (686 lines)
- `addons/website_profile/i18n/my.po` (679 lines)
- `addons/website_profile/i18n/nb.po` (690 lines)
- `addons/website_profile/i18n/nl.po` (750 lines)
- `addons/website_profile/i18n/pl.po` (759 lines)
- `addons/website_profile/i18n/pt.po` (745 lines)
- `addons/website_profile/i18n/pt_BR.po` (751 lines)
- `addons/website_profile/i18n/ro.po` (704 lines)
- `addons/website_profile/i18n/ru.po` (704 lines)
- `addons/website_profile/i18n/sk.po` (679 lines)
- `addons/website_profile/i18n/sl.po` (695 lines)
- `addons/website_profile/i18n/sr@latin.po` (681 lines)
- `addons/website_profile/i18n/sv.po` (699 lines)
- `addons/website_profile/i18n/th.po` (733 lines)
- `addons/website_profile/i18n/tr.po` (716 lines)
- `addons/website_profile/i18n/uk.po` (694 lines)
- `addons/website_profile/i18n/uz.po` (796 lines)
- `addons/website_profile/i18n/vi.po` (742 lines)
- `addons/website_profile/i18n/website_profile.pot` (667 lines)
- `addons/website_profile/i18n/zh_CN.po` (739 lines)
- `addons/website_profile/i18n/zh_TW.po` (696 lines)
- `addons/website_profile/models/__init__.py` (6 lines)
- `addons/website_profile/models/gamification_badge.py` (9 lines)
- `addons/website_profile/models/res_users.py` (73 lines)
- `addons/website_profile/models/website.py` (10 lines)
- `addons/website_profile/security/ir.access.csv` (2 lines)
- `addons/website_profile/static/src/components/profile_dialog/profile_dialog.js` (178 lines)
- `addons/website_profile/static/src/components/profile_dialog/profile_dialog.xml` (81 lines)
- `addons/website_profile/static/src/img/badge_bronze.svg` (1 lines)
- `addons/website_profile/static/src/img/badge_gold.svg` (1 lines)
- `addons/website_profile/static/src/img/badge_silver.svg` (1 lines)
- `addons/website_profile/static/src/img/rank_1.svg` (1 lines)
- `addons/website_profile/static/src/img/rank_2.svg` (1 lines)
- `addons/website_profile/static/src/img/rank_3.svg` (1 lines)
- `addons/website_profile/static/src/interactions/profile_editor.edit.js` (14 lines)
- `addons/website_profile/static/src/interactions/profile_editor.js` (30 lines)
- `addons/website_profile/static/src/interactions/profile_validation.js` (33 lines)
- `addons/website_profile/static/src/scss/website_profile.scss` (282 lines)
- `addons/website_profile/static/tests/tours/tour_website_profile_description.js` (82 lines)
- `addons/website_profile/tests/__init__.py` (3 lines)
- `addons/website_profile/tests/test_website_profile.py` (136 lines)
- `addons/website_profile/tests/test_website_profile_technical_page.py` (9 lines)
- `addons/website_profile/views/gamification_badge_views.xml` (15 lines)
- `addons/website_profile/views/website_profile.xml` (583 lines)
- `addons/website_profile/views/website_views.xml` (15 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
