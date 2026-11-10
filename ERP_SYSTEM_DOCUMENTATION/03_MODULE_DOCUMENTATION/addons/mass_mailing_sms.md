# Module: mass_mailing_sms

- **Module ID:** MOD-372
- **Path:** `addons/mass_mailing_sms`
- **Manifest:** `addons/mass_mailing_sms/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Design, send and track SMS

No manifest description declared.

Declared dependencies: `portal`, `mass_mailing`, `sms`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 29 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 12 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 16 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 9 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 3 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "portal",
    "mass_mailing",
    "sms"
  ],
  "data": [
    "data/utm_data.xml",
    "report/mailing_trace_report_views.xml",
    "views/link_tracker_views.xml",
    "views/mailing_list_views.xml",
    "views/mailing_contact_views.xml",
    "views/mailing_trace_views.xml",
    "views/mailing_mailing_views.xml",
    "views/mass_mailing_sms_templates_portal.xml",
    "views/utm_campaign_views.xml",
    "views/mailing_sms_menus.xml",
    "wizard/sms_composer_views.xml",
    "wizard/mailing_sms_test_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "demo/mailing_list_contact.xml",
    "demo/mailing_subscription.xml",
    "demo/mailing_mailing.xml",
    "demo/mailing_trace.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "mass_mailing_sms/static/src/**"
    ],
    "web.assets_tests": [
      "mass_mailing_sms/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/mass_mailing_sms/__init__.py` (6 lines)
- `addons/mass_mailing_sms/__manifest__.py` (48 lines)
- `addons/mass_mailing_sms/controllers/__init__.py` (4 lines)
- `addons/mass_mailing_sms/controllers/main.py` (142 lines)
- `addons/mass_mailing_sms/data/utm_data.xml` (12 lines)
- `addons/mass_mailing_sms/demo/mailing_list_contact.xml` (35 lines)
- `addons/mass_mailing_sms/demo/mailing_mailing.xml` (32 lines)
- `addons/mass_mailing_sms/demo/mailing_subscription.xml` (23 lines)
- `addons/mass_mailing_sms/demo/mailing_trace.xml` (158 lines)
- `addons/mass_mailing_sms/i18n/ar.po` (1,184 lines)
- `addons/mass_mailing_sms/i18n/az.po` (1,123 lines)
- `addons/mass_mailing_sms/i18n/bg.po` (1,122 lines)
- `addons/mass_mailing_sms/i18n/bs.po` (1,105 lines)
- `addons/mass_mailing_sms/i18n/ca.po` (1,165 lines)
- `addons/mass_mailing_sms/i18n/cs.po` (1,151 lines)
- `addons/mass_mailing_sms/i18n/da.po` (1,143 lines)
- `addons/mass_mailing_sms/i18n/de.po` (1,164 lines)
- `addons/mass_mailing_sms/i18n/el.po` (1,111 lines)
- `addons/mass_mailing_sms/i18n/es.po` (1,194 lines)
- `addons/mass_mailing_sms/i18n/es_419.po` (1,157 lines)
- `addons/mass_mailing_sms/i18n/et.po` (1,143 lines)
- `addons/mass_mailing_sms/i18n/fa.po` (1,121 lines)
- `addons/mass_mailing_sms/i18n/fi.po` (1,186 lines)
- `addons/mass_mailing_sms/i18n/fr.po` (1,163 lines)
- `addons/mass_mailing_sms/i18n/he.po` (1,151 lines)
- `addons/mass_mailing_sms/i18n/hi.po` (1,110 lines)
- `addons/mass_mailing_sms/i18n/hr.po` (1,130 lines)
- `addons/mass_mailing_sms/i18n/hu.po` (1,121 lines)
- `addons/mass_mailing_sms/i18n/id.po` (1,183 lines)
- `addons/mass_mailing_sms/i18n/it.po` (1,163 lines)
- `addons/mass_mailing_sms/i18n/ja.po` (1,152 lines)
- `addons/mass_mailing_sms/i18n/kab.po` (1,104 lines)
- `addons/mass_mailing_sms/i18n/ko.po` (1,176 lines)
- `addons/mass_mailing_sms/i18n/ku.po` (1,110 lines)
- `addons/mass_mailing_sms/i18n/lb.po` (1,096 lines)
- `addons/mass_mailing_sms/i18n/lo.po` (1,132 lines)
- `addons/mass_mailing_sms/i18n/lt.po` (1,130 lines)
- `addons/mass_mailing_sms/i18n/lv.po` (1,104 lines)
- `addons/mass_mailing_sms/i18n/mass_mailing_sms.pot` (1,097 lines)
- `addons/mass_mailing_sms/i18n/mn.po` (1,124 lines)
- `addons/mass_mailing_sms/i18n/my.po` (1,106 lines)
- `addons/mass_mailing_sms/i18n/nb.po` (1,116 lines)
- `addons/mass_mailing_sms/i18n/nl.po` (1,163 lines)
- `addons/mass_mailing_sms/i18n/pl.po` (1,176 lines)
- `addons/mass_mailing_sms/i18n/pt.po` (1,160 lines)
- `addons/mass_mailing_sms/i18n/pt_BR.po` (1,167 lines)
- `addons/mass_mailing_sms/i18n/ro.po` (1,189 lines)
- `addons/mass_mailing_sms/i18n/ru.po` (1,192 lines)
- `addons/mass_mailing_sms/i18n/sk.po` (1,103 lines)
- `addons/mass_mailing_sms/i18n/sl.po` (1,123 lines)
- `addons/mass_mailing_sms/i18n/sr@latin.po` (1,121 lines)
- `addons/mass_mailing_sms/i18n/sv.po` (1,180 lines)
- `addons/mass_mailing_sms/i18n/th.po` (1,166 lines)
- `addons/mass_mailing_sms/i18n/tr.po` (1,205 lines)
- `addons/mass_mailing_sms/i18n/uk.po` (1,175 lines)
- `addons/mass_mailing_sms/i18n/uz.po` (1,367 lines)
- `addons/mass_mailing_sms/i18n/vi.po` (1,184 lines)
- `addons/mass_mailing_sms/i18n/zh_CN.po` (1,174 lines)
- `addons/mass_mailing_sms/i18n/zh_TW.po` (1,165 lines)
- `addons/mass_mailing_sms/models/__init__.py` (14 lines)
- `addons/mass_mailing_sms/models/link_tracker.py` (9 lines)
- `addons/mass_mailing_sms/models/mailing_contact.py` (21 lines)
- `addons/mass_mailing_sms/models/mailing_list.py` (96 lines)
- `addons/mass_mailing_sms/models/mailing_mailing.py` (391 lines)
- `addons/mass_mailing_sms/models/mailing_trace.py` (78 lines)
- `addons/mass_mailing_sms/models/res_partner.py` (11 lines)
- `addons/mass_mailing_sms/models/res_users.py` (54 lines)
- `addons/mass_mailing_sms/models/sms_sms.py` (33 lines)
- `addons/mass_mailing_sms/models/sms_tracker.py` (86 lines)
- `addons/mass_mailing_sms/models/utm_campaign.py` (74 lines)
- `addons/mass_mailing_sms/models/utm_mixin.py` (14 lines)
- `addons/mass_mailing_sms/report/mailing_trace_report_views.xml` (84 lines)
- `addons/mass_mailing_sms/security/ir.access.csv` (4 lines)
- `addons/mass_mailing_sms/static/description/icon.png` (12 lines)
- `addons/mass_mailing_sms/static/description/icon.svg` (1 lines)
- `addons/mass_mailing_sms/static/description/icon_hi.png` (71 lines)
- `addons/mass_mailing_sms/static/src/components/sms_widget/fields_sms_widget.js` (74 lines)
- `addons/mass_mailing_sms/static/tests/tours/mailing_activities_split.js` (38 lines)
- `addons/mass_mailing_sms/tests/__init__.py` (11 lines)
- `addons/mass_mailing_sms/tests/common.py` (305 lines)
- `addons/mass_mailing_sms/tests/test_mailing_contact_to_list.py` (55 lines)
- `addons/mass_mailing_sms/tests/test_mailing_controllers.py` (37 lines)
- `addons/mass_mailing_sms/tests/test_mailing_internals.py` (103 lines)
- `addons/mass_mailing_sms/tests/test_mailing_list.py` (28 lines)
- `addons/mass_mailing_sms/tests/test_mailing_retry.py` (42 lines)
- `addons/mass_mailing_sms/tests/test_mailing_sms_ab_testing.py` (35 lines)
- `addons/mass_mailing_sms/tests/test_mailing_ui.py` (41 lines)
- `addons/mass_mailing_sms/views/link_tracker_views.xml` (16 lines)
- `addons/mass_mailing_sms/views/mailing_contact_views.xml` (94 lines)
- `addons/mass_mailing_sms/views/mailing_list_views.xml` (37 lines)
- `addons/mass_mailing_sms/views/mailing_mailing_views.xml` (273 lines)
- `addons/mass_mailing_sms/views/mailing_sms_menus.xml` (75 lines)
- `addons/mass_mailing_sms/views/mailing_trace_views.xml` (147 lines)
- `addons/mass_mailing_sms/views/mass_mailing_sms_templates_portal.xml` (60 lines)
- `addons/mass_mailing_sms/views/utm_campaign_views.xml` (69 lines)
- `addons/mass_mailing_sms/wizard/__init__.py` (6 lines)
- `addons/mass_mailing_sms/wizard/mailing_contact_to_list.py` (10 lines)
- `addons/mass_mailing_sms/wizard/mailing_sms_test.py` (117 lines)
- `addons/mass_mailing_sms/wizard/mailing_sms_test_views.xml` (29 lines)
- `addons/mass_mailing_sms/wizard/sms_composer.py` (126 lines)
- `addons/mass_mailing_sms/wizard/sms_composer_views.xml` (16 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
