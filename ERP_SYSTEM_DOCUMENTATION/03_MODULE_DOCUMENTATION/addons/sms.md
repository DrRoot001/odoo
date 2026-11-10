# Module: sms

- **Module ID:** MOD-539
- **Path:** `addons/sms`
- **Manifest:** `addons/sms/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

SMS Text Messaging


This module gives a framework for SMS text messaging
----------------------------------------------------

The service is provided by the In App Purchase Odoo platform.


Declared dependencies: `base`, `iap_mail`, `mail`, `phone_validation`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 31 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 13 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 20 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 15 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base",
    "iap_mail",
    "mail",
    "phone_validation"
  ],
  "data": [
    "data/iap_service_data.xml",
    "data/ir_cron_data.xml",
    "wizard/sms_account_code_views.xml",
    "wizard/sms_account_phone_views.xml",
    "wizard/sms_account_sender_views.xml",
    "wizard/sms_composer_views.xml",
    "wizard/sms_template_preview_views.xml",
    "wizard/sms_template_reset_views.xml",
    "views/ir_actions_server_views.xml",
    "views/mail_notification_views.xml",
    "views/res_config_settings_views.xml",
    "views/res_partner_views.xml",
    "views/iap_account_views.xml",
    "views/sms_sms_views.xml",
    "views/sms_template_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/sms_demo.xml",
    "data/mail_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "sms/static/src/**/*"
    ],
    "web.assets_unit_tests": [
      "sms/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/sms/__init__.py` (7 lines)
- `addons/sms/__manifest__.py` (54 lines)
- `addons/sms/controllers/__init__.py` (3 lines)
- `addons/sms/controllers/main.py` (48 lines)
- `addons/sms/data/iap_service_data.xml` (12 lines)
- `addons/sms/data/ir_cron_data.xml` (12 lines)
- `addons/sms/data/mail_demo.xml` (90 lines)
- `addons/sms/data/sms_demo.xml` (8 lines)
- `addons/sms/i18n/ar.po` (1,738 lines)
- `addons/sms/i18n/az.po` (1,660 lines)
- `addons/sms/i18n/bg.po` (1,659 lines)
- `addons/sms/i18n/bs.po` (1,652 lines)
- `addons/sms/i18n/ca.po` (1,699 lines)
- `addons/sms/i18n/cs.po` (1,709 lines)
- `addons/sms/i18n/da.po` (1,698 lines)
- `addons/sms/i18n/de.po` (1,771 lines)
- `addons/sms/i18n/el.po` (1,660 lines)
- `addons/sms/i18n/es.po` (1,766 lines)
- `addons/sms/i18n/es_419.po` (1,753 lines)
- `addons/sms/i18n/et.po` (1,694 lines)
- `addons/sms/i18n/fa.po` (1,696 lines)
- `addons/sms/i18n/fi.po` (1,757 lines)
- `addons/sms/i18n/fr.po` (1,760 lines)
- `addons/sms/i18n/gu.po` (1,551 lines)
- `addons/sms/i18n/he.po` (1,673 lines)
- `addons/sms/i18n/hi.po` (1,654 lines)
- `addons/sms/i18n/hr.po` (1,672 lines)
- `addons/sms/i18n/hu.po` (1,667 lines)
- `addons/sms/i18n/id.po` (1,743 lines)
- `addons/sms/i18n/is.po` (1,547 lines)
- `addons/sms/i18n/it.po` (1,760 lines)
- `addons/sms/i18n/ja.po` (1,726 lines)
- `addons/sms/i18n/kab.po` (1,648 lines)
- `addons/sms/i18n/km.po` (1,550 lines)
- `addons/sms/i18n/ko.po` (1,721 lines)
- `addons/sms/i18n/ku.po` (1,654 lines)
- `addons/sms/i18n/lo.po` (1,711 lines)
- `addons/sms/i18n/lt.po` (1,677 lines)
- `addons/sms/i18n/lv.po` (1,657 lines)
- `addons/sms/i18n/mn.po` (1,668 lines)
- `addons/sms/i18n/my.po` (1,656 lines)
- `addons/sms/i18n/nb.po` (1,665 lines)
- `addons/sms/i18n/nl.po` (1,762 lines)
- `addons/sms/i18n/pl.po` (1,765 lines)
- `addons/sms/i18n/pt.po` (1,717 lines)
- `addons/sms/i18n/pt_BR.po` (1,760 lines)
- `addons/sms/i18n/ro.po` (1,750 lines)
- `addons/sms/i18n/ru.po` (1,746 lines)
- `addons/sms/i18n/sk.po` (1,664 lines)
- `addons/sms/i18n/sl.po` (1,690 lines)
- `addons/sms/i18n/sms.pot` (1,636 lines)
- `addons/sms/i18n/sr@latin.po` (1,662 lines)
- `addons/sms/i18n/sv.po` (1,749 lines)
- `addons/sms/i18n/th.po` (1,698 lines)
- `addons/sms/i18n/tr.po` (1,757 lines)
- `addons/sms/i18n/uk.po` (1,697 lines)
- `addons/sms/i18n/uz.po` (1,956 lines)
- `addons/sms/i18n/vi.po` (1,740 lines)
- `addons/sms/i18n/zh_CN.po` (1,702 lines)
- `addons/sms/i18n/zh_TW.po` (1,697 lines)
- `addons/sms/models/__init__.py` (15 lines)
- `addons/sms/models/iap_account.py` (35 lines)
- `addons/sms/models/ir_actions_server.py` (90 lines)
- `addons/sms/models/ir_model.py` (40 lines)
- `addons/sms/models/mail_followers.py` (29 lines)
- `addons/sms/models/mail_message.py` (32 lines)
- `addons/sms/models/mail_notification.py` (45 lines)
- `addons/sms/models/mail_scheduled_message.py` (48 lines)
- `addons/sms/models/mail_thread.py` (243 lines)
- `addons/sms/models/res_company.py` (11 lines)
- `addons/sms/models/sms_sms.py` (267 lines)
- `addons/sms/models/sms_template.py` (71 lines)
- `addons/sms/models/sms_tracker.py` (99 lines)
- `addons/sms/security/ir.access.csv` (11 lines)
- `addons/sms/static/description/icon.png` (12 lines)
- `addons/sms/static/description/icon.svg` (1 lines)
- `addons/sms/static/description/icon_hi.png` (91 lines)
- `addons/sms/static/img/sms_failure.svg` (1 lines)
- `addons/sms/static/src/components/phone_field/phone_field.js` (69 lines)
- `addons/sms/static/src/components/sms_widget/fields_sms_widget.js` (61 lines)
- `addons/sms/static/src/components/sms_widget/fields_sms_widget.xml` (26 lines)
- `addons/sms/static/src/components/sms_widget/sms_char_counter.js` (66 lines)
- `addons/sms/static/src/components/sms_widget/sms_composer_template_selector.js` (57 lines)
- `addons/sms/static/src/components/sms_widget/sms_composer_template_selector.xml` (8 lines)
- `addons/sms/static/src/core/failure_model_patch.js` (23 lines)
- `addons/sms/static/src/core/notification_model_patch.js` (52 lines)
- `addons/sms/static/src/core/sms_char_counter_utils.js` (22 lines)
- `addons/sms/static/src/messaging_menu/messaging_menu_patch.js` (37 lines)
- `addons/sms/static/src/thread/message_patch.js` (36 lines)
- `addons/sms/static/tests/messaging_menu/messaging_menu_patch.test.js` (147 lines)
- `addons/sms/static/tests/mock_server/mock_models/partner.js` (10 lines)
- `addons/sms/static/tests/mock_server/mock_models/visitor.js` (7 lines)
- `addons/sms/static/tests/sms_test_helpers.js` (10 lines)
- `addons/sms/static/tests/thread/message_patch.test.js` (78 lines)
- `addons/sms/static/tests/web/sms_button.test.js` (154 lines)
- `addons/sms/tests/__init__.py` (6 lines)
- `addons/sms/tests/common.py` (355 lines)
- `addons/sms/tests/test_sms_composer.py` (145 lines)
- `addons/sms/tests/test_sms_template.py` (136 lines)
- `addons/sms/tests/test_sms_template.xml` (9 lines)
- `addons/sms/tools/__init__.py` (2 lines)
- `addons/sms/tools/sms_api.py` (145 lines)
- `addons/sms/tools/sms_tools.py` (17 lines)
- `addons/sms/views/iap_account_views.xml` (39 lines)
- `addons/sms/views/ir_actions_server_views.xml` (23 lines)
- `addons/sms/views/mail_notification_views.xml` (27 lines)
- `addons/sms/views/res_config_settings_views.xml` (13 lines)
- `addons/sms/views/res_partner_views.xml` (50 lines)
- `addons/sms/views/sms_sms_views.xml` (83 lines)
- `addons/sms/views/sms_template_views.xml` (100 lines)
- `addons/sms/wizard/__init__.py` (8 lines)
- `addons/sms/wizard/sms_account_code.py` (36 lines)
- `addons/sms/wizard/sms_account_code_views.xml` (20 lines)
- `addons/sms/wizard/sms_account_phone.py` (27 lines)
- `addons/sms/wizard/sms_account_phone_views.xml` (21 lines)
- `addons/sms/wizard/sms_account_sender.py` (25 lines)
- `addons/sms/wizard/sms_account_sender_views.xml` (27 lines)
- `addons/sms/wizard/sms_composer.py` (567 lines)
- `addons/sms/wizard/sms_composer_views.xml` (106 lines)
- `addons/sms/wizard/sms_template_preview.py` (49 lines)
- `addons/sms/wizard/sms_template_preview_views.xml` (41 lines)
- `addons/sms/wizard/sms_template_reset.py` (29 lines)
- `addons/sms/wizard/sms_template_reset_views.xml` (33 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
