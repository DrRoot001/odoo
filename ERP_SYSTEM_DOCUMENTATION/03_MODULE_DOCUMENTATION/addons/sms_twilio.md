# Module: sms_twilio

- **Module ID:** MOD-540
- **Path:** `addons/sms_twilio`
- **Manifest:** `addons/sms_twilio/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Send SMS messages using Twilio


This module allows using Twilio as a provider for SMS messaging.
The user has to create an account on twilio.com and top
up their account to start sending SMS messages.


Declared dependencies: `sms`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 22 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 8 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "sms"
  ],
  "data": [
    "views/res_config_settings_views.xml",
    "views/sms_sms_views.xml",
    "wizard/sms_twilio_account_manage_views.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_backend": [
      "sms_twilio/static/src/**/*"
    ]
  }
}
```

### Representative source files

- `addons/sms_twilio/__init__.py` (3 lines)
- `addons/sms_twilio/__manifest__.py` (26 lines)
- `addons/sms_twilio/controllers/__init__.py` (1 lines)
- `addons/sms_twilio/controllers/controllers.py` (86 lines)
- `addons/sms_twilio/data/neutralize.sql` (2 lines)
- `addons/sms_twilio/i18n/ar.po` (441 lines)
- `addons/sms_twilio/i18n/az.po` (434 lines)
- `addons/sms_twilio/i18n/bg.po` (434 lines)
- `addons/sms_twilio/i18n/bs.po` (433 lines)
- `addons/sms_twilio/i18n/ca.po` (436 lines)
- `addons/sms_twilio/i18n/cs.po` (434 lines)
- `addons/sms_twilio/i18n/da.po` (435 lines)
- `addons/sms_twilio/i18n/de.po` (448 lines)
- `addons/sms_twilio/i18n/el.po` (432 lines)
- `addons/sms_twilio/i18n/es.po` (449 lines)
- `addons/sms_twilio/i18n/es_419.po` (445 lines)
- `addons/sms_twilio/i18n/et.po` (434 lines)
- `addons/sms_twilio/i18n/fa.po` (434 lines)
- `addons/sms_twilio/i18n/fi.po` (439 lines)
- `addons/sms_twilio/i18n/fr.po` (443 lines)
- `addons/sms_twilio/i18n/he.po` (435 lines)
- `addons/sms_twilio/i18n/hi.po` (434 lines)
- `addons/sms_twilio/i18n/hr.po` (435 lines)
- `addons/sms_twilio/i18n/hu.po` (434 lines)
- `addons/sms_twilio/i18n/id.po` (439 lines)
- `addons/sms_twilio/i18n/it.po` (448 lines)
- `addons/sms_twilio/i18n/ja.po` (441 lines)
- `addons/sms_twilio/i18n/kab.po` (432 lines)
- `addons/sms_twilio/i18n/ko.po` (441 lines)
- `addons/sms_twilio/i18n/ku.po` (432 lines)
- `addons/sms_twilio/i18n/lo.po` (444 lines)
- `addons/sms_twilio/i18n/lt.po` (436 lines)
- `addons/sms_twilio/i18n/lv.po` (432 lines)
- `addons/sms_twilio/i18n/mn.po` (434 lines)
- `addons/sms_twilio/i18n/my.po` (433 lines)
- `addons/sms_twilio/i18n/nb.po` (434 lines)
- `addons/sms_twilio/i18n/nl.po` (443 lines)
- `addons/sms_twilio/i18n/pl.po` (436 lines)
- `addons/sms_twilio/i18n/pt.po` (435 lines)
- `addons/sms_twilio/i18n/pt_BR.po` (450 lines)
- `addons/sms_twilio/i18n/ro.po` (435 lines)
- `addons/sms_twilio/i18n/ru.po` (447 lines)
- `addons/sms_twilio/i18n/sk.po` (431 lines)
- `addons/sms_twilio/i18n/sl.po` (435 lines)
- `addons/sms_twilio/i18n/sms_twilio.pot` (427 lines)
- `addons/sms_twilio/i18n/sr@latin.po` (435 lines)
- `addons/sms_twilio/i18n/sv.po` (435 lines)
- `addons/sms_twilio/i18n/th.po` (435 lines)
- `addons/sms_twilio/i18n/tr.po` (443 lines)
- `addons/sms_twilio/i18n/uk.po` (435 lines)
- `addons/sms_twilio/i18n/uz.po` (506 lines)
- `addons/sms_twilio/i18n/vi.po` (436 lines)
- `addons/sms_twilio/i18n/zh_CN.po` (444 lines)
- `addons/sms_twilio/i18n/zh_TW.po` (438 lines)
- `addons/sms_twilio/models/__init__.py` (7 lines)
- `addons/sms_twilio/models/mail_notification.py` (15 lines)
- `addons/sms_twilio/models/res_company.py` (48 lines)
- `addons/sms_twilio/models/res_config_settings.py` (10 lines)
- `addons/sms_twilio/models/sms_composer.py` (16 lines)
- `addons/sms_twilio/models/sms_sms.py` (74 lines)
- `addons/sms_twilio/models/sms_tracker.py` (7 lines)
- `addons/sms_twilio/models/sms_twilio_number.py` (20 lines)
- `addons/sms_twilio/security/ir.access.csv` (3 lines)
- `addons/sms_twilio/static/src/core/notification_model.js` (24 lines)
- `addons/sms_twilio/tests/__init__.py` (3 lines)
- `addons/sms_twilio/tests/common.py` (257 lines)
- `addons/sms_twilio/tests/test_sms_twilio.py` (213 lines)
- `addons/sms_twilio/tests/test_sms_twilio_controller.py` (119 lines)
- `addons/sms_twilio/tests/test_twilio_account_manage.py` (84 lines)
- `addons/sms_twilio/tools/__init__.py` (2 lines)
- `addons/sms_twilio/tools/sms_api.py` (120 lines)
- `addons/sms_twilio/tools/sms_twilio.py` (42 lines)
- `addons/sms_twilio/views/res_config_settings_views.xml` (24 lines)
- `addons/sms_twilio/views/sms_sms_views.xml` (15 lines)
- `addons/sms_twilio/wizard/__init__.py` (1 lines)
- `addons/sms_twilio/wizard/sms_twilio_account_manage.py` (115 lines)
- `addons/sms_twilio/wizard/sms_twilio_account_manage_views.xml` (52 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
