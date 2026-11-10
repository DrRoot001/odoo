# Module: website_hr_recruitment

- **Module ID:** MOD-620
- **Path:** `addons/website_hr_recruitment`
- **Manifest:** `addons/website_hr_recruitment/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `['hr_recruitment', 'website_mail']`
- **License:** `LGPL-3`

## Purpose and dependencies

Manage your online hiring process

This module allows to publish your available job positions on your website and keep track of application submissions easily.

Declared dependencies: `hr_recruitment`, `website_mail`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 15 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 7 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 11 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 7 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 5 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "hr_recruitment",
    "website_mail"
  ],
  "data": [
    "security/website_hr_recruitment_security.xml",
    "data/config_data.xml",
    "data/website_snippet_filter_data.xml",
    "views/website_hr_recruitment_templates.xml",
    "views/hr_recruitment_views.xml",
    "views/hr_job_views.xml",
    "views/website_pages_views.xml",
    "views/website_hr_recruitment_snippet_templates.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/hr_job_demo.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "website_hr_recruitment/static/src/scss/**/*",
      "website_hr_recruitment/static/src/interactions/*"
    ],
    "web.assets_backend": [
      "website_hr_recruitment/static/src/js/widgets/copy_link_menuitem.js",
      "website_hr_recruitment/static/src/js/widgets/copy_link_menuitem.xml"
    ],
    "website.website_builder_assets": [
      "website_hr_recruitment/static/src/js/website_hr_recruitment_editor.js",
      "website_hr_recruitment/static/src/website_builder/**/*"
    ],
    "website.assets_inside_builder_iframe": [
      "website_hr_recruitment/static/src/js/*.edit.*"
    ],
    "website.assets_editor": [
      "website_hr_recruitment/static/src/js/systray_items/new_content.js"
    ],
    "web.assets_tests": [
      "website_hr_recruitment/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/website_hr_recruitment/README.md` (69 lines)
- `addons/website_hr_recruitment/__init__.py` (5 lines)
- `addons/website_hr_recruitment/__manifest__.py` (52 lines)
- `addons/website_hr_recruitment/controllers/__init__.py` (1 lines)
- `addons/website_hr_recruitment/controllers/main.py` (221 lines)
- `addons/website_hr_recruitment/data/config_data.xml` (40 lines)
- `addons/website_hr_recruitment/data/hr_job_demo.xml` (1,300 lines)
- `addons/website_hr_recruitment/data/website_snippet_filter_data.xml` (19 lines)
- `addons/website_hr_recruitment/i18n/af.po` (1,058 lines)
- `addons/website_hr_recruitment/i18n/ar.po` (1,155 lines)
- `addons/website_hr_recruitment/i18n/az.po` (1,088 lines)
- `addons/website_hr_recruitment/i18n/bg.po` (1,094 lines)
- `addons/website_hr_recruitment/i18n/bs.po` (1,088 lines)
- `addons/website_hr_recruitment/i18n/ca.po` (1,139 lines)
- `addons/website_hr_recruitment/i18n/cs.po` (1,130 lines)
- `addons/website_hr_recruitment/i18n/da.po` (1,155 lines)
- `addons/website_hr_recruitment/i18n/de.po` (1,193 lines)
- `addons/website_hr_recruitment/i18n/el.po` (1,091 lines)
- `addons/website_hr_recruitment/i18n/es.po` (1,166 lines)
- `addons/website_hr_recruitment/i18n/es_419.po` (1,167 lines)
- `addons/website_hr_recruitment/i18n/et.po` (1,135 lines)
- `addons/website_hr_recruitment/i18n/fa.po` (1,134 lines)
- `addons/website_hr_recruitment/i18n/fi.po` (1,167 lines)
- `addons/website_hr_recruitment/i18n/fr.po` (1,179 lines)
- `addons/website_hr_recruitment/i18n/gu.po` (1,058 lines)
- `addons/website_hr_recruitment/i18n/he.po` (1,103 lines)
- `addons/website_hr_recruitment/i18n/hi.po` (1,093 lines)
- `addons/website_hr_recruitment/i18n/hr.po` (1,100 lines)
- `addons/website_hr_recruitment/i18n/hu.po` (1,100 lines)
- `addons/website_hr_recruitment/i18n/id.po` (1,166 lines)
- `addons/website_hr_recruitment/i18n/is.po` (1,054 lines)
- `addons/website_hr_recruitment/i18n/it.po` (1,168 lines)
- `addons/website_hr_recruitment/i18n/ja.po` (1,154 lines)
- `addons/website_hr_recruitment/i18n/kab.po` (1,085 lines)
- `addons/website_hr_recruitment/i18n/km.po` (1,059 lines)
- `addons/website_hr_recruitment/i18n/ko.po` (1,154 lines)
- `addons/website_hr_recruitment/i18n/ku.po` (1,085 lines)
- `addons/website_hr_recruitment/i18n/lo.po` (1,153 lines)
- `addons/website_hr_recruitment/i18n/lt.po` (1,100 lines)
- `addons/website_hr_recruitment/i18n/lv.po` (1,090 lines)
- `addons/website_hr_recruitment/i18n/mk.po` (1,061 lines)
- `addons/website_hr_recruitment/i18n/mn.po` (1,097 lines)
- `addons/website_hr_recruitment/i18n/my.po` (1,085 lines)
- `addons/website_hr_recruitment/i18n/nb.po` (1,091 lines)
- `addons/website_hr_recruitment/i18n/nl.po` (1,179 lines)
- `addons/website_hr_recruitment/i18n/pl.po` (1,180 lines)
- `addons/website_hr_recruitment/i18n/pt.po` (1,144 lines)
- `addons/website_hr_recruitment/i18n/pt_BR.po` (1,177 lines)
- `addons/website_hr_recruitment/i18n/ro.po` (1,160 lines)
- `addons/website_hr_recruitment/i18n/ru.po` (1,160 lines)
- `addons/website_hr_recruitment/i18n/sk.po` (1,101 lines)
- `addons/website_hr_recruitment/i18n/sl.po` (1,096 lines)
- `addons/website_hr_recruitment/i18n/sr@latin.po` (1,107 lines)
- `addons/website_hr_recruitment/i18n/sv.po` (1,161 lines)
- `addons/website_hr_recruitment/i18n/th.po` (1,141 lines)
- `addons/website_hr_recruitment/i18n/tr.po` (1,172 lines)
- `addons/website_hr_recruitment/i18n/uk.po` (1,139 lines)
- `addons/website_hr_recruitment/i18n/uz.po` (1,283 lines)
- `addons/website_hr_recruitment/i18n/vi.po` (1,162 lines)
- `addons/website_hr_recruitment/i18n/website_hr_recruitment.pot` (1,069 lines)
- `addons/website_hr_recruitment/i18n/zh_CN.po` (1,153 lines)
- `addons/website_hr_recruitment/i18n/zh_TW.po` (1,147 lines)
- `addons/website_hr_recruitment/migrations/17.0.1.1/pre-migrate.py` (13 lines)
- `addons/website_hr_recruitment/models/__init__.py` (8 lines)
- `addons/website_hr_recruitment/models/hr_applicant.py` (24 lines)
- `addons/website_hr_recruitment/models/hr_department.py` (10 lines)
- `addons/website_hr_recruitment/models/hr_job.py` (246 lines)
- `addons/website_hr_recruitment/models/hr_recruitment_source.py` (24 lines)
- `addons/website_hr_recruitment/models/website.py` (25 lines)
- `addons/website_hr_recruitment/models/website_published_multi_mixin.py` (20 lines)
- `addons/website_hr_recruitment/security/ir.access.csv` (4 lines)
- `addons/website_hr_recruitment/security/website_hr_recruitment_security.xml` (5 lines)
- `addons/website_hr_recruitment/static/description/icon.png` (10 lines)
- `addons/website_hr_recruitment/static/description/icon.svg` (1 lines)
- `addons/website_hr_recruitment/static/description/icon_hi.png` (54 lines)
- `addons/website_hr_recruitment/static/src/img/1010054_10151543538268963_186969588_n.jpg` (301 lines)
- `addons/website_hr_recruitment/static/src/img/1017407_10151536656083963_857938319_n.jpg` (525 lines)
- `addons/website_hr_recruitment/static/src/img/1044326_10151536655788963_587131144_n.jpg` (465 lines)
- `addons/website_hr_recruitment/static/src/img/882207_10151545507603963_1381082528_o.jpg` (3,979 lines)
- `addons/website_hr_recruitment/static/src/img/job_congratulations.svg` (63 lines)
- `addons/website_hr_recruitment/static/src/img/job_image_1.jpg` (930 lines)
- `addons/website_hr_recruitment/static/src/img/job_image_10.jpg` (681 lines)
- `addons/website_hr_recruitment/static/src/img/job_image_11.jpg` (696 lines)
- `addons/website_hr_recruitment/static/src/img/job_image_12.jpg` (863 lines)
- `addons/website_hr_recruitment/static/src/img/job_image_13.jpg` (564 lines)
- `addons/website_hr_recruitment/static/src/img/job_image_2.jpg` (1,366 lines)
- `addons/website_hr_recruitment/static/src/img/job_image_3.jpg` (1,076 lines)
- `addons/website_hr_recruitment/static/src/img/job_image_4.jpg` (1,167 lines)
- `addons/website_hr_recruitment/static/src/img/job_image_5.jpg` (1,228 lines)
- `addons/website_hr_recruitment/static/src/img/job_image_6.jpg` (1,123 lines)
- `addons/website_hr_recruitment/static/src/img/job_image_7.jpg` (710 lines)
- `addons/website_hr_recruitment/static/src/img/job_image_8.jpg` (699 lines)
- `addons/website_hr_recruitment/static/src/img/job_image_9.jpg` (509 lines)
- `addons/website_hr_recruitment/static/src/img/job_not_found.svg` (50 lines)
- `addons/website_hr_recruitment/static/src/img/job_product.svg` (51 lines)
- `addons/website_hr_recruitment/static/src/img/ui/s_hr_rating_thumb.jpg` (41 lines)
- `addons/website_hr_recruitment/static/src/interactions/hr_recruitment_form.js` (68 lines)
- `addons/website_hr_recruitment/static/src/js/systray_items/new_content.js` (43 lines)
- `addons/website_hr_recruitment/static/src/js/website_hr_recruitment_editor.edit.js` (38 lines)
- `addons/website_hr_recruitment/static/src/js/website_hr_recruitment_editor.js` (17 lines)
- `addons/website_hr_recruitment/static/src/js/widgets/copy_link_menuitem.js` (35 lines)
- `addons/website_hr_recruitment/static/src/js/widgets/copy_link_menuitem.xml` (20 lines)
- `addons/website_hr_recruitment/static/src/scss/website_hr_recruitment.scss` (66 lines)
- `addons/website_hr_recruitment/static/src/website_builder/website_hr_recruitment_floating_snippets_plugin.js` (32 lines)
- `addons/website_hr_recruitment/static/src/website_builder/website_hr_recruitment_option.xml` (45 lines)
- `addons/website_hr_recruitment/static/tests/tours/website_hr_recruitment.js` (158 lines)
- `addons/website_hr_recruitment/tests/__init__.py` (2 lines)
- `addons/website_hr_recruitment/tests/test_website_hr_recruitment.py` (200 lines)
- `addons/website_hr_recruitment/tests/test_website_hr_recruitment_technical_page.py` (9 lines)
- `addons/website_hr_recruitment/views/hr_job_views.xml` (74 lines)
- `addons/website_hr_recruitment/views/hr_recruitment_views.xml` (62 lines)
- `addons/website_hr_recruitment/views/website_hr_recruitment_snippet_templates.xml` (34 lines)
- `addons/website_hr_recruitment/views/website_hr_recruitment_templates.xml` (1,089 lines)
- `addons/website_hr_recruitment/views/website_pages_views.xml` (66 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
